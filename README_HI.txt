MERA HISAB PRO — ANDROID SOURCE PROJECT

Is ZIP mein Android app ka poora source code hai. Yeh ready-made APK nahi hai.
APK banane ke do tareeqe:

TAREEQA A — GitHub Actions se APK banayein (Android phone se bhi)
1. ZIP extract karein.
2. GitHub par naya repository banayein: mera-hisab-pro-android
3. Is ZIP ke ANDAR ki saari files/folders repository ke root mein upload karein.
   Dhyan: settings.gradle.kts, build.gradle.kts, app folder aur .github folder
   repository ke root par hone chahiye.
4. Commit/push karein.
5. GitHub repository mein Actions tab kholein. "Build Android APK" workflow run hona chahiye.
6. Workflow complete hone par run kholein aur Artifacts mein "MeraHisabPro-debug-apk"
   download karein. ZIP artifact ke andar app-debug.apk milega.
7. APK apne Android phone par download karke install karein. Android "Install unknown apps"
   permission pooch sakta hai; sirf apni banayi hui APK ko install karein.

TAREEQA B — Android Studio
1. Project ko computer par extract karein.
2. Android Studio mein is folder ko Open karein.
3. JDK 17 use karein, Gradle sync hone dein.
4. Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Debug APK app/build/outputs/apk/debug/app-debug.apk mein milegi.

APP FEATURES
- Income aur expense entries
- Udhaar lena/dena, pending/paid
- Customer-wise history
- Search, filters, edit/delete
- Reports, print/PDF intent
- JSON backup / CSV export (WebView bridge)
- Offline local storage; data isi device par rehta hai

IMPORTANT
- Google login/cloud sync is version mein nahi hai.
- Data local device par hai. App uninstall ya app data clear karne se data mit sakta hai.
  Regular backup karein.
- Yeh debug APK personal testing ke liye hai; Play Store release ke liye signing aur
  extra testing chahiye.
