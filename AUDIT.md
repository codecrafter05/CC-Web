# Code Crafter Website — Full Audit & Content Plan
> **Date:** June 9, 2026 | **Domain:** https://codecrafter.cc | **Type:** Static HTML Site

---

## PART 1 — Site Map

### 1A. All HTML Pages (21 files)

| # | File | Title | Title Chars | Meta Desc Chars |
|---|------|-------|-------------|-----------------|
| 1 | `index.html` | Code Crafter — Web & Software Development Company in Bahrain | 60 ✅ | 190 ⚠️ |
| 2 | `about.html` | من نحن - Code Crafter \| الشركة التقنية الرائدة في البحرين | 57 ✅ | 253 ⚠️ |
| 3 | `contact.html` | اتصل بنا - Code Crafter \| الشركة التقنية الرائدة في البحرين | 59 ✅ | 227 ⚠️ |
| 4 | `showcase.html` | معرض المشاريع - Code Crafter \| أفضل المشاريع التقنية في البحرين | 63 ⚠️ | 223 ⚠️ |
| 5 | `multimedia.html` | الوسائط المتعددة - Code Crafter \| أفضل الحلول التقنية في البحرين | 64 ⚠️ | 204 ⚠️ |
| 6 | `shortcodes.html` | Code Crafter - Shortcodes | 25 ✅ | 69 ⚠️ (under 140) |
| 7 | `web-development-bahrain.html` | Web Development Bahrain \| Code Crafter - Custom Website Development | 67 ⚠️ | 177 ⚠️ |
| 8 | `software-development-bahrain.html` | Software Development Bahrain \| Code Crafter - Custom Software Company | 69 ⚠️ | 162 ⚠️ |
| 9 | `laravel-development-bahrain.html` | Laravel Development Bahrain \| Code Crafter - PHP Laravel Experts | 64 ⚠️ | 188 ⚠️ |
| 10 | `website-design-bahrain.html` | Website Design Bahrain \| Code Crafter - Professional Web Design Company | 71 ⚠️ | 190 ⚠️ |
| 11 | `aljiwan.html` | Al Jiwan Jewellery - Code Crafter Project \| Bahrain | ~52 ✅ | ~155 ✅ |
| 12 | `MoSD.html` | Ministry of Social Development Bahrain - MoSD \| Code Crafter | ~62 ⚠️ | ~145 ✅ |
| 13 | `IINJAZ.html` | IINJAZ Project \| Code Crafter Portfolio Bahrain | ~49 ✅ | ~120 ⚠️ |
| 14 | `mmbrain.html` | MMBrain Project \| Code Crafter Portfolio Bahrain | ~50 ✅ | ~120 ⚠️ |
| 15 | `caravan.html` | The Booking Manager - Caravan \| Code Crafter Project Bahrain | ~61 ⚠️ | ~150 ✅ |
| 16 | `leen.html` | Leen Project \| Code Crafter Portfolio Bahrain | ~47 ✅ | ~100 ⚠️ |
| 17 | `jaryalshaikhmall.html` | Jaryal Shaikh Mall - Showcase Portfolio \| Code Crafter Bahrain | ~64 ⚠️ | ~138 ⚠️ |
| 18 | `filmzone.html` | Filmzone Project \| Code Crafter Portfolio Bahrain | ~51 ✅ | ~100 ⚠️ |
| 19 | `deepmark.html` | Deepmark Project \| Code Crafter Portfolio Bahrain | ~51 ✅ | ~100 ⚠️ |
| 20 | `magnify.html` | Magnify ERP System \| Code Crafter Project Bahrain | ~51 ✅ | ~140 ✅ |
| 21 | `mql4bot.html` | MQL4 Bot Project \| Code Crafter Portfolio Bahrain | ~51 ✅ | ~100 ⚠️ |

> **ملاحظة:** `shortcodes.html` صفحة داخلية للمكونات — لا يجب أن تُفهرسها محركات البحث.

