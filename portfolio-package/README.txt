========================================
JOJI KHAN — PORTFOLIO — SETUP GUIDE
========================================

Ye poora folder Netlify par upload karne ke liye tayyar hai.
Bas apni files sahi jagah rakhein aur "index.html" ko haath mat lagayein
(sirf zaroorat par).

----------------------------------------
FOLDER STRUCTURE (jo aapke pass hai)
----------------------------------------

portfolio-package/
├── index.html                      <- MAIN FILE (naam mat badlein)
├── README.txt                      <- ye file
│
├── images/
│   ├── design/                     <- GRAPHIC DESIGN / POSTERS yahan
│   │     design-01.jpg
│   │     design-02.jpg
│   │     design-03.jpg
│   │     design-04.jpg
│   │     design-05.jpg
│   │     design-06.jpg
│   │
│   ├── photography/                <- PHOTOGRAPHY yahan
│   │     photo-01.jpg
│   │     photo-02.jpg
│   │     photo-03.jpg
│   │     photo-04.jpg
│   │     photo-05.jpg
│   │     photo-06.jpg
│   │     photo-07.jpg
│   │     photo-08.jpg
│   │
│   └── video-thumbnails/           <- VIDEO KA COVER IMAGE yahan
│         video-01-thumb.jpg
│         video-02-thumb.jpg
│         video-03-thumb.jpg
│         video-04-thumb.jpg
│
└── videos/                         <- SIRF chhoti video files (agar chahein)
      (khali — neeche padhein)


----------------------------------------
STEP 1 — APNI PHOTOS/POSTERS DAALEIN
----------------------------------------

1. Apni graphic design / poster ki images ko "images/design/" folder mein
   daal dein.
2. Apni photography ki images ko "images/photography/" folder mein daal
   dein.
3. Sabse aasan tareeqa: apni file ka naam wahi rakhein jo upar list mein
   likha hai (jaise design-01.jpg, photo-03.jpg).
   - Agar naam match nahi karta, koi masla nahi — bas index.html file
     Notepad se kholein, Ctrl+F se "design-01.jpg" (ya jo bhi naam)
     dhoondein, aur apni asal file ka naam wahan likh dein.

Agar kisi slot ki photo abhi nahi hai to koi masla nahi — us jagah
khud-bakhud ek khoobsurat placeholder design dikh jayega, site kharab
nahi hogi.


----------------------------------------
STEP 2 — VIDEOS KA TAREEQA (ZAROORI PADHEIN)
----------------------------------------

Netlify ka FREE plan kisi bhi EK file ko 10MB se zyada allow nahi karta.
Ek 2-3 minute ki video normally 50MB-500MB ki hoti hai — is liye video
ko seedha is folder mein daalna kaam nahi karega (upload fail ho jayega).

BEHTAR TAREEQA (recommended):
1. Apni video YouTube par "Unlisted" (ya Public) upload kar dein.
   (Vimeo bhi chal jayega)
2. Us video ka sirf ek COVER/THUMBNAIL image nikal kar
   "images/video-thumbnails/" mein rakh dein.
3. index.html mein videoWorks wale hisse mein "link:" ke aage
   apni YouTube video ka URL paste kar dein.
   Example:
      link:'https://youtube.com/watch?v=ABC12345'
4. Bas — website par click karne se video YouTube par khul jayegi.

AGAR CHHOTI VIDEO CLIP KHUD SITE PAR CHALANI HAI (10MB se kam):
1. Video file ko "videos/" folder mein rakh dein, jaise "clip-01.mp4"
2. index.html mein us item ki line mein "link:" hata kar
   "file:" likh dein:
      file:'videos/clip-01.mp4'
   (thumb: wali line waisi hi rehne dein — wo poster/cover ka kaam karegi)


----------------------------------------
STEP 3 — NETLIFY PAR UPLOAD
----------------------------------------

1. netlify.com par free account banayein
2. app.netlify.com/drop par jayein
3. is poore "portfolio-package" folder ko wahan drag-drop kar dein
   (poora folder uthayein, sirf index.html nahi)
4. chand second mein live link mil jayega
5. dashboard mein "Customize" se apna pasand ka naam rakh lein,
   jaise: jojikhan.netlify.app


----------------------------------------
BAAD MEIN UPDATE KARNA HO TO
----------------------------------------

1. Isi folder mein nayi photo/poster daal dein (ya purani replace kar
   dein)
2. Agar naya item add karna hai to index.html mein us catalogue ki
   list mein ek naya line add kar dein (upar wale format jaisa)
3. Poora updated folder dobara Netlify ke "Deploys" tab ke drag-drop
   box mein daal dein
4. Link WAHI rahega — sirf content update ho jayega
