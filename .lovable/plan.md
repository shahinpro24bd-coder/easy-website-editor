# Vercel asset ও inline admin editor fix

## কী বদলাবে
- About এবং homepage-এর About ছবিটি প্রকল্পের নিজস্ব public image file থেকে দেখানো হবে, যাতে Vercel-এ Lovable-only asset URL-এর ওপর নির্ভর না করে।
- Font Awesome ও Bootstrap icon font files public folder-এ রাখা হবে এবং icon stylesheet-কে সেই local files ব্যবহার করানো হবে।
- Admin preview-তে প্রতিটি editable text নিজ জায়গায় হালকা textbox outline হিসেবে দেখা যাবে।
- Text-এ click করলে একই জায়গায় সরাসরি লেখা edit হবে; আলাদা popup, textarea বা input খুলবে না।
- Link/button text edit করার সময় navigation বন্ধ থাকবে; image editing আগের মতো click-to-replace থাকবে।

## যাচাই
- About ও homepage-এ ছবির request এবং rendering যাচাই করা হবে।
- কয়েক ধরনের site icon-এর local font loading যাচাই করা হবে।
- Admin-এ login করে inline text edit, save, এবং public-page persistence যাচাই করা হবে।
- Desktop ও mobile view এবং final build status যাচাই করা হবে।

## সীমা
- বর্তমান browser-only save system অপরিবর্তিত থাকবে; edit অন্য browser/device-এ sync হবে না।