---

### 1B. CSS & JS Files

**CSS (8 ملفات):**

| File | Used By |
|------|---------|
| `style.css` | جميع الصفحات (ملف رئيسي — يستورد الملفات الخمسة أدناه) |
| `css/all.min.css` | جميع الصفحات (Font Awesome ~100KB) |
| `css/home.css` | `index.html` فقط |
| `css/content.css` | عبر `@import` في `style.css` |
| `css/showcase.css` | عبر `@import` في `style.css` |
| `css/portfolio.css` | عبر `@import` في `style.css` |
| `css/shortcodes.css` | عبر `@import` في `style.css` |
| `css/assets.css` | عبر `@import` في `style.css` |

**JS (6 ملفات محلية + CDN):**

| File | Size | Notes |
|------|------|-------|
| `js/jquery.min.js` | 89 KB | جميع الصفحات |
| `js/plugins.js` | 330 KB | جميع الصفحات — حزمة ثقيلة |
| `js/clapatwebgl.js` | 3 KB | جميع الصفحات |
| `js/common.js` | 117 KB | جميع الصفحات |
| `js/scripts.js` | 71 KB | جميع الصفحات |
| `js/contact.js` | 6 KB | جميع الصفحات ما عدا صفحات الخدمات الأربع |

CDN: GSAP 3.10.4، ScrollMagic، Three.js r128، imagesloaded، Google Maps API

---

### 1C. خريطة التنقل (Navigation Map)

**Header — `index.html`:** Work → `showcase.html` | About → `about.html` | Contact → `contact.html`

**Header — جميع الصفحات الأخرى:** Showcase | About | Contact | Multimedia

**Footer (جميع الصفحات):** Back to top | © 2025 Code Crafter | LinkedIn | Instagram

> **⚠️ تناقض في التنقل:** الصفحة الرئيسية تحتوي على 3 عناصر ("Work") بينما جميع الصفحات الأخرى تحتوي على 4 عناصر ("Showcase" + "Multimedia"). يُربك المستخدم عند التنقل.

---

### 1D. روابط معطوبة وملفات مفقودة

| المشكلة | التفصيل |
|---------|---------|
| 🔴 `IINJAZ.html` يرتبط بـ `project05.html` | **الملف غير موجود** — رابط "المشروع التالي" معطوب |
| 🔴 `index.html` في JSON-LD يرجع إلى `services.html` | **الملف غير موجود** — خطأ في schema |
| 🟡 خلفية في `index.html` تشير إلى `images/MoSD-BG.jpg` | **الملف موجود في** `images/projects/MoSD-BG.jpg` — مسار خاطئ محتمل |

---

### 1E. الصور — ملفات كبيرة وغير محولة إلى WebP

**إجمالي الصور:** 192 ملف | **WebP:** ملف واحد فقط (`images/fx6.webp`) | **191 صورة ليست WebP**

أكبر الملفات (فوق 200KB — الكاملة):

| الحجم | الملف |
|-------|-------|
| 3,911 KB | `images/studio03.jpg` |
| 2,730 KB | `images/MMBrain-BG.png` |
| 2,607 KB | `images/studio04.jpg` |
| 2,479 KB | `images/about.jpg` |
| 2,431 KB | `images/studio02.jpg` |
| 2,417 KB | `images/shooq.JPG` |
| 1,980 KB | `images/projects/MMBrain-01.png` |
| 1,884 KB | `images/sh1.png` |
| 1,840 KB | `images/studio01.jpg` |
| 1,427 KB | `images/aljiwanjewellery3.png` |
| 1,383 KB | `images/aljiwanjewellery2.png` |
| + 50 ملفاً آخر بين 200KB و 1,400KB | |

> ⚠️ ملف `images/Thumbs.db` (222KB) — بقايا Windows، يجب حذفه قبل النشر.

---

## PART 2 — SEO Technical Check

