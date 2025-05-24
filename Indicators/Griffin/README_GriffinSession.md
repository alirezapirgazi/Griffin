# 🟪 GriffinSession

## 📌 توضیح کوتاه (فارسی)

**GriffinSession** ابزاری جامع برای نمایش سشن‌های بازار، نواحی مهم و رویدادهای خبری در نمودار است. این ابزار چند عملکرد مهم دارد:

* نمایش سشن‌های اصلی بازار (آسیا، اروپا، آمریکا) در یک قاب با سقف و کف هر سشن
* نمایش **برچسب نام سشن** همراه با **زمان باقی‌مانده تا پایان سشن** (اگر فعال باشد)
* نمایش **زمان باقی‌مانده تا شروع سشن** (اگر هنوز آغاز نشده باشد)
* نمایش سقف و کف بازار در روز قبل در یک قاب مجزا
* اگر چارت مربوط به طلا باشد (XAUUSD)، نمایش محدوده‌هایی که به تجربه شخصی توسعه‌دهنده، تریدرهای بانک‌ها در آن شروع به معامله می‌کنند
* دریافت خودکار اخبار مهم از سایت ForexFactory و نمایش آن‌ها به صورت:

  * **خط عمودی در زمان خبر**
  * **برچسب شامل نام و نوع خبر**

---

## 📌 Short Description (English)

**GriffinSession** is an advanced tool for visualizing market sessions, key price zones, and economic news on chart. Key features include:

* Displays main trading sessions (Asia, Europe, US) as zones with their high/low
* Shows **session name** and **time remaining** until close (or until start if not yet open)
* Displays previous day's high and low in a distinct frame
* For gold (XAUUSD), marks custom bank-trader zones based on developer's personal experience
* Fetches major economic events from **ForexFactory** and displays:

  * **Vertical line at event time**
  * **Label with event type and name**

---

## ⚙️ نحوه عملکرد | How It Works

### ✅ فارسی:

* شناسایی خودکار سشن فعال بازار بر اساس ساعت سیستم یا سرور
* محاسبه زمان باقی‌مانده و تعیین نوع برچسب (شروع نشده / فعال / در حال اتمام)
* دریافت داده روز گذشته برای محاسبه سقف و کف روزانه
* در چارت طلا، فعال‌سازی نواحی خاص فعالیت بانک‌ها
* استفاده از API سایت ForexFactory برای دریافت اخبار مهم روز و رسم آن‌ها روی نمودار

### ✅ English:

* Auto-detects active session by system/server time
* Calculates remaining time and shows contextual label
* Gets previous day high/low data
* Activates bank trader zones for XAUUSD only
* Uses ForexFactory API to pull major news events and draw them on chart

---

## 🌟 مزایا | Key Benefits

### فارسی:

* اطلاع از وضعیت فعلی و آینده سشن‌ها برای تحلیل بهتر زمان ورود
* هشدار بصری برای رویدادهای مهم خبری
* تشخیص نواحی مهم روز گذشته برای تعیین نقاط ورود/خروج
* ویژه معامله‌گران طلا با توجه به تجربه عملی در بازار بین‌بانکی

### English:

* Clear view of session status and time guidance
* Visual alerts for major news events
* Prior day's levels for support/resistance zones
* Gold-specific zones based on real institutional behavior
