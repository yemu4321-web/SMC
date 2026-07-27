# SMC Forex ትምህርት (Smart Money Concepts በአማርኛ)

ይህ ፕሮጀክት Smart Money Concepts (SMC) ን ለ Forex ገበያ በአማርኛ የሚያስተምር ድህረ ገጽ ነው። የተሰራው በ
[Horizon UI](https://github.com/horizon-ui) (Next.js + Tailwind CSS) ቴምፕሌት ላይ በመመስረት ነው።

## ተጨምረው የገቡ ገፅታዎች

- **`/`** — የ SMC / Forex ትምህርት ማስተዋወቂያ ላንዲንግ ገጽ (አማርኛ)
- **`/admin/default`** — የተማሪ ዳሽቦርድ: አጠቃላይ እድገት %, የተጠናቀቁ ትምህርቶች, ቀጣይ ትምህርት
- **`/admin/lessons`** — 8ቱ የ SMC ትምህርቶች ዝርዝር (የገበያ መዋቅር, BOS/CHoCH, Liquidity, Order
  Blocks, Fair Value Gap, Premium/Discount, Risk Management, ወዘተ)
- **`/admin/lessons/[slug]`** — እያንዳንዱ ትምህርት ገጽ + "እንደተጠናቀቀ ምልክት አድርግ" የሚል ቁልፍ
- እድገት (progress) የሚቀመጠው በተጠቃሚው አሳሽ `localStorage` ውስጥ ነው (ያለ ሰርቨር/ዳታቤዝ) —
  ስለዚህ በዚህ መሳሪያ/አሳሽ ላይ ብቻ ይቆያል።

ትምህርታዊ ይዘቱ የሚገኘው በ `src/variables/lessons.ts` ውስጥ ነው፤ አዲስ ትምህርት ለመጨመር ወደዚያ
ፋይል ብቻ አንድ object መጨመር በቂ ነው።

> ማሳሰቢያ፡ ይህ ትምህርታዊ ይዘት ብቻ ነው፤ የፋይናንስ ምክር አይደለም። ግብይት ከፍተኛ ኪሳራ ሊያስከትል ይችላል።

## በኮምፒውተርዎ ላይ ለማስኬድ

```bash
npm install
npm run dev
```

ከዚያ http://localhost:3000 ይክፈቱ።

## ወደ GitHub ለመስቀል

1. በ https://github.com/new ላይ አዲስ ባዶ ሪፖዚቶሪ ይፍጠሩ (README/license አይጨምሩ)።
2. በዚህ ፎልደር ውስጥ የሚከተሉትን ትዕዛዞች ያስኪዱ፡

```bash
git init
git add .
git commit -m "SMC Forex ትምህርት ድህረ ገጽ"
git branch -M main
git remote add origin https://github.com/<የእርስዎ-username>/<repo-name>.git
git push -u origin main
```

3. ለቀጥታ (live) ማስተናገጃ [Vercel](https://vercel.com) ን ይመከራል፤ የ GitHub ሪፖዎን ብቻ
   ያገናኙ፣ Vercel ራሱ Next.js መሆኑን ስለሚያውቅ ራሱ ይገነባል/ያስተናግዳል።

## ቴክኖሎጂ

Next.js (App Router) • React • TypeScript • Tailwind CSS
