# 🧠 GriffinTrader

## 📌 توضیح کوتاه (فارسی)

**GriffinTrader** یک اکسپرت و پلتفرم پیشرفته مبتنی بر ساختار Griffin است که برای استفاده بهینه از تمام ابزارهای گریفین طراحی شده و دارای بخش‌های مختلفی برای مدیریت معاملات، تحلیل عملکرد، مدیریت سرمایه و استفاده از چک‌لیست‌ها و ابزارهای روانشناسی و هوش مصنوعی است.

**English:**
**GriffinTrader** is an advanced expert advisor and platform based on the Griffin structure, designed to fully utilize all Griffin tools with features for trade management, performance analysis, capital management, checklists, psychology, and AI-powered assistance.

---

## 🧾 معرفی اولیه | Startup Page

در شروع روز یا اجرای اولیه، کاربر با **صفحه معرفی** مواجه می‌شود:

* **بخش چک‌لیست ورود و خروج:**

  * دارای یک باکس متنی برای تایپ آیتم‌های چک‌لیست
  * دکمه افزودن آیتم به چک‌لیست ورود و دکمه افزودن آیتم به چک‌لیست خروج
  * حداقل ۳ آیتم برای ورود و ۱ آیتم برای خروج لازم است
  * پس از تکمیل چک‌لیست، دکمه‌ای برای ورود به چارت و فعال‌سازی GriffinTrader ظاهر می‌شود

* **جدول تحلیل عملکرد چک‌لیست:**

  * بررسی تأثیر چک‌لیست‌ها بر موفقیت معاملات بر اساس داده‌های قبلی

**English:**
At the start of the day or first launch, the user sees the **Startup Page**:

* **Entry/Exit Checklist:**

  * A textbox to write checklist items
  * Buttons to add items to entry or exit checklist
  * At least 3 items for entry and 1 for exit are required
  * After completing the checklist, a button appears to open the chart and activate GriffinTrader

* **Checklist Performance Table:**

  * Analyzes how the checklist has impacted trade success based on past data

---

## 🧩 GriffinTrader Management Panel

### ⏱ Remaining Trade

* تایمر ۴۵ دقیقه‌ای برای مجاز بودن معامله
* پس از اتمام زمان، صفحه چارت به مدت ۱۵ دقیقه سیاه می‌شود (زمان استراحت)
* در این زمان فقط مدیریت معامله باز ممکن است (نه باز کردن معامله جدید)
* دکمه‌ای برای مشاهده چارت بدون امکان انجام معامله

**English:**

* 45-minute timer allowing active trading
* After time ends, the chart goes black for 15 minutes (rest time)
* During rest, only open trades can be managed—not new ones
* A button lets you view the chart without trading ability

### 🔐 Account Status

اطلاعات حساب کاربری و وضعیت سبد معاملات:

* **Account Info:** نام صاحب حساب، نوع حساب
* **Usable:** مقدار پول مجاز برای ترید امروز (بین ۵ دلار تا ۲٪ موجودی)

  * اگر صفر شود، اجازه باز کردن معامله ندارید
  * اگر منفی شود، متاتریدر بسته می‌شود
* **Used:** مقدار استفاده‌شده از سرمایه مجاز
* **Now:** سود/ضرر لحظه‌ای معاملات باز به درصد
* **Day:** سود/ضرر معاملات امروز
* **W/R:** درصد معاملات موفق
* **Spread:** مقدار اسپرد فعلی بازار

**English:**

* **Account Info:** Account owner and type
* **Usable:** Capital available for today (from \$5 to 2% of balance)

  * If it hits zero, you can’t open new trades
  * If it turns negative, MetaTrader will close
* **Used:** Capital already committed
* **Now:** Live PnL (percentage)
* **Day:** PnL of today
* **W/R:** Win rate
* **Spread:** Current market spread

### 🛒 Open Trade

مراحلی برای باز کردن معامله:

1. **Entry:**

   * دکمه‌ای برای قرار دادن خط Op (ورود)
   * خط آبی افقی قابل تنظیم روی چارت
   * در صورت فشردن گزینه Instance، خط به قیمت لحظه‌ای بازار متصل می‌شود

2. **Set SL:**

   * خط نارنجی به‌عنوان حدضرر همراه با برچسب شامل:

     * فاصله تا نقطه ورود (پیپت)
     * مبلغ استفاده‌شده (USD)
     * حجم لات معامله
   * هم‌زمان دکمه‌هایی برای انتخاب استراتژی مدیریت سرمایه:

     * 100٪، 50٪، 30٪ از Usable
     * MaxLot: بیشترین حجم با توجه به Usable
     * FullMargin: بر پایه موجودی کل حساب (تنها در صورت فعال‌سازی در تنظیمات اولیه)

