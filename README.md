# قلم — Qalam (Android)

تطبيق نوتات بالقلم: الواجهة كلها في `app/src/main/assets/www/index.html`، والجزء ده بيشغّلها كتطبيق أندرويد
(تخزين على الجهاز، ميكروفون لتسجيل المحاضرات، حفظ الملفات في Download/Qalam، وقراءة بالصوت).

## الطريقة ١: Android Studio على اللابتوب
1. افتح Android Studio ← **Open** ← اختار فولدر `qalam-android`.
2. استنى لحد ما الـ Gradle sync يخلص (أول مرة بينزّل الأدوات من Google).
3. **Build ▸ Build App Bundle(s) / APK(s) ▸ Build APK(s)**.
4. الملف هيبقى في `app/build/outputs/apk/debug/app-debug.apk` — ابعته لموبايلك وثبّته
   (هيطلب منك تسمح بالتثبيت من مصادر غير معروفة).

## الطريقة ٢: GitHub يبنيه لك (من غير برامج)
1. اعمل repository جديد (يفضّل Private) وارفع محتويات الفولدر ده كلها، ومعاها فولدر `.github`.
2. GitHub Actions هيبني التطبيق لوحده في حوالي ٥ دقايق.
3. من صفحة **Releases** في الـ repository، نزّل `Qalam.apk` من الموبايل وثبّته.

## Option 1: Android Studio
Open this folder, wait for Gradle sync, then Build ▸ Build APK(s). The APK is in `app/build/outputs/apk/debug/`.

## Option 2: GitHub Actions
Push this folder (including `.github`) to a new repository. The workflow builds `Qalam.apk` and attaches it to a Release.