### 2A. وسوم H1 لكل صفحة

| الصفحة | عدد H1 | نص H1 | المشكلة |
|--------|--------|-------|---------|
| `index.html` | 1 | "We Build / Digital Products." | ✅ |
| `about.html` | 1 | "Design / Inspire / Deliver" | ✅ |
| `contact.html` | 1 | "Hello / Friend!" | ✅ |
| `showcase.html` | **0** | لا يوجد | 🔴 **H1 مفقود** |
| `multimedia.html` | 1 | "Multimedia" | ✅ |
| `shortcodes.html` | **4** | عناوين ديكورية مكررة | 🟡 |
| `web-development-bahrain.html` | 1 | "Web Development Bahrain" | ✅ |
| `software-development-bahrain.html` | 1 | "Software Development Bahrain" | ✅ |
| `laravel-development-bahrain.html` | 1 | "Laravel Development Bahrain" | ✅ |
| `website-design-bahrain.html` | 1 | "Website Design Bahrain" | ✅ |
| 11 صفحة portfolio | 1 لكل | معظمها "Project Challenge" | 🟡 عام — لا كلمات مفتاحية |

---

### 2B. طول العنوان والوصف

| الصفحة | العنوان | الوصف |
|--------|---------|-------|
| `index.html` | 60 حرف ✅ | 190 حرف ⚠️ (زيادة 30) |
| `about.html` | 57 حرف ✅ | 253 حرف ⚠️ (زيادة 93) |
| `contact.html` | 59 حرف ✅ | 227 حرف ⚠️ (زيادة 67) |
| `showcase.html` | 63 حرف ⚠️ | 223 حرف ⚠️ |
| `multimedia.html` | 64 حرف ⚠️ | 204 حرف ⚠️ |
| `web-development-bahrain.html` | 67 حرف ⚠️ | 177 حرف ⚠️ |
| `software-development-bahrain.html` | 69 حرف ⚠️ | 162 حرف ⚠️ |
| `laravel-development-bahrain.html` | 64 حرف ⚠️ | 188 حرف ⚠️ |
| `website-design-bahrain.html` | 71 حرف ⚠️ | 190 حرف ⚠️ |

> **الخلاصة:** جميع الأوصاف تتجاوز 160 حرفاً — Google ستقطعها وتقلل نسبة النقر (CTR).

---

### 2C. البيانات المنظمة (JSON-LD Schema)

| الصفحة | Schema موجود | المفقود |
|--------|-------------|---------|
| `index.html` | `Organization` + `LocalBusiness` ✅ | رابط `hasOfferCatalog` معطوب |
| `about.html` | `BreadcrumbList` فقط | `Organization` أو `AboutPage` schema |
| `contact.html` | `BreadcrumbList` + `LocalBusiness` ✅ | — |
| `showcase.html` | `BreadcrumbList` فقط | `ItemList` / `CollectionPage` schema |
| `multimedia.html` | **لا يوجد** | على الأقل BreadcrumbList |
| `web-development-bahrain.html` | `Service` + `BreadcrumbList` ✅ | — |
| `software-development-bahrain.html` | `Service` + `BreadcrumbList` ✅ | — |
| `laravel-development-bahrain.html` | `Service` + `BreadcrumbList` ✅ | — |
| `website-design-bahrain.html` | `Service` + `BreadcrumbList` ✅ | — |
| 11 صفحة portfolio | **لا يوجد** | `CreativeWork` schema |

---

### 2D. sitemap.xml و robots.txt

كلا الملفين **موجودان ومضبوطان بشكل جيد**. Sitemap يحتوي على 20 URL.

**مشاكل موجودة:**
- `sitemap.xml` لا يحتوي على صفحتَي الخدمة المفقودتين اللتين يجب إنشاؤهما
- `sitemap.xml` يتضمن `shortcodes.html` — صفحة داخلية لا ينبغي لـ Google فهرستها
- `robots.txt` يحجب Ahrefs وSEMrush وMoz — هذا يعني عدم القدرة على تتبع الترتيب عبر هذه الأدوات

