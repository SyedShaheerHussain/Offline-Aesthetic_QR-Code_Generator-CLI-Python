# 🌟 Universal QR Generator

**One-line Description:**

Create aesthetic, high-quality, static, animated, gradient, AI-themed, and transparent QR codes with logos, backgrounds, batch support, and offline/online AI integration.

**Developed by:** Syed Shaheer Hussain
**Copyright:** 2026

## 📷 Screenshot

![Screenshot](https://github.com/SyedShaheerHussain/Offline-Aesthetic_QR-Code_Generator-CLI-Python/blob/388c252b38ff32499a1cb44cd2442564135435ac/Offline-Aesthetic_QR-Code_Generator/screenshot/cli%20ss.png)

## 📱 Example QR CODES:

![Example 1](https://github.com/SyedShaheerHussain/Offline-Aesthetic_QR-Code_Generator-CLI-Python/blob/388c252b38ff32499a1cb44cd2442564135435ac/Offline-Aesthetic_QR-Code_Generator/animated.gif)

![Example 2](https://github.com/SyedShaheerHussain/Offline-Aesthetic_QR-Code_Generator-CLI-Python/blob/388c252b38ff32499a1cb44cd2442564135435ac/Offline-Aesthetic_QR-Code_Generator/google.svg)

![Example 2](https://github.com/SyedShaheerHussain/Offline-Aesthetic_QR-Code_Generator-CLI-Python/blob/388c252b38ff32499a1cb44cd2442564135435ac/Offline-Aesthetic_QR-Code_Generator/hq.png)

![Example 2](https://github.com/SyedShaheerHussain/Offline-Aesthetic_QR-Code_Generator-CLI-Python/blob/388c252b38ff32499a1cb44cd2442564135435ac/Offline-Aesthetic_QR-Code_Generator/insta.png)

![Example 2](https://github.com/SyedShaheerHussain/Offline-Aesthetic_QR-Code_Generator-CLI-Python/blob/388c252b38ff32499a1cb44cd2442564135435ac/Offline-Aesthetic_QR-Code_Generator/qr.png)

## 📚 1. Project Overview

**What is this project?**

A comprehensive QR code generator that allows users to create high-quality, aesthetic QR codes for any type of content—URLs, social media handles, phone numbers, emails, texts, and more. It supports offline generation, batch generation, AI-themed QR codes, animated gradients, transparency, SVG export, posters, and story templates.

**Mission / Objective:**

* Enable users to easily generate scannable, beautiful QR codes.
* Integrate AI-generated artistic enhancements for aesthetic appeal.
* Provide a safe, offline-first solution while also supporting online AI features.
* Help individuals and businesses create shareable QR codes for marketing, branding, and personal use.

**Why it was made:**

* QR codes are widely used but often look plain and unengaging.
* Trend of aesthetic, anime, or AI-generated QR art is increasing.
* Existing QR tools lack advanced offline and batch features, or AI aesthetics.

**Market value:**

* High usability for social media influencers, marketing campaigns, branding, and creative professionals.
* Shareable, visually appealing QR codes have higher scan rates.
* Can be monetized as a SaaS or desktop utility.

## ⚡ 2. Features & Functions

### 🔹 Core Features

1. **Static QR Codes:** High-quality QR codes for any type of content.
2. **Animated Gradient QR:** Multi-frame GIF QR codes with gradient animation.
3. **SVG Export:** Vector output for print and scalable designs.
4. **AI Themes:** Unique color schemes generated randomly or via AI.
5. **Gradient QR (Real Multi-Color):** QR codes with smooth color gradients.
6. **Transparent QR:** QR codes with transparent backgrounds for overlay purposes.
7. **Logo Embed:** Embed logos or icons at the center of QR codes.
8. **Background Image:** Blend QR with custom backgrounds.
9. **Batch QR Generator:** Generate multiple QR codes at once from a CSV file.
10. **Offline & Online AI Integration:**

    * Offline: Anime or aesthetic QR with center images.
    * Online: AI-stylized QR codes via APIs (like Replicate or HuggingFace).
11. **Poster & Story Templates:** Ready-to-share designs for social media.

### 🔹 Optional Features

* `--gradient`: Apply a gradient to the QR code.
* `--transparent`: Make the QR code background transparent.
* `--logo`: Add a logo to the center of QR code.
* `--background`: Blend QR with a custom background image.
* `-l / --label`: Add text below the QR code.
* `-o / --output`: Define output filename.

## 🛠 3. Technologies Used

* **Python 3.10+**: Core programming language.
* **Libraries:**

  * `qrcode` → QR code generation
  * `Pillow` → Image manipulation
  * `imageio` → Animated GIFs
  * `csv` → Batch generation
  * `requests` → Online AI API integration
* **Optional Online Tools:**

  * AI models (Replicate, ControlNet, HuggingFace, Stable Diffusion) for stylized QR codes.

## 🏛 4. Architecture & Flow

### 🔹 Folder Structure

```
Universal-QR-Generator/
├── qr.py                  # Main executable script
├── assets/                # Optional images like logos, backgrounds, anime
├── data/                  # CSV files for batch generation
├── output/                # Saved QR codes and posters
├── .env                   # Environment variables (API keys)
└── README.md

```

### 🔹 Flowchart (Simplified)

```
[User Input] --> [QR Type & Data] --> [Create Basic QR]
                                      |
                                      V
                          ----------------------
                          | Optional Features   |
                          | Gradient / Transparent
                          | Logo / Background
                          | Label / Size
                          ----------------------
                                      |
                                      V
                         [Offline QR or Online AI QR]
                                      |
                                      V
                         [Generate Poster / Story / GIF]
                                      |
                                      V
                               [Save Output]

```

## ⚙ 5. How It Works

1. User runs the script.
2. Wizard guides the user:

   * Select QR type (URL, Instagram, WhatsApp, text, email, etc.)
   * Choose theme, size, high-quality option, gradient, transparency
   * Optionally add logo, background, label
   * Specify output filename
3. Script generates QR based on selected features.
4. For batch mode: read CSV → generate multiple QR codes automatically.
5. For AI-styled QR (online):

   * Upload base QR → API → receive stylized QR → save locally.
6. Poster and story templates can be automatically generated for shareable social media content.

## 💻 6. Installation

### Prerequisites

* Python 3.10 or higher
* Git (optional, for cloning repository)
* Internet connection (for online AI features)

### Step-by-Step

1. Clone the repository:

```
git clone https://github.com/username/Universal-QR-Generator.git

```
```
cd Universal-QR-Generator

```

2. Install Python dependencies:

```
pip install qrcode[pil] pillow imageio requests python-dotenv

```

3. For AI features (online):

   * Create `.env` in root folder:

```
REPLICATE_API_TOKEN=your_token_here

```

* Sign up for [Replicate](https://replicate.com) or other AI service.

## 🏃 7. Running the Project

### 🔹 Wizard Mode (Interactive)

```
python qr.py

```

* Follow the prompts to choose type, theme, size, gradient, transparency, logos, backgrounds, labels, and output filename.
* Poster and story templates can also be generated.

### 🔹 Direct CLI / Advanced

```
python qr.py instagram username --gradient --transparent --logo logo.png --background bg.png -l "My Insta" -o output.png

```

### 🔹 Batch Mode

CSV example (`data.csv`):

```
instagram,user1,insta1
url,https://google.com,googleQR
text,Hello,helloQR

```

Command:

```
python qr.py --batch data/data.csv

```

## 📐 8. Use & Usage Examples

| Use Case | Command | Output |
| --- | --- | --- |
| Static QR | `python qr.py url https://google.com`                | qr.png |
| Gradient QR | `python qr.py instagram username --gradient`         | qr.png |
| Transparent QR | `python qr.py url https://example.com --transparent` | qr.png |
| Batch QR | `python qr.py --batch data.csv`                      | Multiple PNGs |
| Poster | Wizard Mode → create poster                          | poster.png |
| Story | Wizard Mode → create story | story.png |


## ⚡ 9. Advantages & Disadvantages

**Advantages**

* Fully customizable, offline-first
* Batch generation
* AI aesthetics support
* High quality, printable QR
* Supports social media marketing
* Transparent & gradient options
* Poster & story templates for sharing

**Disadvantages**

* Online AI features require internet & API keys
* Large AI-generated QR may take time
* Advanced features may require learning for full use

## 🛡 10. Safety & Security

* No sensitive data is stored unless user saves it.
* Batch CSV should not include passwords.
* QR should not redirect to unsafe sites.
* Always verify URLs before sharing.
* Safe offline generation reduces phishing risk.
* Online AI uses third-party services; do not upload confidential data.

## ⚠️ 11. Cautions & Important Notes

>[!caution]
> 1. Overwriting existing files will replace them without confirmation.
> 2. Large images may require higher memory.
> 3. AI API may have rate limits.
> 4. Test QR codes after generation before distribution.
> 5. Avoid using confidential information in public QR codes.

## 🔧 12. Programming Concepts & Architecture

* Procedural & modular Python design
* Image manipulation via Pillow
* CSV parsing for batch processing
* Command-line arguments for flexibility
* Optional wizard mode for beginners
* API integration for AI online QR generation

## 🧩 13. Future Enhancements

1. Offline AI-styled QR using ControlNet locally
2. Animated QR stickers & GIFs
3. GUI desktop app
4. Web-based SaaS platform
5. QR analytics / tracking for marketing
6. NFT-ready QR generation

## 📌 14. Technologies & Concepts Covered

* **Python Programming**
* **Image Processing** (Pillow)
* **QR Code Generation**
* **CLI Interfaces** (argparse)
* **Batch Processing**
* **Online API Integration**
* **AI Image Generation**
* **Design & Aesthetics**
* **Security & Phishing Awareness**

## 🔑 15. Learning & Achievements

By developing and using this project, one learns:

* Python programming & modular coding
* Image manipulation and design
* Automation with batch processing
* Integrating AI APIs
* UX-focused design for CLI tools
* Security and phishing awareness
* Creative application of QR codes in marketing

## 🌐 16. How to Host / Run in Browser / Online

* For web-based deployment, wrap the Python code in Flask / FastAPI and host on services like:

  * Heroku
  * Render
  * Railway
* Use `.env` for API keys
* Add login if needed for SaaS version

## 🏷 17. Tags / Keywords

QR Code, QR Generator, AI QR, Gradient QR, Animated QR, Poster, Story, Batch QR, Transparent QR, Logo QR, Social Media, Marketing, Offline QR, Safe QR, Python CLI, Replicate API, Aesthetic QR, Anime QR, Visual QR

## 🧠 18. How This Project Helps Users Avoid Phishing & Harm

* Generate QR codes offline → no third-party data exposure
* Transparent / gradient QR → visually confirm authenticity
* Batch CSV → only user data is included
* Always preview QR → prevent redirection to unsafe links
* Can include labels for content type
* Optional AI → visually inspect QR before sharing

## ✅ 19. Summary

The **Universal QR Generator PRO v5** is a professional, multifunctional tool:

* ✅ Offline & Online hybrid
* ✅ High-quality QR generation
* ✅ Gradient, transparent, logo, background support
* ✅ Batch & poster generation
* ✅ AI aesthetic integration
* ✅ Safe, customizable, shareable

It is **installation-ready**, fully functional, beginner-friendly, and future-proof for advanced QR design projects.

## ⭐ Support & Engagement

If you find this repository useful or insightful, please consider:

- ⭐ Starring the repository
- 🔁 Sharing it within your network
- 👤 Following my GitHub profile for future projects and updates

Your support helps drive continued innovation and open-source contributions.

— Syed Shaheer Hussain

[![GitHub followers](https://img.shields.io/github/followers/SyedShaheerHussain?label=Follow&style=social)](https://github.com/SyedShaheerHussain)

![Followers](https://img.shields.io/github/followers/SyedShaheerHussain?label=Followers&color=blue)

![Stars](https://img.shields.io/github/stars/SyedShaheerHussain/Offline-Aesthetic_QR-Code_Generator-CLI-Python?label=Stars&color=yellow)

>[!note]
> Developed by: **Syed Shaheer Hussain**
> **Copyright 2026 ©**
