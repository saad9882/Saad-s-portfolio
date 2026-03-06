# Saad's-portfolio
Rana Saad Ullah Khan — Portfolio

Personal portfolio website for **Rana Saad Ullah Khan** — _Full Stack Developer, Video Editor, and Content Creator_ based in Rawalpindi, Pakistan.


Live Demo
Deploy on Vercel by dragging portfolio.html into vercel.com/new — it goes live in under a minute on the free plan.

What's Inside
A single portfolio.html file. No frameworks, no build tools, no installs. Everything runs in the browser.
Tech used:

Pure HTML + CSS + Vanilla JavaScript
GSAP 3 — all animations and transitions
Google Fonts — Unbounded, Outfit, Syncopate
Cloudinary — live bike photo gallery (free tier)


Features
Splash Screen
Cinematic game-style boot sequence. HUD corner brackets, scanline overlay, name slams in letter by letter, chromatic aberration glitch effect (red/blue ghost layers), and a progress counter that runs to 100.
Hero
Full-screen motorcycle background with your name in two layers — RANA SAAD filled solid lime with chromatic split shadow, ULLAH KHAN as a hollow outline. Four round pill buttons open popup modals. No scrolling — everything is one page.
Modals (Popups)
All content lives inside blur-backdrop modals:
ButtonWhat's InsideAboutYour photo placeholder + bio + 4 info cards + personality pillsWorkInteractive card deck — 5 project cards that fly off like a real deckSkillsBlockchain, Backend, Languages, Frontend/Mobile, CreativeContactEmail (selectable/copyable) + LinkedIn, Instagram, YouTube cards
Card Deck (Work)
Cards stack on top of each other like a real physical pile with slight rotation. Click the top card or hit → and it flies off to the right revealing the one underneath. ← brings it back. Wedding invitation cards include live demo links.
Biker Gallery
iPhone Photos-style 2×2 button under the social icons. Opens a full gallery modal. Upload photos directly from your phone — they save to Cloudinary and appear live worldwide instantly. Tap any photo to open a lightbox.
Constellation Button
Fixed in the bottom right corner. Click it → fullscreen dark overlay → stars appear one by one → dashed lines connect them forming a real constellation (Orion, Cassiopeia, or Ursa Major, picked randomly) → name fades in → disappears in ~3–4 seconds. Tied to the CelestialLens AR project theme.
Other Details

All text is uncopyable (user-select: none) except the email address in Contact
Film grain overlay across the entire site
Proper SVG brand logos for LinkedIn, Instagram, YouTube
Responsive — works on mobile


Projects Showcased

Hyperledger Blockchain (Go) — Distributed ledger with Hyperledger Fabric. Marked In Progress / Coming Soon.
CelestialLens — Real-time AR constellation explorer for Android. Final Year Project.
Digital Wedding Invitations — Interactive online invites. Live samples: Walima · Shendi
Academic Assistance — Assignments, thesis, case studies, dissertations.
Freelance Full Stack — 3+ years, clients from scratch to launch.


Setup: Cloudinary Gallery
The live photo gallery uses Cloudinary's free tier with unsigned uploads. Before the upload button works, do this once:

Go to cloudinary.com and sign in
Navigate to Settings → Upload → Upload Presets
Click Add upload preset
Set the name to exactly: portfolio_bikes
Set Signing Mode to Unsigned
Set Folder to bikes
Hit Save

That's it. Photos uploaded from the portfolio will be tagged saad_bikes and appear in the gallery publicly worldwide.
Your Cloudinary details (already in the code):
Cloud Name:    day04dkda
Upload Preset: portfolio_bikes
Gallery Tag:   saad_bikes

Adding Your Photo
In the About modal there's a placeholder where your photo goes. To swap it in, find this comment in portfolio.html:
html<!-- Replace the <div class="ph">...</div> with: -->
<img src="YOUR_PHOTO_URL" alt="Rana Saad Ullah Khan" />
You can use a direct image URL, a Cloudinary link, or a local path if self-hosting.

Deploying on Vercel (Free)

Go to vercel.com and sign in with GitHub
Click Add New → Project
Drag and drop portfolio.html or push it to a GitHub repo and import it
Vercel detects it as a static site automatically
Hit Deploy — you get a live *.vercel.app URL

To use a custom domain, add it in Project Settings → Domains.

Customisation Cheatsheet
What to changeWhere to find itYour photoab-photo-frame div in About modalBackground image.hero-bg and .sp-bg CSS background URLsProject descriptionscardData array in the <script> tagWedding invite linkslinks array inside cardData[2]Social linkshref attributes on .soc-btn and .c-soc-card elementsEmail addressTwo places: c-email anchor tag and mailto: linksColor scheme:root CSS variables at the top of <style>Cloudinary cloud nameCLOUD_NAME constant in <script>

Color Scheme
css--lime:    #c8ff00   /* Electric chartreuse — primary accent */
--orange:  #ff3c00   /* Burning orange — hover / glitch */
--bg:      #050505   /* Near black background */
--surface: #0c0c0c   /* Modal / card backgrounds */
--white:   #f5f5f0   /* Off-white text */
--muted:   #404040   /* Secondary text, labels */

Fonts
FontWeightUsed ForUnbounded900Name, modal titles, card titlesOutfit300–700Body text, buttons, descriptionsSyncopate400, 700Labels, tags, HUD text

Contact
Rana Saad Ullah Khan

Email: ranasaad988@gmail.com
