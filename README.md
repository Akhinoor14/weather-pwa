# আবহাওয়া অ্যাপ

আইকনে চাপলেই Google-এর আবহাওয়া খোলে।

## ১. Vercel-এ আপলোড (ফ্রি)
1. vercel.com-এ লগইন করুন → Add New → Project
2. ZIP খুলে weather-pwa ফোল্ডারটি GitHub-এ আপলোড করে Import করুন
   (GitHub ছাড়া চাইলে: কম্পিউটারে `npx vercel` চালিয়ে ফোল্ডার থেকে ডিপ্লয় করা যায়)
3. Framework Preset: Other। Build Command ও Output Directory খালি রাখুন → Deploy
4. লিংক পাবেন, যেমন: your-name.vercel.app

## ২. আব্বুর ফোনে ইনস্টল
- ফোনে সেই লিংক খুলুন
- Android (Chrome): "ফোনে ইনস্টল করুন" বাটন চাপুন
- iPhone (Safari): Share → Add to Home Screen
- এরপর হোম স্ক্রিনের আইকনে চাপলেই আবহাওয়া খুলবে

## ৩. কিছু বদলাতে চাইলে
index.html-এর একদম নিচে ৩ লাইনের সেটিংস আছে:
- CITY = "" → ফোনের লোকেশন। "khulna" লিখলে খুলনা
- BANGLA = true → বাংলা রেজাল্ট
- WAIT_MS = 900 → স্প্ল্যাশ কতক্ষণ থাকবে

নাম বদলাতে: manifest.webmanifest-এর "name" ও "short_name", এবং index.html-এর <title>।

## ৪. আপডেট দিলে
ফাইল বদলে আবার push করলে Vercel নিজে ডিপ্লয় করবে। ফোনের অ্যাপ একবার বন্ধ করে খুললে নতুন ভার্সন আসবে।
