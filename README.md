## Islam Soliman

Communication engineer. I build products end to end — mobile, web, backend, and the
infrastructure under them. Arabic-first, RTL designed in from day one rather than
translated in later.

Most of my work is in private repos (client data and pricing), so here is what is
actually behind them.

### What I'm building

**[Hekta](https://github.com/Elba4a/Hekta)** — a personal financial operating system for
the Arab world. Daily money tracking, net worth with karat-aware gold, and shared
expenses, all fused under one AI input layer: type it, say it, or scan the receipt.
762 commits · 33 Postgres tables with RLS on every one · 14 Edge Functions ·
1,345 client + 361 edge tests. *Pre-submission, v1.0.0.*
`Expo · React Native · TypeScript · Supabase · Claude API`

**[NOOR](https://github.com/Elba4a/noor-eg)** — a bilingual landing page for an Egyptian
construction company. Zero build step, zero dependencies, one CSS file, one JS file.
The gold only appears where the light lands, because `#C9A24D` measures 7.9:1 on the
dark surface and 2.4:1 on white. **[noor-eg.net](https://noor-eg.net)**
`Static HTML/CSS · Caddy · Railway`

**Muhrah** — a handmade mastic bukhoor brand I own, in Cairo. Shopify storefront, full
design system, and a WhatsApp bot that answers in Egyptian Arabic and closes the order
in Shopify. One external dependency; everything else is the Node standard library.
The model proposes a `variant_id` — **the price is read from Shopify at order time,
never from the model.** **[muhrah.shop](https://muhrah.shop)**
`Shopify · Claude tool use · node:sqlite · WhatsApp Cloud API`

**Horus Transfer** — fixed-price airport transfers in Egypt, in 14 languages, confirmed
over WhatsApp. Search only ever offers destinations the operator has actually priced.
`Next.js · next-intl · PostgreSQL`

### How I work

- **The model never invents a number.** Prices come from the source of truth at request
  time; model output goes through hand-written parsers that return `null` on any
  violation — and that `null` is what triggers the retry on a stronger model.
- **API keys never reach the client.** Every LLM call runs server-side.
- **Arabic is not a translation layer.** Native RTL, Arabic fonts loaded by PostScript
  name per weight, Arabic copy written in Arabic.
- **Decisions get measured, not guessed.** Contrast ratios, bundle sizes, and a real
  `expo export` beat an assumption every time.

### Stack

`TypeScript` `React Native / Expo` `Next.js` `React` `Node.js`
`PostgreSQL / PLpgSQL` `Supabase` `Deno` `Claude API` `Shopify Liquid`
`Railway` `Vercel` `Cloudflare` `Docker` `Caddy`
`Jest` `Deno test` `Maestro`

---

<div dir="rtl">

## إسلام سليمان

مهندس اتصالات. بابني منتجات من أولها لآخرها — موبايل وويب وباك-إند والبنية اللي تحتيهم.
**عربي أولًا** — الـ RTL متصمّم من اليوم الأول مش مترجم بعدين.

أغلب شغلي في ريبوهات private (فيها داتا عملاء وأسعار)، فده اللي وراها بالظبط:

- **Hekta** — نظام مالي شخصي للعالم العربي. مصاريف يومية، وصافي ثروة بذهب واعي بالقيراط،
  ومصاريف مشتركة — كلهم تحت طبقة إدخال واحدة بالـ AI: اكتبها أو قولها أو صوّر الإيصال.
  ٧٦٢ commit · ٣٣ جدول عليهم RLS · ١٤ Edge Function · ١٧٠٦ اختبار. *قبل التقديم، v1.0.0.*
- **NOOR** — لاندنج بيدج لشركة تشطيبات مصرية. صفر build وصفر dependency.
  [noor-eg.net](https://noor-eg.net)
- **مُهرة** — براند بخور مستكة يدوي **بملكه**، في القاهرة. متجر Shopify وبوت واتساب
  بيرد بالعامية ويقفل الأوردر. **الموديل ما بيقدرش يخترع سعر** — السعر بيتقرا من
  Shopify لحظة الأوردر. [muhrah.shop](https://muhrah.shop)
- **Horus Transfer** — حجز مواصلات بسعر ثابت في مصر، بـ١٤ لغة، تأكيد على واتساب.

</div>
