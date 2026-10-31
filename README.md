# Ahmed Mazen Website — Firebase Spark version

واجهة عربية للرسائل المجهولة واختبار من 8 أسئلة، تعمل مع Firebase Authentication وCloud Firestore على خطة Spark.

## الملفات
- `index.html`: الموقع.
- `firestore.rules`: قواعد Firestore التي تتحقق من درجة الاختبار دون كشف مفتاح الإجابات للزائر.

## إعداد Firebase
1. فعّل Email/Password في Authentication.
2. أنشئ Firestore Database.
3. افتح Firestore > Rules، استبدل القواعد بالكامل بمحتوى `firestore.rules` ثم اضغط Publish.
4. ارفع `index.html` إلى استضافة HTTPS ثابتة.

ملاحظة: آلية التحقق من الدرجة تستخدم قواعد Firestore وتسمح بمحاولات تحقق محدودة من 0 إلى 8، ولا تحتاج Cloud Functions. اختبر الموقع بحسابين تجريبيين قبل مشاركة الرابط علنًا.