3. **Set TP1, TP2, TP3:**

   * خطوط سبز برای تعیین نقاط سود با نمایش نسبت R/R

4. **دکمه ثبت معامله:**

   * فقط اگر شرایط (مانند اسپرد، موجودی) برقرار باشد
   * رنگ دکمه بسته به نوع معامله (Buy آبی / Sell قرمز)
   * هم‌زمان تصویر چارت ذخیره و ژورنال خودکار ایجاد می‌شود

**English:**
Steps to open a trade:

1. **Entry:**

   * Add Op line (blue) to the chart
   * Adjustable line; can attach to market price via Instance button
2. **Set SL:**

   * Orange line shows:

     * Distance to entry (pipettes), risk in USD, trade lot size
   * Capital buttons:

     * 100%, 50%, 30% of Usable
     * MaxLot (max volume using Usable)
     * FullMargin (uses full account balance—only visible if activated in settings)
3. **Set TP1, TP2, TP3:**

   * Green lines with R/R info
4. **Trade Execution Button:**

   * Appears only if all filters pass
   * Blue for Buy, Red for Sell
   * Saves chart snapshot and creates journal entry

---

### 📊 Management Panel

(در زمان فعال بودن معامله)

* **Deleted All:** حذف معاملات لیمیت
* **Close All:** بستن تمام معاملات فعال
* **Close 1/2:** بستن ۵۰٪ حجم هر معامله
* **TP1/TP2/TP3:** انتقال TakeProfit به یکی از سطوح تعیین‌شده
* **SLZeroAll / SLZeroOne:** انتقال حدضرر به نقطه ورود (breakeven)
* **SL Back:** قرار دادن SL در بالای/پایین کندل قبل

**English:**

* **Deleted All:** Remove all pending limit orders
* **Close All:** Close all open trades
* **Close 1/2:** Close 50% of each position
* **TP1/TP2/TP3:** Set TakeProfit to one of the defined levels
* **SLZeroAll / SLZeroOne:** Move SL to entry point
* **SL Back:** Move SL to above/below previous candle

---

### 📋 Check List

#### Open Checklist:

* مشاهده چک‌لیست ورود از صفحه معرفی
* پاسخ به سه سوال:

  1. آیا خواب کافی داشته‌اید؟ (بله/خیر)
  2. احساس امروزتان چیست؟ (خنثی، هیجان‌زده، شک، ناامید، اعتمادبه‌نفس زیاد)
  3. درصد اعتماد به معامله (۱-۱۰۰٪)
* پس از پاسخ به سوالات و تایید چک لیست ورود به معامله و هشدارهای هوش مصنوعی، مجاز به باز کردن معامله خواهید بود

**English:**

* Entry checklist from startup page
* Answer 3 questions:

  1. Did you sleep well? (Yes/No)
  2. How do you feel today? (Neutral, Excited, Doubtful, Frustrated, Overconfident)
  3. Confidence in this trade (1–100%)
* After confirming the checklist and AI warning review, you’ll be allowed to open trades

#### Close Checklist:

* مشاهده چک‌لیست خروج
* با تأیید، معامله بسته خواهد شد

**English:**

* View exit checklist
* Upon confirmation, the trade will be closed

---

### 🛠 Griffin Tools

* دکمه‌هایی برای فعال/غیرفعال‌سازی اندیکاتورهای Griffin (با نام هر اندیکاتور)
* دکمه Clear All برای حذف تمام اندیکاتورها
* دکمه حذف تمام خطوط ترسیم‌شده روی چارت

**English:**

* Buttons to toggle Griffin indicators (by name)
* Clear All button removes all indicators
* Button to delete all drawn lines on the chart

---

## 🌟 مزایا | Benefits

### فارسی:

* تضمین ورود و خروج بر پایه اصول مدیریت ریسک و روانشناسی
* ایجاد ژورنال خودکار برای یادگیری از معاملات گذشته
* جلوگیری از overtrade و رعایت سرمایه مجاز روزانه

### English:

* Structured entries/exits based on risk and mental filters
* Auto journaling for post-trade analysis
* Avoids overtrading by enforcing capital limits

---

📌 این ابزار مناسب تریدرهایی است که می‌خواهند معاملاتشان را با **انضباط حرفه‌ای** و **هوش مصنوعی شخصی‌سازی‌شده** انجام دهند.

📌 This tool is ideal for traders who want to trade with **professional discipline** and **personalized AI support**.