---

### 2E. صور بدون `alt` attributes

أكثر من 60 صورة عبر الموقع تفتقر إلى نص بديل:

| الصفحة | العدد التقريبي | التفاصيل |
|--------|---------------|---------|
| `showcase.html` | 22 | جميع thumbnails الـ portfolio بـ `alt=""` فارغ |
| `about.html` | 4 | صور carousel الاستديو |
| `multimedia.html` | 14 | صور الكولاج |
| `IINJAZ.html` | 6 | لقطات المشروع |
| `mmbrain.html` | 8 | صور carousel |
| `MoSD.html` | 4 | صور carousel |
| `leen.html` | 6 | صور المشروع |
| `magnify.html` | 8 | صور المصباح |
| `mql4bot.html` | 8 | صور fx |
| + 3 صفحات أخرى | متفرقة | |

---

### 2F. التوافق مع الجوال (Mobile)

جميع الصفحات الـ 21 تحتوي على `<meta name="viewport" content="width=device-width, initial-scale=1.0">` ✅

---

## PART 3 — Content Gap Analysis

### صفحات موجودة مقابل صفحات مطلوبة

| الصفحة | موجودة؟ | قيمة SEO |
|--------|---------|---------|
| الصفحة الرئيسية | ✅ | — |
| About | ✅ | — |
| Contact | ✅ | — |
| Portfolio / Showcase | ✅ (`showcase.html`) | — |
| Web Development Bahrain | ✅ | عالية |
| Website Design Bahrain | ✅ | عالية |
| Software Development Bahrain | ✅ | عالية |
| Laravel Development Bahrain | ✅ | متوسطة |
| **Mobile App Development Bahrain** | ❌ | **عالية جداً** |
| **E-commerce Development Bahrain** | ❌ | **عالية جداً** |
| **Blog / مقالات SEO** | ❌ | **عالية جداً** |
| **FAQ** | ❌ | متوسطة |
| **services.html** (صفحة فهرس الخدمات) | ❌ | متوسطة |

### الصفحات المفقودة ذات الأولوية

**1. `mobile-app-development-bahrain.html`**
كلمة "mobile app development Bahrain" ذات بحث مرتفع. غياب صفحة مخصصة = صفر فرصة للترتيب.

**2. `ecommerce-development-bahrain.html`**
التجارة الإلكترونية من أكثر الخدمات بحثاً في البحرين. مشروع Al Jiwan يثبت أنكم تبنونها — استثمروا ذلك.

**3. مدونة / Blog**
حالياً لا يوجد محتوى SEO. المنافسون الذين يتصدرون "web development Bahrain" كلهم لديهم مدونات نشطة.
مقترحات للمقالات:
- "كم تكلفة تصميم موقع في البحرين؟"
- "تصميم مواقع إلكترونية في البحرين — دليل 2026"
- "أفضل 10 أعمال تحتاج موقعاً إلكترونياً في البحرين"

**4. `faq.html`**
يستهدف خانة "People Also Ask" في نتائج Google (Featured Snippets).

**5. `services.html`**
مذكور في JSON-LD الصفحة الرئيسية لكن غير موجود — إما إنشاؤه أو إصلاح الـ schema.

---

## PART 4 — قائمة المهام بالأولويات

### 🔴 أولوية عالية — تأثير مباشر على الفهرسة والترتيب

