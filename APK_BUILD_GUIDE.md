# 🚀 بناء APK - تطبيق واجد

هذا المستودع يحتوي على كل ما تحتاج لبناء APK من التطبيق!

## 📦 المتطلبات:

1. **Java Development Kit (JDK 11+)**
   - حمّل من: https://www.oracle.com/java/technologies/downloads/

2. **Android SDK**
   - حمّل Android Studio من: https://developer.android.com/studio

3. **Gradle**
   - يأتي مع Android Studio تلقائياً

---

## 🛠️ خطوات البناء:

### **الطريقة 1: استخدام Android Studio (الأسهل)**

```bash
1. فتح Android Studio
2. File → New → Import Project
3. اختر مجلد المستودع
4. انتظر حتى ينتهي Gradle من التهيئة
5. Build → Build Bundle(s)/APK(s) → Build APK(s)
6. انتظر حتى ينتهي البناء
7. APK بيكون في: app/build/outputs/apk/release/app-release.apk
```

### **الطريقة 2: استخدام Terminal**

```bash
# Windows
gradlew.bat build

# macOS/Linux
chmod +x gradlew
./gradlew build
```

---

## 📱 تثبيت APK على الهاتف:

### **الطريقة 1: عبر USB**

```bash
# وصّل الهاتف بالـ USB
# فعّل "Developer Mode" في الهاتف

# من Terminal:
adb install app/build/outputs/apk/release/app-release.apk
```

### **الطريقة 2: نقل مباشر**

```
1. انسخ ملف APK من المجلد أعلاه
2. انقله للهاتف عبر USB أو Bluetooth
3. افتح الملف من مدير الملفات
4. اضغط "تثبيت"
5. ✅ خلاص!
```

---

## 📁 هيكل المشروع:

```
Multi-Use-App/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/wajid/app/
│   │       ├── res/
│   │       ├── assets/
│   │       │   ├── index.html
│   │       │   ├── app.js
│   │       │   ├── manifest.json
│   │       │   └── sw.js
│   │       └── AndroidManifest.xml
│   └── build.gradle
├── build.gradle
├── settings.gradle
└── gradlew
```

---

## 🔧 إصلاح المشاكل الشائعة:

### ❌ **"Gradle not found"**
- ثبّت Gradle من: https://gradle.org/install/
- أو استخدم Android Studio

### ❌ **"Java not found"**
- ثبّت JDK من: https://www.oracle.com/java/technologies/downloads/

### ❌ **"Android SDK not found"**
- ثبّت Android Studio
- شغّل SDK Manager من داخل Android Studio

---

## 📥 تحميل APK جاهز:

**إذا ما بتبي تبني الـ APK بنفسك:**

حمّل من الإصدارات (Releases):
```
https://github.com/mouadzeyoun-spec/Multi-Use-App/releases
```

---

## ✅ بعد التثبيت:

- التطبيق يعمل **بدون إنترنت** (معظم الميزات)
- جميع البيانات محفوظة **محلياً** على الهاتف
- **آمن تماماً** - لا توجد بيانات شخصية

---

**أي سؤال؟ استفسر في Issues!** 🚀
