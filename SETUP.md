# ResumeCraft Download Website

## 1. Install
Open this folder in VS Code, then run:

```bash
npm install
npm run dev
```

## 2. Add the APK
Copy your Flutter release APK into:

`public/downloads/ResumeCraft.apk`

For example, from your Flutter project you can use the APK produced by:

```bash
flutter build apk --release
```

## 3. Test
Open the local Vite URL shown in the terminal and click **Download for Android**.

## 4. Production build

```bash
npm run build
```

The production files will be in `dist/`. This default build uses the site root, as expected by Vercel.

## 5. Deploy
This project is ready for Vercel, Netlify, or GitHub Pages. Keep `ResumeCraft.apk` inside `public/downloads/` before deployment.

The GitHub Pages workflow builds with its repository subpath automatically. For a manual GitHub Pages build, use:

```bash
npm run build -- --base=/ResumeCraft-Website/
```

### Important
The website does not create the APK. It hosts and serves the APK you already built with Flutter.
