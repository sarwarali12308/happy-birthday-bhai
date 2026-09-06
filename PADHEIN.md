# Happy Birthday Website — Instructions (اردو + English)

## Folder Structure
```
bday-site/
├── index.html          ← main website file
├── images/
│   ├── brother.jpg      ← bhai ki main photo (circle frame me dikhegi)
│   ├── pin1.jpg
│   ├── pin2.jpg
│   ├── pin3.jpg
│   └── pin4.jpg
└── videos/
    ├── video1.mp4
    ├── video2.mp4
    ├── video3.mp4
    └── video4.mp4
```

## Apni photo/video/pins kaise add karein

1. **Main photo** (upar wali circle photo): apni file ko `images/brother.jpg` naam se rakhein — ya `index.html` file me search karein `brother.jpg` aur apni file ka naam likh dein.
2. **4 Videos**: apni 4 videos ko `videos/video1.mp4`, `video2.mp4`, `video3.mp4`, `video4.mp4` naam de dein aur `videos/` folder me daal dein.
3. **4 Pins (photos)**: apni 4 photos ko `images/pin1.jpg`, `pin2.jpg`, `pin3.jpg`, `pin4.jpg` naam de kar `images/` folder me daal dein.
4. Agar file ka naam/format alag rakhna hai (jaise `.png` ya `.mov`), to `index.html` me jahan `src="images/pin1.jpg"` ya `src="videos/video1.mp4"` likha hai, wahan apna naam likh dein.

## Bhai ka naam add karna
`index.html` me yeh line dhoondein:
```html
<p class="brother-name">میری جانو کے پیارے بھائی کے نام</p>
```
Yahan apne bhai ka naam add kar sakte hain, jaise:
```html
<p class="brother-name">Happy Birthday, [Naam] ✦</p>
```

## Vercel par Deploy kaise karein

**Option 1 — Vercel website se (sabse asaan):**
1. https://vercel.com par jaayein aur account bana lein (free hai, GitHub/Google se login).
2. "Add New Project" → "Deploy" section me niche "Upload" option milega, ya
3. Poora `bday-site` folder ko zip karke drag & drop kar dein Vercel dashboard me.
4. Deploy dabayein — 30 second me live link mil jayega jo aap apni Janu ko aur unke bhai ko bhej sakte hain.

**Option 2 — Vercel CLI se (agar terminal use karte hain):**
```bash
npm install -g vercel
cd bday-site
vercel
```
Terminal me jo sawal aayenge unka default answer (Enter) dabate jaayein, aakhir me live URL mil jayega.

**Option 3 — GitHub se:**
1. Is folder ko GitHub repo bana kar upload kar dein.
2. Vercel dashboard me "Import Project" → apna GitHub repo select karein → Deploy.

Bas! Website ready ho jayegi, welcome animation, shayari, videos aur pins sab kaam karenge.