| # | المهمة |
|---|--------|
| H1 | **إصلاح الرابط المعطوب** في `IINJAZ.html` → حذف أو استبدال رابط `project05.html` |
| H2 | **إضافة `<h1>` إلى `showcase.html`** — مثال: "Our Work — Selected Projects" |
| H3 | **إنشاء `mobile-app-development-bahrain.html`** بمحتوى كامل وفق نفس القالب |
| H4 | **إنشاء `ecommerce-development-bahrain.html`** بمحتوى كامل وفق نفس القالب |
| H5 | **تقليص جميع الأوصاف إلى 140–160 حرفاً** — جميع الصفحات الـ 9 الرئيسية تتجاوز الحد |
| H6 | **إصلاح JSON-LD في `index.html`** — تحديث أو حذف رابط `hasOfferCatalog` → `services.html` |
| H7 | **إضافة `alt` وصفي لجميع الصور المفقودة (~60 صورة)** مع `loading="lazy"` |
| H8 | **تحديث `sitemap.xml`** — إضافة الصفحتين الجديدتين، حذف `shortcodes.html` |

### 🟡 أولوية متوسطة — تحسين SEO ملموس

| # | المهمة |
|---|--------|
| M1 | **تقليص عناوين الصفحات إلى أقل من 60 حرفاً** — showcase وmultimedia والخدمات الأربع |
| M2 | **إضافة `Service` schema للصفحتين الجديدتين** |
| M3 | **إضافة `AboutPage` schema لـ `about.html`** |
| M4 | **إضافة `BreadcrumbList` + `CreativeWork` schema لـ 11 صفحة portfolio** |
| M5 | **إضافة `BreadcrumbList` schema لـ `multimedia.html`** |
| M6 | **تمييز H1 في صفحات Portfolio** — "Project Challenge" على 10 من 11 صفحة لا قيمة منه |
| M7 | **ضغط الصور وتحويلها إلى WebP** — ملفات studio01–04 وحدها = 12 MB |
| M8 | **إضافة روابط داخلية من الصفحة الرئيسية** للصفحتين الجديدتين |
| M9 | **توحيد قائمة التنقل** — الصفحة الرئيسية ("Work") مقابل باقي الصفحات ("Showcase"+"Multimedia") |
| M10 | **إضافة `noindex` لـ `shortcodes.html`** — صفحة داخلية |
| M11 | **إصلاح Google Analytics** — `ga('create', 'code_here', 'auto')` placeholder موجود على جميع الصفحات |

### 🟢 أولوية منخفضة — تحسينات طويلة المدى

| # | المهمة |
|---|--------|
| L1 | إنشاء **قسم Blog** (حتى صفحة هبوط ثابتة + 2–3 مقالات) |
| L2 | إنشاء **صفحة FAQ** (`faq.html`) |
| L3 | إنشاء **`services.html`** كفهرس لجميع الخدمات الست |
| L4 | **حذف `images/Thumbs.db`** |
| L5 | توحيد أسماء الملفات — `MoSD.html` و`IINJAZ.html` يجب أن تكون بأحرف صغيرة لأمان الخوادم |
| L6 | إضافة **`hreflang` tags** للمحتوى ثنائي اللغة (بعض الصفحات عربي، بعضها إنجليزي) |
| L7 | تأمين Google Maps API key (حالياً مضمّن مباشرة في HTML) |

---

## ملخص سريع

| المعيار | النتيجة |
|---------|---------|
| إجمالي صفحات HTML | 21 صفحة |
| صفحات الخدمات الموجودة | 4 من 6 |
| صفحات الخدمات المفقودة | 2 (Mobile App, E-commerce) |
| وسوم Title مناسبة (<60 حرف) | 3 من 9 ✅ |
| أوصاف Meta مناسبة (140–160 حرف) | 0 من 9 ❌ |
| صفحات بـ H1 صحيح | 19 من 21 ✅ |
| صفحات بـ JSON-LD schema | 6 من 10 رئيسية ✅ |
| sitemap.xml | موجود ✅ |
| robots.txt | موجود ✅ |
| صور بـ alt مفقود | ~60+ صورة ⚠️ |
| صور WebP | 1 من 192 ⚠️ |
| روابط معطوبة | 2 🔴 |

---

*تقرير أعده: Cursor AI Agent — June 9, 2026*
