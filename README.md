# llama2.c_dos
這是一個 djgpp版本的 llama2.c 中的run.c
並在FreeDos 1.3 and DosBox 中測試通過
編譯使用
Djgpp
bnu2351b.zip
csdpmi7b.zip
djdev205.zip
gcc1030b.zip
gpp1030b.zip

把這些檔案解壓縮到 c:\djgpp
Freedos下
fdauto.bat中加入
path=%path%;c:\djgpp\bin
set djgpp=c:\djgpp\djgpp.env

DosBox下 
[autoexec]
mount c: /home/youliang/Dosbox_gcc
path=%path%;c:\djgpp\bin
set djgpp=c:\djgpp\djgpp.env

編譯
gcc run.c -lm -o run.exe 

且要加入 HuggingFace
stories260K/tok512.bin
改名為 c:\token.bin
stories260K/stories260K.bin
改名為 
F260k.bin
執行
C:\run.exe f260k.bin -t 0.8 -n 256 -i "One day, Lily met a Shoggoth"



