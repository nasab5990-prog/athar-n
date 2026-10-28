# تحويل أثَر إلى تطبيق أندرويد / iOS باستخدام Capacitor

## المتطلبات
- Node.js مثبت
- Android Studio (لأندرويد)
- Xcode (لـ iOS - على ماك فقط)

## الخطوات
1. انسخ الملفات إلى مجلد المشروع:
   - index.html
   - manifest.json
   - sw.js
   - capacitor.config.json

2. في المجلد نفّذ:
```bash
npm init -y
npm install @capacitor/core @capacitor/cli @capacitor/android
npx cap init "أثَر" "om.edu.athar.ai" --web-dir .
npx cap add android
npx cap sync
npx cap open android
```

3. في Android Studio:
   - Build → Build Bundle(s) / APK(s) → Build APK
   - ستجد ملف APK في مجلد android/app/build/outputs

## ملاحظات
- التطبيق سيعمل كتطبيق حقيقي على أندرويد.
- يمكنك لاحقًا إضافة ميزات أصلية (إشعارات، كاميرا...).
- للمسابقة: الـ PWA + رابط الويب كافيان، والتطبيق الأصلي خطوة إضافية.
