POWERBALL PREDICTOR SA — ANDROID INSTALLABLE WEB APP

This is a working Progressive Web App (PWA). It can be installed on Android from Chrome after it is hosted on an HTTPS website.

QUICK START
1. Extract the ZIP.
2. Upload the contents of this folder to any HTTPS static web host (for example GitHub Pages, Netlify, or your own website).
3. Open the hosted address in Chrome on your Android phone.
4. Chrome menu (⋮) > Install app / Add to Home screen.

LOCAL PREVIEW
You need a local web server; opening index.html directly may prevent service-worker installation. From this folder run:
  python -m http.server 8000
Then open http://localhost:8000 on the same computer.

HISTORICAL DATA
The app does NOT ship with a verified historical results database. Use Import CSV with columns:
date,n1,n2,n3,n4,n5,pb
Example:
2026-11-06,5,17,24,40,45,3
The app validates number ranges and calculates frequency, gaps, repeated pairs, and PowerBall frequency. "Load demo data" creates synthetic data only and is clearly labelled as demo.

IMPORTANT MODEL NOTES
- The generator's pattern score is a descriptive heuristic, not a probability of winning.
- The three generation modes are balanced, frequency mix, and random.
- Back-testing is a simple walk-forward historical comparison and should be interpreted cautiously.
- Each valid line has the same jackpot probability. Past draws do not make a number due.
- Current assumed format: 5 distinct main numbers from 1–50 plus one PowerBall from 1–16.

APK
This bundle is a PWA, not a signed APK. It installs directly from Chrome once hosted over HTTPS. To publish a native APK, wrap the hosted PWA using Android Studio/Trusted Web Activity (Bubblewrap) and sign it with your own Android signing key. This project does not generate or sign an APK.
