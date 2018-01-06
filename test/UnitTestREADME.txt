Creating and adding new unit tests - 

> Prerequisites : 
1. 16 bit PCM mono wav file sampled at 16 kHz
2. .srt file for the .wav file
3. CCAligner installed along with all dependencies.

>Steps : 

1. Generate .json file for your wav file using CCAligner - ./ccalinger -wav <wav_file>.wav -srt <srt_file>.srt -oFormat json
NOTE: Make sure that name of all the files is same.

2. Copy the unit test files (.wav, .srt & .json) to CCAligner/test/data and paste them there. Create a new file with the same contents as .json file and add .expected in the end of its name. (For example, if the json file was "a.json" the new file should be named "a.json.expected").

3. Add the name of your unit test to /test/test_info.json





