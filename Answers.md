# پاسخ تمرین‌ها

## ۱. Git چیست؟
Git یک ابزار کنترل نسخه است. از تغییرات پروژه «نسخه» (commit) نگه می‌دارد تا بتوان به نسخه‌های قبلی برگشت، تغییرات را بررسی کرد و چند نفر هم‌زمان روی یک پروژه کار کنند.

## ۲. تفاوت Git و GitHub
- **Git**: برنامه‌ای که روی کامپیوتر نصب می‌شود و نسخه‌ها را مدیریت می‌کند.
- **GitHub**: سرویس آنلاینی که repositoryهای Git را روی اینترنت نگه می‌دارد و امکان اشتراک‌گذاری و همکاری می‌دهد.

## ۳. کلاس‌ها

| کلاس | صفات (Properties) | رفتارها (Methods) |
|---|---|---|
| Customer | Id, Name, Email, Address | PlaceOrder(), UpdateAddress() |
| Student | StudentId, Name, Grade, Major | Enroll(), SubmitAssignment() |
| Teacher | TeacherId, Name, Subject, Salary | Teach(), GradeExam() |
| Employee | EmployeeId, Name, Position, Salary | Work(), CalculateBonus() |
| Rectangle | Width, Height | CalculateArea(), CalculatePerimeter() |
| Square | SideLength | CalculateArea(), CalculatePerimeter() |
| Dog | Name, Age, Breed | Bark(), Fetch() |
| Cat | Name, Age, Color | Meow(), Purr() |

## ۴. HTTP چیست؟
HTTP (Hypertext Transfer Protocol) پروتکل ارتباط بین مرورگر (کلاینت) و سرور است. مرورگر درخواست می‌فرستد و سرور پاسخ می‌دهد. داده‌ها **رمزنگاری‌نشده** منتقل می‌شوند.

## ۵. HTTPS چیست؟
HTTPS نسخه‌ی امن HTTP است. ارتباط با استفاده از TLS/SSL **رمزنگاری** می‌شود.

## ۶. تفاوت HTTP و HTTPS
| ویژگی | HTTP | HTTPS |
|---|---|---|
| رمزنگاری | ندارد | دارد (TLS) |
| پورت پیش‌فرض | 80 | 443 |
| امنیت | پایین | بالا |
| گواهی SSL | نیاز ندارد | نیاز دارد |
| نماد قفل در مرورگر | ندارد | دارد |

## ۷. چرا بیشتر وب‌سایت‌ها از HTTPS استفاده می‌کنند؟
- محافظت از اطلاعات حساس (رمز عبور، کارت بانکی) در برابر شنود
- جلوگیری از تغییر داده‌ها در مسیر
- تأیید هویت سایت
- مرورگرها سایت‌های HTTP را «Not Secure» نشان می‌دهند
- گوگل در رتبه‌بندی (SEO) به HTTPS امتیاز می‌دهد
- گواهی رایگان (مثل Let's Encrypt) در دسترس است

## ۸. URL چیست؟
URL (Uniform Resource Locator) آدرس یک منبع در اینترنت است.

مثال: `https://www.example.com:443/products/shoes?color=red&size=42#reviews`

| بخش | مقدار | توضیح |
|---|---|---|
| Scheme (پروتکل) | https | نوع پروتکل |
| Host (دامنه) | www.example.com | آدرس سرور |
| Port | 443 | پورت (معمولاً مخفی است) |
| Path (مسیر) | /products/shoes | مسیر منبع روی سرور |
| Query (پارامترها) | ?color=red&size=42 | داده‌های اضافه به‌صورت کلید=مقدار |
| Fragment | #reviews | بخشی از صفحه |

## ۹. GET چیست؟
متدی برای **دریافت** اطلاعات از سرور. پارامترها در URL می‌آیند.

## ۱۰. POST چیست؟
متدی برای **ارسال** اطلاعات به سرور (ساخت یا ثبت داده). داده‌ها در بدنه‌ی (Body) درخواست قرار می‌گیرند.

## ۱۱. تفاوت GET و POST
| ویژگی | GET | POST |
|---|---|---|
| هدف | دریافت داده | ارسال/ثبت داده |
| محل داده | در URL | در Body |
| امنیت | کمتر (داده در URL دیده می‌شود) | بیشتر |
| محدودیت حجم | دارد | تقریباً ندارد |
| کش و بوکمارک | قابل‌انجام | معمولاً خیر |
| تغییر داده روی سرور | نمی‌دهد | می‌دهد |

## ۱۲. کاربرد GET
نمایش صفحه، جست‌وجو، فیلتر کردن، دریافت لیست محصولات، دریافت اطلاعات یک کاربر.

## ۱۳. کاربرد POST
ثبت‌نام، ورود (login)، ارسال فرم، ثبت سفارش، آپلود فایل، ارسال نظر.

## ۱۴. مثال واقعی API
- **GET**: `GET https://api.github.com/users/octocat` ← اطلاعات یک کاربر GitHub را برمی‌گرداند.
- **POST**: `POST https://jsonplaceholder.typicode.com/posts` ← یک پست جدید می‌سازد (بدنه: `{"title":"hello","body":"text","userId":1}`).

## ۱۵. JSON چیست؟
JSON (JavaScript Object Notation) فرمت سبک و خوانا برای نمایش و تبادل داده به‌صورت جفت «کلید: مقدار» است.

## ۱۶. XML چیست؟
XML (eXtensible Markup Language) زبان نشانه‌گذاری با تگ‌های سفارشی برای ذخیره و انتقال داده است.

## ۱۷. کاربردها
- **JSON**: APIهای وب، ارتباط فرانت‌اند و بک‌اند، فایل‌های تنظیمات
- **XML**: فایل‌های تنظیمات (مثل `.csproj`)، سرویس‌های SOAP، RSS، اسناد ساختارمند

## ۱۸. تفاوت JSON و XML
| ویژگی | JSON | XML |
|---|---|---|
| ساختار | کلید/مقدار | تگ‌های باز و بسته |
| حجم | کمتر | بیشتر |
| خوانایی | ساده‌تر | پرحرف‌تر |
| آرایه | پشتیبانی مستقیم | ندارد (تگ تکراری) |
| کامنت | ندارد | دارد |
| سرعت پردازش | سریع‌تر | کندتر |

## ۱۹. اطلاعات Student

**JSON**
```json
{
  "studentId": 1001,
  "name": "Ali Rezaei",
  "age": 20,
  "major": "Computer Engineering",
  "grade": 18.5
}
```

**XML**
```xml
<student>
  <studentId>1001</studentId>
  <name>Ali Rezaei</name>
  <age>20</age>
  <major>Computer Engineering</major>
  <grade>18.5</grade>
</student>
```
