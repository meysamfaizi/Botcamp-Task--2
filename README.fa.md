# منوی حساب کاربری — Task 2

<p align="center">
  <a href="README.md">English</a> •
  <a href="README.fa.md"><bdi>فارسی</bdi></a>
</p>

<div dir="rtl">

- نسخه آنلاین: https://meysamfaizi.github.io/Botcamp-Task--2/
- مخزن پروژه: https://github.com/meysamfaizi/Botcamp-Task--2

## معرفی

کارت «منوی حساب کاربری» برای یک فروشگاه اینترنتی فارسی. سند به‌صورت
`lang="fa"` و `dir="rtl"` نوشته شده و رابط از دو بخش تشکیل می‌شود:
سربرگ پروفایل (آواتار، نام، شماره موبایل، دکمه ویرایش) و فهرست ناوبری
حساب کاربری که هر آیتم آن یک آیکون SVG داخلی دارد.

## چالش

- ساخت چیدمان کامل RTL با تراز درست آیکون، متن و دکمه‌ها
- نام‌گذاری منظم با BEM برای یک بلوک قابل استفاده مجدد
- مدیریت رنگ‌ها با متغیرهای CSS به‌جای مقادیر تکراری
- تمایز حالت فعال منو از سایر آیتم‌ها
- هماهنگ‌شدن رنگ آیکون‌ها با رنگ متن لینک

## ساخته‌شده با

- HTML5 معنایی (`main`، `section`، `header`، `nav`، `ul`)
- Flexbox و Grid
- متغیرهای CSS در `:root`
- قاعده نام‌گذاری BEM
- آیکون‌های SVG داخلی با `currentColor`
- Media Query برای واکنش‌گرایی
- فونت ایران‌یکان با `@font-face`

## ساختار پروژه

</div>
```text
Task2/
├── index.html
├── README.md
├── README.fa.md
├── assets/
│   └── fonts/
│       └── IRANYekanBold.ttf
└── src/
├── font.css
└── style.css

<div dir="rtl">

## ساختار BEM

بلوک اصلی `account-menu` است و المان‌های آن:

| کلاس                     | نقش                   |
| ------------------------ | --------------------- |
| `account-menu__profile`  | سربرگ پروفایل         |
| `account-menu__avatar`   | آواتار کاربر          |
| `account-menu__identity` | ظرف نام و شماره       |
| `account-menu__name`     | نام کاربر             |
| `account-menu__phone`    | شماره موبایل ماسک‌شده |
| `account-menu__edit`     | دکمه ویرایش پروفایل   |
| `account-menu__nav`      | ناوبری منو            |
| `account-menu__list`     | فهرست آیتم‌ها         |
| `account-menu__item`     | آیتم فهرست            |
| `account-menu__link`     | لینک آیتم             |
| `account-menu__icon`     | آیکون SVG آیتم        |

مودیفایر: `account-menu__link--active` برای آیتم فعال.
کلاس عمومی: `card` به‌عنوان ظرف بیرونی.

## متغیرهای رنگ

رنگ‌ها در `:root` فایل `src/style.css` تعریف شده‌اند:

`--color-surface` · `--color-bg` · `--color-text` · `--color-muted` ·
`--color-active` · `--color-danger` · `--color-badge` ·
`--color-border` · `--color-order-cart`

## ویژگی‌ها

- چیدمان RTL-first با تراز منطقی درست
- برچسب‌گذاری دسترس‌پذیر با `aria-label` روی بخش منو و دکمه ویرایش
- آیکون‌های SVG مقیاس‌پذیر و مستقل از فایل خارجی
- تفکیک استایل فونت (`font.css`) از استایل رابط (`style.css`)

## راه‌اندازی

</div>

bash
git clone https://github.com/meysamfaizi/Botcamp-Task--2.git
cd Botcamp-Task--2

<div dir="rtl">

سپس `index.html` را در مرورگر باز کنید یا با افزونه Live Server در VS Code اجرا کنید.

## توسعه‌های آینده

- افزودن ناوبری با کیبورد بین آیتم‌های منو
- تم تاریک با تغییر مقادیر متغیرهای `:root`
- افزودن وزن‌های بیشتر فونت (Regular و Medium)
- انیمیشن ورود ملایم برای آیتم‌های فهرست

## منابع مفید

- [MDN — CSS Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout)
- [MDN — currentColor](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)
- [MDN — Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)
- [روش BEM](https://getbem.com/)

## نویسنده

- میثم فیضی
- گیت‌هاب: [@meysamfaizi](https://github.com/meysamfaizi)

## مجوز

منتشرشده تحت مجوز MIT.

</div>

## دو مشکل که باید قبل از انتشار حل کنی

**۱. مسیر فونت مطلق است** — در `Task2/src/font.css` نوشته شده:

```css
src: url(/assets/fonts/IRANYekanBold.ttf);
```
