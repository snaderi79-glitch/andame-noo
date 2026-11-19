# اندام نو
اپ تک‌فایلی فارسی (تاریخ شمسی). اجرا: فایل index.html را باز کنید.
## انتشار روی GitHub Pages
1. ریپو جدید بسازید و `index.html` را آپلود کنید.
2. Settings ← Pages ← Branch: main / root ← Save.
3. آدرس `https://USERNAME.github.io/REPO` آماده است (روی موبایل: Add to Home Screen).

## فونت بی‌زر
فایل فونت را با نام `BZar.woff2` (یا `.woff`/`.ttf`) در پوشه `fonts/` قرار دهید.

## راه‌اندازی Firebase (ورود و Ban واقعی)
1. https://console.firebase.google.com → پروژه جدید (پلن Spark رایگان).
2. Build → **Authentication** → Sign-in method → **Email/Password** را فعال کنید.
3. Authentication → Settings → **Authorized domains** → `USERNAME.github.io` را اضافه کنید.
4. Build → **Firestore Database** → Create (حالت production).
5. تب **Rules** → محتوای `firestore.rules` را بچسبانید → Publish.
6. Project settings → Your apps → Web (`</>`) → مقادیر را در `firebase-config.js` بگذارید.
7. در سایت ثبت‌نام کنید، سپس در Firestore → Authentication، **UID** حساب خود را کپی کنید و در Firestore یک collection با نام `admins` بسازید و Document ID را همان UID بگذارید (فیلد دلخواه، مثلاً `ok: true`). حالا تب «مدیریت» دارید.
8. همه فایل‌ها را روی GitHub آپلود کنید.
