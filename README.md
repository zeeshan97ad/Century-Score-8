# Century Score

Offline score tracker app. GitHub Actions isse Android APK banata hai.

## APK kaise milega
1. Repo ke root par ye files hon: `.github/`, `www/`, `package.json`, `capacitor.config.json`.
2. Code `main` branch par push karein.
3. **Actions** tab -> *Build APK* (ya "Run workflow").
4. Run khatam hone par neeche **Artifacts -> century-score-apk** download karein, zip kholein, `app-debug.apk` install karein.

## Manual build
```
npm install
npx cap add android
npx cap sync android
cd android && ./gradlew assembleDebug
```
APK: `android/app/build/outputs/apk/debug/app-debug.apk`
