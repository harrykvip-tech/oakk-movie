# OAK K Movies

Google Sheet ကနေ ဇာတ်ကားစာရင်းဖတ်တဲ့ ဇာတ်ကားကက်တလော။ **Web + App (APK) နှစ်မျိုးလုံး GitHub ကနေ အလိုအလျောက် ထုတ်ပေးပါတယ်။**

## ၁။ GitHub မှာ တင်ပါ
1. github.com မှာ repository အသစ်ဆောက်ပါ (ဥပမာ `oakk-movies`) – **Public**။
2. ဒီ folder ထဲက ဖိုင်အားလုံးကို upload လုပ်ပါ။ **`.github` folder ပါအောင်လည်း တင်ပါ** (Add file → Upload files ထဲကို folder ဆွဲထည့်ပါ)။

## ၂။ Web ဗားရှင်း (App မရတဲ့ ဖုန်းများအတွက်)
1. **Settings → Pages → Source** ကို **GitHub Actions** လို့ ရွေးပါ။
2. **Actions** tab မှာ *Deploy Web* ပြီးသွားရင် `https://<username>.github.io/oakk-movies/` မှာ ဖွင့်လို့ရပါပြီ။
3. ဒီလင့်ကို ဖုန်းမှာဖွင့်ပြီး –
   - **Android (Chrome):** ညာထိပ်က 📲 ခလုတ် (သို့) ⋮ → *Install app*
   - **iPhone (Safari):** Share → *Add to Home Screen*
   
   လုပ်ရင် Home Screen မှာ App အဖြစ် ထည့်သွင်းနိုင်ပါတယ်။

## ၃။ Android APK ထုတ်နည်း
1. **Actions → Build Android APK → Run workflow** ကိုနှိပ်ပါ (၅-၈ မိနစ်ကြာပါမယ်)။
2. ပြီးရင် run ထဲက **Artifacts → OAKK-Movies-APK** ကို download လုပ်ပါ (zip ဖြည်ရင် `OAKK-Movies.apk`)။
3. ဖုန်းမှာ APK ကို install လုပ်ပါ ("မသိသော source" ခွင့်ပြုရပါမယ်)။
- Release အဖြစ်ထုတ်ချင်ရင် tag `v1.0` လို့ push လုပ်ပါ – Releases မှာ APK တန်းပေါ်ပါမယ်။
- ဒါက debug APK ဖြစ်လို့ install လုပ်လို့ရပါတယ်။ Play Store တင်ချင်ရင် signed build လိုပါမယ်။

## Google Sheet
- **Anyone with the link → Viewer** ထားရပါမယ်။ `index.html` ထဲက `SHEET_URL` မှာ လင့်ပြောင်းလို့ရပါတယ်။
- ကော်လံ: `A` နာမည် · `B` ခုနှစ် · `C` Quality · `D` Poster URL · `E` အညွှန်း · `F` TeraBox လင့် · `G` ဖိုင်အရွယ်အစား · `H` Genre
- Genre မှာ `Action` / `Animation` / `Hollywood` / `popular` (သို့) `လူကြိုက်များ` ပါရင် အဲဒီ row တွေမှာ ပေါ်ပါမယ်။
- အောက်ဆုံးကြောင်း = အသစ်ဆုံး၊ အောက်ဆုံး ၅ ကားက ပင်မ banner မှာ auto ပြောင်းပြပါမယ်။
- APK ထဲက မျှဝေလင့် မှန်စေရန် `index.html` ထဲက `WEB_URL` မှာ သင့် GitHub Pages လင့်ကို ထည့်ပါ။
