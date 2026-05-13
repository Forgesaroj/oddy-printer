# Oddy Sticker Printer

> 🇳🇵 **If you've ever wasted 3 sticker sheets fighting Microsoft Word
> over a 2mm margin, this tool is for you.**

**👉 Open it now: https://forgesaroj.github.io/oddy-printer/**

Free. Browser-based. All 21 Oddy A4 SKUs pre-configured.
No install. No signup. No cost. Works offline once loaded.
Made in Nepal for the MRP labelling system that every shop now needs.

![Tool screenshot](https://img.shields.io/badge/status-live-success) ![Made in Nepal](https://img.shields.io/badge/made%20in-Nepal%20%F0%9F%87%B3%F0%9F%87%B5-red) ![License](https://img.shields.io/badge/license-MIT-blue) ![No signup](https://img.shields.io/badge/signup-not%20required-brightgreen)

---

## The problem this solves

**As of April 28, 2026, the Nepal Government has made printed MRP
(Maximum Retail Price) labels compulsory on every product sold in
the country** — under the Consumer Protection Act 2019, Section 6(3).
Customs offices in Birgunj, Bhairahawa, Biratnagar, Rasuwagadhi,
Nepalgunj and Kakarbhitta started stopping shipments without MRP
stickers, stranding over 1,000 containers at border points within
days of the rule taking effect. Writing prices by hand with a marker
is no longer legally acceptable.

So now every shopkeeper, every retailer, every small business in
Nepal is suddenly facing the same headache:

- You buy a packet of Oddy stickers — **ST-24, ST-33, ST-48, ST-65**, whichever
- You open MS Word and hunt for "Avery L7159" or "33 labels per sheet"
- You guess at margins. You print a test page. Labels are 2mm off.
- You waste 3 sheets (₹500–1000 down the drain). You try again.
- Eventually you give up and tell your supplier to print them somehow.

This is happening **every single day** in shops across the country —
and the printed-label requirement isn't going away.

This tool fixes it. **Pick your Oddy code → type your content → print.**
The exact margins and pitches from the official Oddy spec sheet are
already baked in for all 21 SKUs.

## What you can do with it

- 📋 Print **MRP labels** with shop name, MRP price, mfg date, item code
- 🏷️ Print **price tags** for retail shelves
- 📦 Print **address / return labels** for parcels & couriers
- 🗂️ Print **file labels** for offices and lawyers
- 📊 Print **barcode labels** (Code-128, EAN-13 — paste your generated image)
- 🛍️ Print **product stickers** with different content on each label,
  all on the same sheet (e.g. 33 different prices on one ST-33 sheet)

## Features

- ✅ Every Oddy A4 SKU pre-configured with the **exact margins, pitches, and
  label sizes** from the official Oddy "Dimensions Identification Table"
- ✅ **Free-write** content (one text block per label) or **structured**
  labels (name / address / phone / ref / date / footer)
- ✅ **Save named content presets** in your browser — type once, reuse forever
- ✅ **Print queue** — put different content on different labels of the same
  sheet (e.g. 11 return-address + 22 price tags on one ST-33 sheet)
- ✅ **Live preview** updates as you type, with zoom and page navigation
- ✅ **Typography controls** — font, size sliders, weight, italic, underline,
  uppercase, line height, auto-shrink-to-fit
- ✅ **CSV bulk fill** — paste a spreadsheet column and fill 84 different
  labels in one click
- ✅ **Works offline** once the page has loaded once
- ✅ **No tracking, no analytics, no servers** — everything runs in your browser

---

## Supported Oddy SKUs

All values from the official Oddy A4 Multipurpose Labels spec sheet.

| Code           | Labels | Grid  | Size (mm)        | Word ref     |
|----------------|-------:|-------|------------------|--------------|
| ST-1 A4100     |      1 | 1×1   | 199.6 × 289      | L-7167       |
| ST-2 A4100     |      2 | 1×2   | 199.6 × 143.6    | L-7168       |
| ST-4 A4100     |      4 | 2×2   |  99.1 × 139      | L-7169       |
| ST-6 A4100     |      6 | 2×3   |  99.1 × 93.4     | L-7166       |
| ST-6S A4100    |      6 | 2×3   |  90  × 80        | —            |
| ST-8 A4100     |      8 | 2×4   |  99.1 × 67.7     | L-7165       |
| ST-10 A4100    |     10 | 2×5   |  99.1 × 57       | L-7173       |
| ST-12 A4100    |     12 | 2×6   | 100   × 44.15    | —            |
| ST-14 A4100    |     14 | 2×7   |  99.06 × 38.4    | L-7163       |
| ST-16 A4100    |     16 | 2×8   |  99.1 × 33.9     | L-7162       |
| ST-18 A4100    |     18 | 3×6   |  63.5 × 46.6     | L-7161       |
| ST-20 A4100    |     20 | 2×10  |  98   × 28       | —            |
| ST-21 A4100    |     21 | 3×7   |  63.5 × 38.1     | L-7160       |
| ST-24 A4100    |     24 | 3×8   |  64   × 34       | L-7159       |
| ST-30 A4100    |     30 | 5×6   |  39   × 47.5     | —            |
| **ST-33 A4100**|     33 | 3×11  |  66   × 25.4     | —            |
| ST-40 A4100    |     40 | 4×10  |  52.5 × 29.7     | Z-Weck 3651  |
| ST-48 A4100    |     48 | 4×12  |  45.7 × 21.1     | —            |
| ST-56 A4100    |     56 | 4×14  |  50   × 20.1     | —            |
| ST-65 A4100    |     65 | 5×13  |  38.1 × 21.2     | L-7651       |
| ST-84 A4100    |     84 | 4×21  |  46   × 11       | L-7656       |

---

## How to print

1. Open the [tool](https://forgesaroj.github.io/oddy-printer/) in your browser
2. Pick your Oddy SKU from the dropdown
3. Enter content (or load a saved preset / CSV file)
4. Click **Generate full sheet →**
5. Press **🖨 Print** (or Ctrl+P) and choose:
   - **Paper:** A4
   - **Margins:** None (Chrome) / Default (Firefox)
   - **Scale:** 100% — uncheck "Fit to page"
   - **Background graphics:** ON if you want guides visible

**First-time calibration:** print one sheet on plain paper first.
Overlay it on a real Oddy sheet against a window — text blocks should
sit inside each adhesive die-cut. If labels are 1–2 mm off, adjust the
print dialog "Custom scale" by 0.5–1% increments, or set printer offset
in your printer driver.

---

## CSV bulk fill

Load a CSV from the form to fill many labels at once. One CSV row per
label. Column order:

```
free-write:    title, body
structured:    title, name, address, phone, ref, date, footer
```

Header row optional (auto-detected).

---

## Privacy

Everything runs **in your browser**. Saved content presets are stored
in your browser's `localStorage` only — never sent anywhere. No
analytics, no tracking, no servers. You can export / import the library
as JSON to move it between machines.

---

## Share this with a shopkeeper

If you know someone in Nepal who runs a shop, a clinic, a courier
service, or any small business that prints labels — **send them this
link**. They'll save hours every month and stop wasting sticker
sheets.

> साथीहरूलाई share गर्नुहोस् 🙏
> कुनै नेपाली व्यापारी, shopkeeper, clinic, courier सेवा,
> ​ साना-ठूला सबै businesses को लागि — free मा हुन्छ।

🔗 **https://forgesaroj.github.io/oddy-printer/**

---

## Made by

**Saroj Rijal** · [Sahara Labs](https://github.com/Forgesaroj) · 🇳🇵 Nepal
Made with ❤️ for everyone, forever free.

Released under the [MIT License](LICENSE) — free to use, fork, and modify.

Issues, feature requests, and contributions welcome on
[GitHub](https://github.com/Forgesaroj/oddy-printer/issues).

If this tool saved you time, you can support the project by:
- ⭐ Starring the repo on GitHub
- 📢 Sharing it with one other shopkeeper
- 💬 Opening an issue if you find a SKU that needs tweaking
