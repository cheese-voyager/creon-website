
<div align="center">

# 🤖 CREON Website

### Creative Robotics Engineers of ITENAS

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS_v2-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://v2.tailwindcss.com/)
[![Alpine.js](https://img.shields.io/badge/Alpine.js_v2-8BC0D0?style=for-the-badge&logo=alpine.js&logoColor=black)](https://alpinejs.dev/)
[![AOS](https://img.shields.io/badge/AOS-Animate_On_Scroll-blueviolet?style=for-the-badge)](https://michalsnik.github.io/aos/)

The official website for CREON (Creative Robotics Engineers of ITENAS),
a robotics research and engineering forum based at Institut Teknologi Nasional (ITENAS) Bandung, Indonesia.

[🌐 Live Site](#) · [📋 KRTI Page](#) · [👥 Team Page](#)

</div>

---

## 📖 About

CREON merupakan wadah bagi mahasiswa ITENAS untuk berinovasi dan berprestasi di bidang robotika. Organisasi ini terlibat aktif dalam riset dan pengembangan teknologi melalui tiga divisi utama: **KRAI** (Kontes Robot ABU Indonesia), **KRTI** (Kontes Robot Terbang Indonesia), dan **KKI** (Kompetisi Kendaraan Impian). Dengan tim yang kompeten dan semangat inovasi yang tinggi, CREON berkomitmen menjadi pusat akademik robotika terdepan serta berkontribusi terhadap kemajuan teknologi nasional.

> CREON is a forum for ITENAS students to innovate and excel in the field of robotics. Actively involved in research and development of technology through its divisions: KRAI, KRTI, and KKI. With a competent team and a high spirit of innovation, CREON is committed to becoming a leading center for academic robotics and contributing to the advancement of national technology.

---

## ✨ Features

### 🏠 Landing Page (`index.html`)

- Hero section with animated floating UI elements and particle effects
- CREON organization overview with responsive typography
- Division showcase cards for KRAI, KRTI, and KKI (KKI currently as "Coming Soon")
- Footer with social media links (Instagram, YouTube)
- ITENAS institutional branding

### 🚁 KRTI Division Page (`krti.html`)

- Full-screen hero banner with parallax overlay and particle animations
- S-Curve layout showcasing the AERO-GUARD drone project and team divisions
- Interactive drone photo gallery with hover overlays and captions
- Competition timeline with animated milestones (Preliminary, Technical, Flight Test, Final)
- Progress documentation photo grid from KRTI 2026 preparation
- Social media footer with dedicated AEROTENS contacts (Instagram, TikTok, Website)

### 👥 Team Directory (`team.html`)

- Dark-themed immersive layout with floating glassmorphism orbs
- Gradient text effects and glow animations
- 27+ team members organized by 5 departments:
  - 💻 Informatika - Software and Administration
  - ⚙️ Teknik Mesin - Mechanical Engineering
  - ⚡ Teknik Elektro - Electrical Engineering
  - 🎨 Desain Produk - Product Design
  - 🖌️ Desain Komunikasi Visual - Visual Communication Design
- Advisor and Project Manager highlighted cards with role badges
- Member cards with avatar fallback system (initials when photos unavailable)

---

## 🏗️ Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| HTML5 | 5 | Semantic page structure and content |
| Tailwind CSS | v2 (CDN) | Utility-first responsive styling and layout |
| Alpine.js | v2 (CDN) | Lightweight reactive UI interactions |
| AOS | Latest (CDN) | Scroll-triggered animations |
| Google Fonts | Poppins | Typography (weights 400 to 900) |
| Custom CSS | creon.css | Glassmorphism, floating orbs, S-curve, gradient effects |

All dependencies load from CDN. Zero build tools and zero npm install required.

---

## 📁 Project Structure

```
creon-website/
├── index.html                          # Landing page (CREON main)
├── krti.html                           # KRTI division page (AERO-GUARD)
├── team.html                           # Team directory (dark theme)
├── css/
│   └── creon.css                       # Custom animations and effects
├── img/
│   ├── robot.png                       # Hero illustration
│   ├── KRAI.jpg                        # KRAI division card image
│   ├── Rectangle 19.png                # KKI division card image
│   ├── Rectangle 21.png                # KRTI division card image
│   ├── company/                        # Institutional logos (ITENAS)
│   └── krti/
│       ├── progress/
│       │   └── krti2026/               # 52 high-res progress photos
│       └── team/                       # Team member photos (name.png)
├── PROPOSAL KRTI AEROTENS.docx         # Project proposal document
├── Presentasi Dekan.docx               # Dean presentation
├── Progress AEROTENS KRTI 2026.pptx    # Progress presentation slides
└── README.md
```

---

## 🚀 Getting Started

No build tools, package managers, or server-side runtimes are required. You only need a modern web browser and optionally a local web server.

### Option 1: Laragon (Recommended)

1. Clone the repository into your Laragon `www` directory:

```bash
cd C:\laragon\www
git clone https://github.com/your-username/creon-website.git
```

2. Start Laragon and enable Apache.
3. Open your browser and navigate to `http://localhost/creon-website/`

### Option 2: VS Code Live Server

1. Clone the repository:

```bash
git clone https://github.com/your-username/creon-website.git
cd creon-website
```

2. Open the folder in VS Code.
3. Install the **Live Server** extension by Ritwick Dey.
4. Right-click `index.html` and select **Open with Live Server**.

### Option 3: Python HTTP Server

```bash
cd creon-website
python -m http.server 8000
```

Then visit `http://localhost:8000/` in your browser.

---

## 🖼️ Adding Team Photos

The team page (`team.html`) uses an automatic avatar fallback system. When a team member photo file is not found, the page shows stylized initials instead.

To add actual photos, place `.png` files in the `img/krti/team/` directory:

```
img/krti/team/
├── lisa.png          # Dr. sc. Lisa Kristiana (Advisor)
├── aria.png          # Aria Krisna Putra (Project Manager)
├── aliya.png         # Aliya Marwa Kamila
├── shafira.png       # Shafira Kurnia Fasya
├── zakhwa.png        # Zakhwa Aliya Maryam
├── fathan.png        # Fathan Kairu Ilham
├── ryan.png          # Ryan Febrianto
├── budi.png          # Budi Kurnia
├── aga.png           # Aga Fahim Zaydan Taqi
├── ridoane.png       # Muhammad Ridoane Zildjiana
├── saepul.png        # Saepul Anwarudin
├── ikhwan.png        # Muhamad Ikhwan Syakir
├── firly.png         # El Firly Faranro
├── aryo.png          # Aryo Tri Alfikri
├── alvin.png         # Alvin Nurdin
├── hary.png          # Hary Indra Permana
├── rianie.png        # Rianie Mukti Handayani
├── ilham.png         # Muhammad Ilham Gimnasty Sianipar
├── ihsan.png         # Ihsan Rijal Pratama
├── rhaya.png         # Rhaya Prayoga
├── rifqi.png         # Muhammad Rifqi Sardono
├── rizkhan.png       # Muhammad Rizkhan
├── abimanyu.png      # Muhammad Abimanyu
├── dea.png           # Dea Humaira
├── fania.png         # Fania Khairani Dewi
├── vina.png          # Vina Putri Pratama
├── dzaky.png         # Muhammad Dzaky Albukhori
└── faza.png          # Muhammad Faza Salman
```

**Photo Guidelines:**

- Format: PNG (transparent background preferred)
- Aspect ratio: 1:1 (square crop)
- Minimum resolution: 200x200px
- Maximum file size: 500KB per photo

---

## 🎨 Custom CSS Components

The `css/creon.css` file provides reusable design components:

| Component | Description |
|---|---|
| `.krti-hero` | Full-screen hero with background image and gradient overlay |
| `.s-curve-box` | Glassmorphism card for S-curve sections |
| `.drone-gallery` | CSS Grid photo gallery with hover overlays |
| `.team-page-bg` | Dark radial gradient background |
| `.orb` | Animated floating gradient spheres |
| `.glass-dark` | Dark glassmorphism card with backdrop blur |
| `.member-card` | Team member card with department-colored borders |
| `.member-avatar` | Circular avatar with gradient border ring |
| `.gradient-text` | Text with gradient fills |
| `.glow-text` | Text with glow shadow effects |
| `.back-to-top` | Fixed scroll-to-top button |
| `.timeline-*` | Competition timeline with connected dots |

---

## 📱 Responsiveness

The website is fully responsive across all device sizes:

| Breakpoint | Tailwind Class | Behavior |
|---|---|---|
| < 640px | default | Single column, stacked layout, compact nav |
| 640px+ | sm | Two-column grids, expanded spacing |
| 768px+ | md | Multi-column layouts, side-by-side content |
| 1024px+ | lg | Full desktop layout, S-curve visible |
| 1280px+ | xl | Max-width container, 5-column team grids |

---

## 🔗 Pages and Navigation

| Page | Route | Status |
|---|---|---|
| Landing | `index.html` | ✅ Complete |
| KRTI Division | `krti.html` | ✅ Complete |
| Team Directory | `team.html` | ✅ Complete (photos pending) |
| KKI Division | `#` | 🔜 Coming Soon |
| KRAI Division | `#` | 🔜 Planned |

---

## 🤝 Contributing

Contributions from CREON members and collaborators are welcome!

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "feat: add your feature description"`
4. Push to your branch: `git push origin feature/your-feature-name`
5. Open a Pull Request with a clear description of your changes

### Commit Convention

| Prefix | Usage |
|---|---|
| `feat:` | New feature or page |
| `fix:` | Bug fix |
| `style:` | CSS/UI changes (no logic change) |
| `docs:` | Documentation updates |
| `refactor:` | Code restructuring |
| `assets:` | Adding or updating images and media |

---

## 📄 License

This project is maintained by **CREON ITENAS** for internal and academic purposes.

All drone photography and team assets are property of **AEROTENS** (Aeronautica Team of Engineering Itenas).

---

<div align="center">

**Built with 💛 by CREON ITENAS**

*Crafting the Future, One Robot at a Time*

[![Instagram](https://img.shields.io/badge/@creon__itenas-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/creon_itenas/)
[![YouTube](https://img.shields.io/badge/@CREON-FF0000?style=flat-square&logo=youtube&logoColor=white)](https://www.youtube.com/@CREON-p6z)
[![Instagram](https://img.shields.io/badge/@aerotens.itenas-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/aerotens.itenas/)

© 2026 CREON - Institut Teknologi Nasional Bandung

</div>