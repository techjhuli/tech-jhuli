# Tech Jhuli — Product Website

## GitHub Pages এ হোস্ট করার নিয়ম

1. GitHub এ একটা নতুন repository তৈরি করুন (যেমন: `tech-jhuli`)
2. এই ফোল্ডারের সব ফাইল (index.html + images ফোল্ডার) repository তে আপলোড করুন
   - ফাইলগুলোর গঠন এমন থাকতে হবে:
     ```
     index.html
     images/
       Awei_PA92_power_bank.jpg
       Jysuper_2218_Fan.jpg
       ... (বাকি ছবিগুলো)
     ```
3. GitHub repository তে যান → **Settings** → **Pages**
4. **Branch** সেকশনে `main` সিলেক্ট করুন এবং **Save** চাপুন
5. কিছুক্ষণ পর আপনার সাইট লাইভ হয়ে যাবে এই লিংকে:
   `https://<আপনার-ইউজারনেম>.github.io/tech-jhuli/`

## নতুন প্রোডাক্ট যোগ করবেন যেভাবে

`index.html` ফাইলের ভিতরে `const products = [...]` অংশে একটা নতুন অবজেক্ট যোগ করুন, এভাবে:

```js
{
  id: 10,
  name: "প্রোডাক্টের নাম",
  price: 1000,
  category: "ক্যাটাগরির নাম",
  catKey: "fan",   // fan / powerbank / light / toy / ups — অথবা নতুন ক্যাটাগরি হলে categories লিস্টেও যোগ করুন
  image: "images/your-image.jpg",
  tagline: "এক লাইনে সংক্ষিপ্ত বিবরণ",
  warranty: "৬ মাস ওয়ারেন্টি",
  features: [
    "ফিচার ১",
    "ফিচার ২"
  ]
}
```

ছবিটি `images/` ফোল্ডারে রাখতে ভুলবেন না।

## যোগাযোগ বাটন ঠিক করুন

`index.html` এ "অর্ডার করতে যোগাযোগ করুন" এবং ফুটার অংশে আপনার WhatsApp/Facebook পেজের লিংক বসিয়ে দিতে পারবেন।
