# 这个玩意儿咋用的？
make
./main -f samples/jfk.wav
ll models/
make base
./main -f samples/jfk.wav
./main
./main -m models/ggml-base.bin -f samples/jfk.wav
./main -m models/ggml-base.bin -f samples/jfk.wav
./main -m models/ggml-base.bin -n -f samples/jfk.wav
./main -m models/ggml-base.bin -ng -f samples/jfk.wav
./main -m models/ggml-base.bin -ng -f samples/new_name_of_ldjj.wav 
./main -m models/ggml-base.bin -ng -f samples/jfk.wav
./main -m models/ggml-base.bin -ng -f samples/new_name_of_ldjj.wav 
cd examples/
cd ..
cd samples/
ffmpeg -i new_name_of_ldjj.wav -acodec pcm_s16le -ac 1 -ar 16000 out.wav
cd ..
./main -m models/ggml-base.bin -ng -f samples/out.wav 
./main -m models/ggml-base.bin -ng -l zh -f samples/out.wav 



