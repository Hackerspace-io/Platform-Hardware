[pyInstallRef]: /ESP32/python_Installation.png
# مثال markdown:
این یک مثال markdown برای بررسی نوشتار‌های مختلف آن است.

## ۱. بررسی حالت‌های مختلف markdown:

+ #### [GitHub Page](https://github.com/espressif/arduino-esp32 "GitHub Page")

+ #### [Original Installation guide for windows](https://github.com/espressif/arduino-esp32/blob/master/docs/arduino-ide/windows.md)

## لینک‌های مرتبط:
- [source md](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/doc/user/markdown.md)
- [gitlab guide](https://about.gitlab.com/handbook/product/technical-writing/markdown-guide/#markdown-style-guide-for-aboutgitlabcom)
- [syntax](https://daringfireball.net/projects/markdown/syntax)
- [tester](https://daringfireball.net/projects/markdown/dingus)

## لیست‌ها و ~ و ـ و * و backward tick
* **آخرین** نسخه‌ی `Arduino IDE` را از [arduino.cc](https://www.arduino.cc/en/Main/Software) نصب کنید.
    * این یک ~~تست~~ __*یک* سند__ است!
      1. __gitlab test__
      1. **gitlab test**
        - ۱. فارسی باید دستی بنویسیم.
        + ۲. که شماره هاش اوکی بشه.
    + _gitlab test_
    * *gitlab test*
    + __میتونیم *ترکیب* کنیم__
* نسخه‌ی`python 2.7` را از [python.org](https://www.python.org/downloads) نصب کنید و در قسمت `Customize Python 2.7.X` مطابق تصویر زیر عمل کنید:
![python_installation](/ESP32/python_Installation.png)

> this one has tooltip
![python_installation](/ESP32/python_Installation.png  "this is a tooltip")

دستکاری اندازه‌ها به صورت html
> and this is as is <img src="/ESP32/python_Installation.png" alt="nothing2" width=80% height=100>

این عکس اومده راست چون ادامه متن فارسی بوده![python_installation](/ESP32/python_Installation.png)



## emoji test
می‌توان ایموجی گذاشت! 😄 از این  [سایت](https://www.emojicopy.com/)

## قرار دادن کد به این صورت:
```c
void main(){
  printf("hello world");
}
```
```cpp
void onMqttPublish(uint16_t packetId) {
  Serial.println("Publish acknowledged.");
  Serial.print("  packetId: ");
  Serial.println(packetId);
}
```
```python
def hello():
    #indenting works just fine in the fenced code block
    s = "Python syntax highlighting"
    print s
```
## quote:
>این متن یک placeHolder است
>و این یک quote است.

>>>
Many small embedded systems exist to collect data from sensors, analyse the data, and either take an appropriate action or send that sensor data to another system for processing.

One of the many challenges of embedded systems design is the fact that parts you used today may be out of production tomorrow, or system requirements may change and you may need to choose a different sensor down the road.

>inner quote

Creating new drivers is a relatively easy task, but integrating them into existing systems is both error prone and time consuming since sensors rarely use the exact same units of measurement.

By reducing all data to a single sensors_event_t 'type' and settling on specific, standardised SI units for each sensor family the same sensor types return values that are comparable with any other similar sensor. This enables you to switch sensor models with very little impact on the rest of the system, which can help mitigate some of the risks and problems of sensor availability and code reuse.
>>>
## تست جدول:
هدر اولی | هدر دومی | dejwp
------------ | ------------- | ----
سلول۱ |  | left cell empty
Content in the first column | Content in the second column | st

## فرمول:
```math
a^2+2ab+b^2
```
خط کشیدن بین متن

---
بعد از خط
