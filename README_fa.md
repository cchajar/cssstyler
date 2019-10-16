# سلب مسئولیت #

این پروژه یک شاخه جدا شده است . نگاهی بیندازید به  [پروژه‌ی اصلی](https://github.com/senchalabs/cssbeautify) .

# زیباساز سی.اس.اس #

 زیباساز سی.اس.اس یک پروژه اجرایی به زبان جاوااسکریپت است که کد های استایل‌دهی نوشته شده به زبان [سی.اس.اس](http://www.w3.org/Style/CSS/) را مرتب و دندانه‌دهی می‌کند . 

استایل زیر را به زیباساز سی.اس.اس بدهید :

```css
menu{color:red} navigation{background-color:#333}
```

زیباساز سی.اس.اس کد زیر را به شما تحویل می‌دهد :

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

می‌توانید به صورت آنلاین امتحان کنید :  [amirmehrabi.github.io/cssstyler/](https://amirmehrabi.github.io/cssstyler/).

همچنین ، برای مثال های بیشتر نگاهی بیندازید به [مجموعه تست ها](http://cssbeautify.com/test/).


# Screenshots #

![screencapture-localhost-cssstyler-index-en-html-2019-10-15-15_36_23](https://user-images.githubusercontent.com/3878847/66830108-93ad8700-ef61-11e9-95d9-df30792b5aef.png)

## استفاده از تابع cssbeautify() ##

از آن جایی که زیباساز سی.اس.اس با جاوااسکریپت خام ( بدون هیچگونه وابستگی ) نوشته شده است ، هر جایی که جاوااسکریپت بتواند اجرا شود ، زیباساز سی.اس.اس نیز می‌تواند اجرا شود .

API بسیار ساده است :

```javascript
var result = cssbeautify(style, options);
```

**options** یک شی ء اختیاری برای تنظیم و سازگار کردن مرتب‌‍‌‌سازی می‌باشد . گزینه های شناخته شده تا به این لحظه :

  *  <code>indent</code> یک رشته متنی برای دندانه‌دهی است. ( به طور پیش‌فرض با 4 فاصله )  
  *  <code>openbrace</code> محل آکولاد باز را تعریف می‌کند , می‌تواند *end-of-line* (پیش‌فرض) یا *separate-line* باشد.
  *  <code>autosemicolon</code> همیشه بعد از آخرین قاعده ، سمی‌کالِن اضافه می‌کند . (به طور پیش‌فرض *false*)

مثال فراخوانی :

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## مشارکت در پروژه ##

از مشارکت ها استقبال می‌شود! برای اطلاعات بیشتر لطفا [راهنمای همکاری](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) را مطالعه کنید

## مجوز ##

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

بدین وسیله ، به هر فردی که نسخه ای از این نرم‌افزار و مستندات مرتبط با آن را در دست دارد ، بدون دریافت هزینه ای مجوز داده می‌شود که از نرم افزار بدون هیچ محدودیتی استفاده کند . این استفاده شامل : بهره‌وری ، کپی ‌، اصلاح ، ادغام ، انتشار ، تعمیم ، و/یا فروش نسخه ای از نرم‌افزار ،

حقوق‌ کپی‌رایت که در بالا ذکر شده و این مجوز ، باید در تمامی نسخه های کپی و بخش های مهم نرم افزار ، ذکر شود .

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
