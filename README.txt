Skill Wheel ToE CZ – Android projekt

Projekt je připraven jako jednoduchá fullscreen WebView aplikace.
Načítá lokální index.html a Ruffle runtime z assets, takže nevyžaduje internet.

Poznámka:
V dodaných souborech chybí fallback chunk:
core.ruffle.831c4f4a93befb9e84af.js
Na moderním Android WebView se očekává použití SIMD varianty
core.ruffle.0875e44536e955474b0c.js, kterou projekt obsahuje.
Pro maximální kompatibilitu je vhodné doplnit i fallback soubor.

Sestavení:
Android Studio -> Open project -> Build APK.
