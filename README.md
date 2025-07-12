# Capy Typer Adventure

Capy Typer Adventure is a lightweight, single-page typing game for kids inspired by the classic *Mario Teaches Typing*.  
Guide a cute capybara, collect seeds, stomp bad-guys, and level-up your keyboard skills!

---

## 🎮  Gameplay

| Key            | Action                            |
| -------------- | --------------------------------- |
| **Letter / Symbol** | Type the label on the nearest seed or enemy |
| **ESC**        | Pause / resume                    |

Objectives:

1. Type the characters shown on seeds to *eat* them for points.  
2. Type the full label on enemies to *stomp* them.  
3. Clear all seeds in a level to advance.  
4. Maintain combos for bonus score — but they decay after 1.5 s of inactivity.  
5. You have 5 hearts; collisions or missed seeds cost health.

---

## ✨  Features

- 22 progressive keyboard levels (letters → numbers → symbols).
- Randomised backgrounds, particle effects, combo system.
- Real-time speed scaling: correct keys **+10 %** speed, mistakes **−5 %**.
- One-target-at-a-time design keeps focus for younger players.
- Company branding row with clickable Teddy Kids & TISA logos.
- LocalStorage save-data (unlocked levels, stats, high scores).
- Single self-contained HTML (< 80 kB) — no frameworks, no backend.

---

## 🛠️  Tech Stack

* HTML5 Canvas + vanilla JS  
* Tailwind-free custom CSS (pixel-style)  
* Sound via Web Audio API (inline)  
* LocalStorage for persistence

---

## 🚀 Local Setup

```bash
git clone https://github.com/<your-org>/capy-typer-adventure.git
cd capy-typer-adventure
# Static file — open directly or via small server
python3 -m http.server 8080
# Visit http://localhost:8080
```

---

## 🌐 Deployment (Vercel + TransIP)

1. **GitHub**

   ```bash
   git init
   git add .
   git commit -m "Initial game"
   git remote add origin https://github.com/<your-org>/capy-typer-adventure.git
   git push -u origin main
   ```

2. **Vercel**

   • Sign in at https://vercel.com with GitHub.  
   • *Import Project* → pick the repo.  
   • **Framework**: “Static HTML”. Build & output commands: *leave blank*.  
   • Deploy → you get `https://capy-typer-adventure.vercel.app`.

3. **Custom Domain**

   In Vercel → *Settings › Domains* → add `cappy.teddykids.nl`.  
   In TransIP DNS create **CNAME** record:

   ```
   Name:  cappy
   Value: cname.vercel-dns.com.
   TTL:   300
   ```

   DNS propagates in minutes.  
   Now play at **https://cappy.teddykids.nl**.  
   Optionally add a path-based redirect `teddykids.nl/cappy` → sub-domain from your main CMS.

---

## 📊  Folder Structure

```
capy-typer-adventure/
├── index.html      # identical to capy-typer-adventure.html
├── vercel.json     # (optional) static config
└── README.md
```

_No node modules, no build step._  

---

## 🤝  Credits

Made with ❤️ by Teddy Kids & TISA.  
Game code by the Teddy Kids dev team with help from Factory.ai.

---

## 📄  License

MIT — free to play, learn, and modify. Please retain copyright notice.
