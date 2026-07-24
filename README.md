# MFT Music Player

شروع پروژه‌ی موزیک‌پلیر تیم MFT بر پایه‌ی Android Media3.

## تیم

| نفر | نقش | مسئولیت |
| --- | --- | --- |
| [Amin Sakha](https://github.com/aminsakha) (`@aminsakha`) | Project Owner & Project Coordinator | مالک پروژه، هماهنگی تیم، مدیریت ریپو و تصمیم‌های نهایی |
| `behnam` | Developer | راه‌اندازی Media3 و پیاده‌سازی اتصال Player |
| `mohamad ali farajolahi` | Developer | اسکن فایل‌های صوتی و نمایش کتابخانه موسیقی |
| `Shayan armannia` | Developer | پیاده‌سازی پخش صدا و صفحه Player |
| `مهدیار قزوینیان` | Developer | پیاده‌سازی صف پخش و جست‌وجوی آهنگ‌ها |
| `Abolfazl Khalili` | Developer | اعلان Media، آهنگ‌های اخیر و آماده‌سازی انتشار |
| `Parsa` | Developer | آهنگ‌های موردعلاقه، تنظیمات و آماده‌سازی انتشار |
| `Leila Abdi` | Developer | تست و کنترل کیفیت |

> این فهرست بر اساس کارت‌هایی است که در برد Trello به اعضا assign شده‌اند. نام‌ها عیناً از Trello استخراج شده‌اند؛ برای منشن GitHub، هندل دقیق هر نفر باید در GitHub مشخص شود.

## MVP فعلی

- **Set Up Media3 Framework** — راه‌اندازی وابستگی‌ها و اسکلت Media3. مسئول: `behnam` — [Trello](https://trello.com/c/iRuCxnPp/67-set-up-media3-framework)
- **Implement Media3 Player Integration** — اتصال Player و آماده‌سازی پخش موسیقی. مسئول: `behnam` — [Trello](https://trello.com/c/Bb5vsWHt/68-implement-media3-player-integration)
- **MVP Version** — کارت مادر اسپرینت MVP — [Trello](https://trello.com/c/zTHovh5v/65-mvp-version)

### سایر تخصیص‌های Trello

- `mohamad ali farajolahi`: [Scan Local Audio Files](https://trello.com/c/XB70yd1y/44-scan-local-audio-files)، [Display Music Library](https://trello.com/c/pYjvZUcC/45-display-music-library)
- `Shayan armannia`: [Implement Audio Playback](https://trello.com/c/dgzyHG6T/47-implement-audio-playback)، [Create Player Screen](https://trello.com/c/zXqN6u07/48-create-player-screen)
- `مهدیار قزوینیان`: [Implement Queue](https://trello.com/c/l3McHqns/50-implement-queue)، [Search Songs](https://trello.com/c/nlHJAOOX/46-search-songs)
- `Abolfazl Khalili`: [Media Notification](https://trello.com/c/JSYMOTBb/53-media-notification)، [Recently Played Songs](https://trello.com/c/dSi69QCt/54-recently-played-songs)، [App Polish & Release](https://trello.com/c/Q5vO5Aq1/58-app-polish-release)
- `Parsa`: [Favorite Songs](https://trello.com/c/vmn4GiSQ/56-favorite-songs)، [Settings](https://trello.com/c/a8Cs31Qa/57-settings)، [App Polish & Release](https://trello.com/c/Q5vO5Aq1/58-app-polish-release)
- `Leila Abdi`: [Testing](https://trello.com/c/M4MjQpbC/7-testing)

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
