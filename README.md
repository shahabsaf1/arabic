
قبل التثبيت يجب ان يكون لديك سيرفر خاص

حاول ان تصنع سيرفر لنفسك على موقع 
https://www.c9.io
التثبيت

```bash
انسخ هذا الكود اولا
sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev libevent-dev make unzip git redis-server g++ libjansson-dev libpython-dev expat libexpat1-dev
```
الان اكتب الاوامر ادناه
```bash
cd $HOME
git clone https://github.com/sajadaltaie/arabicbot
cd arabicbot
./launch.sh install
git clone --resursive https://github.com/vysheng/tg.git
cd tg
mv lua-tg.c lua-th.bkp
wget http://pastebin.com/raw.php?i=UNS6kh6k -O lua-tg.c
./configure && make
cd $HOME
cd arabicbot
./launch.sh # هنا سوف يطلب منك رقم ورمز يصلك على حسابك
```
بعد تسجيل وتثبيت لان نذهب الى data/config.lua
ولتعديل على سطر 21 كتابة لايدي الخاص بك وحفظ العمل
ثم اطفاء وتشغيل لبوت
```bash
quit  اطفاء
./launch.sh تشغيل
```
تفعيل وتعطيل اوامر الابلاجنس

اولا القي نظرا على البلاجنس

التفعيل !plugins enable [اسم البلاجنس].

التعطيل !plugins disable [اسم البلاجنس].

