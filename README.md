# MFT Music Player

شروع پروژه‌ی موزیک‌پلیر تیم MFT بر پایه‌ی Android Media3.

## تیم

| نفر | نقش | مسئولیت |
| --- | --- | --- |
| [Amin Sakha](https://github.com/aminsakha) (`@aminsakha`) | Project/Repository Owner | هماهنگی پروژه، مدیریت ریپو و تصمیم‌های نهایی |
| `behnam` | Android/Media3 Developer | راه‌اندازی Media3 و پیاده‌سازی اتصال Player |

> طبق برد Trello، تسک‌های اجرایی MVP به `behnam` تخصیص داده شده‌اند. اگر هندل GitHub بهنام متفاوت است، منشن README و Reviewers را با هندل دقیق به‌روزرسانی کنید.

## MVP فعلی

- **Set Up Media3 Framework** — راه‌اندازی وابستگی‌ها و اسکلت Media3. مسئول: `behnam` — [Trello](https://trello.com/c/iRuCxnPp/67-set-up-media3-framework)
- **Implement Media3 Player Integration** — اتصال Player و آماده‌سازی پخش موسیقی. مسئول: `behnam` — [Trello](https://trello.com/c/Bb5vsWHt/68-implement-media3-player-integration)
- **MVP Version** — کارت مادر اسپرینت MVP — [Trello](https://trello.com/c/zTHovh5v/65-mvp-version)

تاریخ سررسید ثبت‌شده برای دو تسک اجرایی: **2026-08-22**.

برد برنامه‌ریزی: [MFT | Music_Player در Trello](https://trello.com/b/ruH9Ggzz/mft-musicplayer)

## استراتژی Git

شاخه‌ی پیش‌فرض ریپو `master` است و فقط نقش release/stable دارد. توسعه‌ی روزمره باید از `develop` انجام شود.

1. همیشه آخرین `develop` را بگیرید:

   ```bash
   git switch develop
   git pull origin develop
   ```

2. برای هر تسک یک شاخه از `develop` بسازید:

   ```bash
   git switch -c feature/<short-task-name>
   ```

3. تغییرات را با commitهای کوچک و معنادار push کنید و یک Pull Request به `develop` باز کنید.
4. در PR، کارت Trello مرتبط، خلاصه‌ی تغییرات و روش تست را بنویسید و **Behnam (`@behnam`)** را برای review منشن کنید؛ همچنین لینک PR و وضعیت آن را در گروه اعلام کنید.
5. تا قبل از تأیید review و پاس‌شدن تست‌ها، PR را merge نکنید. merge به `master` فقط برای release و با هماهنگی مالک پروژه انجام می‌شود.

### نام‌گذاری شاخه‌ها

- `feature/<name>` برای قابلیت جدید
- `fix/<name>` برای رفع باگ
- `refactor/<name>` برای بازآرایی بدون تغییر رفتار
- `chore/<name>` برای کارهای build، dependency و tooling

## وضعیت شاخه‌ها

- `master`: شاخه‌ی پیش‌فرض و پایدار
- `develop`: شاخه‌ی ادغام توسعه

## وضعیت پروژه

این ریپو نقطه‌ی شروع پروژه است. ساختار اپلیکیشن، تست‌ها و CI هم‌زمان با شکستن کارت‌های MVP اضافه می‌شوند.
