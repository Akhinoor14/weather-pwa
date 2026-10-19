# আবহাওয়া অ্যাপ (v5)

ফোনের আসল লোকেশনে বাংলায় আবহাওয়া দেখায়। অ্যাপ খুললেই তাপমাত্রা, বৃষ্টির সম্ভাবনা, ঘণ্টা অনুযায়ী ও ৭ দিনের পূর্বাভাস।
নিচে "Google-এ দেখুন" বাটন আছে, চাইলে Google-এর সাথে মিলিয়ে দেখা যায়।

## ১. Vercel-এ আপলোড (ফ্রি)
1. vercel.com-এ লগইন করুন → Add New → Project
2. weather-pwa ফোল্ডারটি GitHub-এ আপলোড করে Import করুন
3. Framework Preset: Other। Build Command ও Output Directory খালি রাখুন → Deploy
4. লিংক পাবেন, যেমন: your-name.vercel.app

## ২. আব্বুর ফোনে ইনস্টল
- ফোনে লিংক খুলুন। প্রথমবার ফোন লোকেশনের অনুমতি চাইবে, "Allow" চাপুন
- Android (Chrome): পেজের নিচের "ফোনে ইনস্টল করুন" বাটন
- iPhone (Safari): Share → Add to Home Screen
- এরপর হোম স্ক্রিনের আইকনে চাপলেই আবহাওয়া

## ৩. সেটিংস
index.html-এর নিচের দিকে LAT ও LON আছে। ফাঁকা থাকলে ফোনের লোকেশন ব্যবহার হয়।
কোনো নির্দিষ্ট জায়গা ঠিক করতে চাইলে লিখুন, যেমন খুলনা: LAT = 22.8456, LON = 89.5403

## ৪. নাম বদলাতে
manifest.webmanifest-এর "name" ও "short_name", এবং index.html-এর <title>।

## তথ্যের উৎস
Open-Meteo (ফ্রি, কোনো চাবি লাগে না)। জায়গার নাম: BigDataCloud (ফ্রি)।
