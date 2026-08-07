# Skill Wheel ToE CZ

Offline Android obal pro český **Heroes of Might and Magic V: Tribes of the East – Skill Wheel 3.0**.
Původní SWF běží přes lokálně přibalený Ruffle runtime. Aplikace nevyžaduje internet.

## Aktuální stav

- Android WebView + `WebViewAssetLoader`
- Ruffle self-hosted runtime
- původní český `skillwheel3.swf`
- vlastní spodní panel pro detail skillu
- data skillů v `app/src/main/assets/data/skills_cs.json`
- automatický debug APK build přes GitHub Actions

## Struktura webové části

- `assets/index.html` – kostra UI
- `assets/css/style.css` – vzhled
- `assets/js/dataLoader.js` – načtení databáze
- `assets/js/skillSheet.js` – detail skillu
- `assets/js/app.js` – start aplikace a Ruffle
- `assets/data/skills_cs.json` – česká data skillů

## Build

GitHub Actions sestaví `app-debug.apk` pomocí workflow `.github/workflows/build-apk.yml`.
