ANKISMART – INSTALOVATELNÁ WEBOVÁ APLIKACE (PWA)

DŮLEŽITÉ:
Samotný soubor HTML otevřený přes file:// nelze v Chrome nainstalovat jako PWA.
Pro instalaci musí být tato složka zveřejněna na HTTPS adrese (např. GitHub Pages,
Netlify nebo vlastní webhosting). Po nasazení otevři HTTPS adresu v Chrome na Androidu
a zvol „Nainstalovat aplikaci“ / „Přidat na plochu“.

OBSAH:
- index.html: aplikace
- manifest.webmanifest: název, ikony a režim samostatné aplikace
- sw.js: service worker pro aplikační shell a cache
- icons/: ikony aplikace

UPOZORNĚNÍ:
Některé části původní aplikace načítají knihovny, písma nebo CSS z internetu.
Service worker ukládá lokální aplikační soubory; úplně první načtení a import .apkg
proto vyžadují internet. Uložená data kartiček zůstávají v úložišti przeglížeče
(localStorage) daného webu.
