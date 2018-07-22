# نصب و آماده‌سازی Arduino-IDE برای ویندوز:

#### •    [GitHub Page](https://github.com/espressif/arduino-esp32 "GitHub Page")

#### •    [Original Installation guide for windows](https://github.com/espressif/arduino-esp32/blob/master/docs/arduino-ide/windows.md)

## ۱. نصب پیش‌نیاز‌ها:

آخرین نسخه‌ی Arduino IDE را از «[arduino.cc](https://www.arduino.cc/en/Main/Software)» نصب کنید.

پایتون 2.7 را از «[python.org](https://www.python.org/downloads)» نصب کنید و در قسمت «Customize Python 2.7.X» مطابق تصویر زیر عمل کنید:

![](/ESP32/python_Installation.png)

سپس  
Git را از «git-scm.com» دانلود و نصب کنید.

#### ۲.Git GUI را باز کنید و مراحل زیر را انجام دهید:

o    گزینه‌ی «Clone Existing Repository» را انتخاب کنید.

o    محل Sketchbook تنظیم شده برای Arduino IDE خود را پیدا کنید:

برای یافتن این آدرس از داخل Arduino IDE از منوی «File&gt;Preferences» فیلد Sketchbook location مراجعه کنید. این آدرس معمولا به صورت زیر می‌باشد: C:/Users/\[YOUR\_USER\_NAME\]/Documents/Arduino

o    در Git GUI تنظیمات زیر را انجام دهید:

Source Location: [https://github.com/espressif/arduino-esp32.git](https://github.com/espressif/arduino-esp32.git)

Target Directory: \[ARDUINO\_SKETCHBOOK\_DIR\]\hardware\espressif\esp32

به جای \[ARDUINO\_SKETCHBOOK\_DIR\] آدرسی که از قسمت قبل یافته‌اید قرار‌دهید.

o    روی Clone کلیک کنید تا عملیات clone انجام شود.

۳. به آدرس «\[ARDUINO\_SKETCHBOOK\_DIR\]/hardware/espressif/esp32» رفته و با کلیک راست و انتخاب گزینه‌ی «Git Bash Here» ترمینال Git Bash را باز کنید و دستور زیر را اجرا کنید:

•    git submodule update --init --recursive

۴. پوشه‌ی « \[ARDUINO\_SKETCHBOOK\_DIR\]/hardware/espressif/esp32/tools» را باز‌کرده و «get.exe» را اجرا‌کنید.

o    وقتی «get.exe» به پایان برسد محتویات این پوشه چیزی مشابه این تصویر خواهد بود:

۵. ماژول Esp32 خود را به کامپیوتر متصل کنید و منتظر بمانید تا درایور آن نصب شود.

o    اگر به اینترنت متصل باشید در Windows 10 درایور اکثر برد‌ها خود‌به‌خود نصب می‌شود.

o    در صورتی که درایور نصب نشد باید به صورت دستی درایور آن را نصب کنید!

o    این درایور به قسمت Usb to Serial شما مربوط می‌شود.

o    با جستجوی مدل ماژول خود در گوگل به نتایج خوبی دست پیدا می‌کنید!

o    برای مدل Node MCU ESP32-S درایور مربوط به cp2102 همراه این آموزش قرار دارد.

۶. بورد خود را از منوی «Tools &gt; Board» انتخاب کنید. \( به طور مثال Node MCU ESP32-S\)

۷. پورت خود را از منوی «Tools &gt; port» انتخاب کنید.

۸. مثال Blink که در بخش Examples همراه این آموزش قرار دارد را پروگرم کنید تا از صحت نصب خود اطمینان یابید.

o    ممکن است لازم باشد LED\_PIN را تغییر دهید. برای بورد Node MCU ESP32-S به GPIO2 متصل است.

o    در برخی بورد‌ها ممکن است لازم باشد پیش از پروگرم کردن ESP32 را به download mode ببریم. برای این کار باید دکمه‌ی reset \(یا EN \) را نگاه داشته \(به زمین وصل کنیم\). در همین حال GPIO0 به زمین متصل می‌کنیم \(یعنی کلید متناظر که معمولا به اسم boot شناخته می‌شود فشرده شود\) سپس ابتدا کلید ریست را رها می‌کنیم و سپس کلید boot.

در این مرحله اگر Serial monitor در baud rate مناسب \(معمولاً ۱۱۵۲۰۰\) باز باشد می‌توانید فرآیند ریست شدن ESP32 را دنبال کنید.

