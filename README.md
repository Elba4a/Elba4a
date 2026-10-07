## Islam Soliman

Software engineer in Cairo. I build every layer of a product myself: the mobile app, the
web front end, the Postgres schema, the Edge Functions, and the container the whole thing
ships in.

**[elba4a.com](https://elba4a.com)** has the work on one page, including eight screens of
Hekta you can click through. Most of the code itself is in private repos because it holds
client data and pricing, so here is what is behind them.

### What I'm building

**Hekta**: a money app for Egypt and the Gulf. It covers daily spending, net worth with gold
counted in karats and grams, and shared expenses, all through one AI input layer. You type
it, say it, or scan the receipt, and nothing saves until you confirm it.
1,300+ commits · 43 Postgres tables with RLS on every one · 15 Edge Functions ·
7,000+ client and edge tests.
**[On the App Store](https://apps.apple.com/app/id6778138657)** · [hekta.money](https://hekta.money)
`Expo · React Native · TypeScript · Supabase · Claude API`

**Muhrah**: a handmade mastic bukhoor brand I own, in Cairo. A Shopify storefront, a full
design system, and a WhatsApp bot that answers in Egyptian Arabic and closes the order in
Shopify. The project has one external dependency; everything else is the Node standard library.
**[muhrah.shop](https://muhrah.shop)**
`Shopify · Claude tool use · node:sqlite · WhatsApp Cloud API`

**Wehdtak**: a platform for real-estate brokerage offices in Egypt. Each office keeps its own
units and clients, shares the ones it chooses on a common market, and closes deals with other
offices. The platform keeps the record and never touches the money. In development.
[wehdtak.com](https://wehdtak.com)
`Next.js · Supabase · Railway`

**Horus Transfer**: fixed-price airport transfers in Egypt, in 14 languages, confirmed over
WhatsApp. Search only ever offers destinations the operator has actually priced.
`Next.js · next-intl · PostgreSQL`

**[NOOR](https://github.com/Elba4a/noor-eg)**: a bilingual landing page for an Egyptian
finishing contractor. No build step, no dependencies, one CSS file. The gold only appears
where the light lands, because `#C9A24D` measures 7.9:1 on the dark surface and 2.4:1 on
white. **[noor-eg.net](https://noor-eg.net)**
`Static HTML/CSS · Caddy · Railway`

### Open source

**[karat-gold](https://github.com/Elba4a/karat-gold)**: gold weight and value in karats and
grams, 24K down to 10K. I pulled it out of Hekta because no library does it.
MIT · 10 tests · zero dependencies

**[arabic-type-rn](https://github.com/Elba4a/arabic-type-rn)**: type styling for React Native
where Arabic fonts must load by PostScript name per weight and `letterSpacing` has to be
zeroed, because negative tracking breaks the joins between letters.
MIT · 12 tests · zero dependencies

### How I build

- **I audit my own work before anyone else gets to.** A pre-launch pass over Hekta turned
  up five problems the documentation already claimed were finished. All five were closed
  before the app went to the store.
- **Domain rules the libraries don't have.** Gold is counted in karats and grams, never ounces.
  Every entry is locked to its exchange rate on the day it was made, so last year's numbers
  are never rewritten.
- **Decisions get measured, not guessed.** Contrast ratios, bundle sizes, and a real
  `expo export` beat an assumption every time.
- **Secrets stay on the server.** Every sensitive call runs from an Edge Function, and
  nothing sensitive ships in a client bundle.

### Stack

`TypeScript` `React Native / Expo` `Next.js` `React` `Node.js`
`PostgreSQL / PLpgSQL` `Supabase` `Deno` `Claude API` `Shopify Liquid`
`Railway` `Cloudflare` `Docker` `Caddy`
`Jest` `Deno test` `Maestro`

---

<div dir="rtl">

## إسلام سليمان

مهندس برمجيات في القاهرة. بابني كل طبقة في المنتج بنفسي: تطبيق الموبايل، والويب،
وسكيما Postgres، والـ Edge Functions، والكونتينر اللي المنتج كله بيتشحن فيه.

الشغل كله في صفحة واحدة على [elba4a.com](https://elba4a.com). أغلب الكود في ريبوهات
private (فيها داتا عملاء وأسعار)، فده اللي وراها:

- **Hekta**: تطبيق فلوس لمصر والخليج. فيه المصاريف اليومية، وصافي الثروة بالذهب بالجرام والعيار،
  والمصاريف المشتركة، وكلهم من طبقة إدخال واحدة بالـ AI: تكتبها أو تقولها أو تصوّر الإيصال.
  +١٣٠٠ commit · ٤٣ جدول عليهم RLS · ١٥ Edge Function · +٧٠٠٠ اختبار.
  *[على App Store](https://apps.apple.com/app/id6778138657)* · [hekta.money](https://hekta.money)
- **مُهرة**: براند بخور مستكة يدوي **بملكه**، في القاهرة. فيه متجر Shopify وبوت واتساب
  بيرد بالعامية المصرية ويقفل الأوردر. [muhrah.shop](https://muhrah.shop)
- **Wehdtak**: منصة لمكاتب السمسرة العقارية في مصر. كل مكتب بيدير وحداته وعملاءه، ويعرض
  اللي يختاره منهم في سوق مشترك، ويقفل صفقات مع مكاتب تانية. لسه بيتبني. [wehdtak.com](https://wehdtak.com)
- **Horus Transfer**: حجز مواصلات بسعر ثابت في مصر، بـ١٤ لغة، والتأكيد على واتساب.
- **NOOR**: لاندنج بيدج لشركة تشطيبات مصرية، من غير build ومن غير ولا dependency.
  [noor-eg.net](https://noor-eg.net)

</div>
