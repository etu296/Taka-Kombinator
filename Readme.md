# ভাংতি Kombinator 💵

A single-page web app that helps users in Bangladesh exchange their ৳500 or ৳1000 taka notes into the best possible combination of smaller denominations (৳200, ৳100, ৳50, ৳20, ৳10) — instantly and smartly.

---

## 📸 Preview

![App Flowchart](flowchart.png)

---

## ✨ Features

- **Real Bangladeshi Taka Note Images** — All 6 denominations (৳10 to ৳500) displayed with authentic note photos throughout the app
- **Two Exchange Modes:**
  - 🤖 **Auto Mode** — System automatically calculates the optimal note combination using a greedy algorithm
  - ✋ **Manual Mode** — User selects exactly how many of each denomination they want, with live total tracking and overflow protection
- **Step-by-step Flow** — Guided 4-step process matching the original system design flowchart
- **৳10 Service Fee** — Transparently deducted before combination calculation
- **Input Validation** — Only accepts ৳500 or ৳1000 taka notes
- **Fully Offline** — All note images are embedded as base64; no external assets needed
- **Bilingual UI** — Bengali + English throughout
- **Responsive Design** — Works on both desktop and mobile

---

## 🗺️ System Design / Flowchart

The app was built directly from this system design diagram:

![System Flowchart](flowchart.png)

The flow covers:
1. User indicates they need ভাংতি (change)
2. User submits a ৳500 or ৳1000 note → validated
3. User confirms the ৳10 service charge
4. User chooses Auto or Manual combination mode
5. Final combination is previewed and confirmed
6. Success screen shows the full breakdown

---

## 🚀 Getting Started

No installation, no dependencies. Just open the HTML file.

```bash
# Clone the repo
git clone https://github.com/your-username/vangti-kombinator.git

# Open in browser
open taka_kombinator_v2.html
```

Or simply **download** `taka_kombinator_v2.html` and open it in any modern browser.

---

## 🏗️ How It Works

### Auto Mode Algorithm
The system uses a **greedy denomination breakdown** — it fills the amount with the largest available notes first, working down through ৳200 → ৳100 → ৳50 → ৳20 → ৳10.

```
Input:  ৳500 note
Fee:    ৳10
Net:    ৳490

Auto breakdown:
  ৳200 × 2 = ৳400
  ৳50  × 1 = ৳50
  ৳20  × 2 = ৳40
  ──────────────
  Total    = ৳490 ✓
```

### Manual Mode
User picks quantities with `+` / `−` controls. The app tracks the running total in real time and prevents the user from exceeding the net amount.

---

## 🪙 Supported Denominations

| Note | Name | Featured Landmark |
|------|------|-------------------|
| ৳500 | পাঁচশত টাকা | কেন্দ্রীয় শহীদ মিনার, ঢাকা |
| ৳200 | দুইশত টাকা | অপরাজেয় বাংলা, ঢাকা বিশ্ববিদ্যালয় |
| ৳100 | একশত টাকা | ষাট গম্বুজ মসজিদ, বাগেরহাট |
| ৳50  | পঞ্চাশ টাকা | আহসান মঞ্জিল, ঢাকা |
| ৳20  | বিশ টাকা | কান্তজির মন্দির, দিনাজপুর |
| ৳10  | দশ টাকা | Ten Taka (2026 Series) |

---

## 📁 Project Structure

```
vangti-kombinator/
├── taka_kombinator_v2.html   # Main app (all-in-one, self-contained)
├── flowchart.jpg             # System design diagram
└── README.md                 # This file
```

---

## 🛠️ Built With

- Pure **HTML5 / CSS3 / Vanilla JavaScript** — zero frameworks, zero dependencies
- **Google Fonts** — Playfair Display, Noto Sans Bengali, DM Mono, Instrument Serif
- **Base64 embedded images** — all 7 note photos baked directly into the HTML

---

## 🤝 Contributing

Pull requests are welcome! If you'd like to suggest improvements:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author - Etu Mahmuda Era

Made with ❤️ in Bangladesh.

> *"No more ভোগান্তি — Enjoy your hassle-free ভাংতি!"*