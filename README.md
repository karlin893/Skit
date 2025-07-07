Absolut! Här kommer en fullständig beskrivning av hemsidans layout, struktur, tema och funktionalitet – sammanfattat på ett sätt som ger dig en övergripande teknisk och visuell förståelse för att bygga, dokumentera eller vidareutveckla Älgholm RP:s webbplats.

⸻

🌐 Webbplatsöversikt: Älgholm RP – Din Bloxburg Gemenskap

🔹 Mål med webbplatsen

Att ge medlemmar i Älgholm RP (en Roblox Bloxburg-rollspelsserver) en samlad digital plats för:
	•	Karaktärshantering
	•	Bostadsannonsering
	•	Jobbsökning
	•	RP-sessioner
	•	Nyheter, företag & kommuninfo
	•	Kommunikation och rollspecifika verktyg

⸻

🎨 Tema och Designstil

Element	Värde / Användning
Färgpalett	Blå toner (from-blue-50 till to-blue-200) med accenter av gult, grönt, rött beroende på kontext (t.ex. knappar).
Typsnitt	Sans-serif (via Tailwind CSS), modern och lättläst.
Designstil	Kortbaserad layout, responsiv, mjuka rundade hörn, skuggor och färgblock.
Ikoner	Font Awesome – används för att representera innehåll visuellt (hus, jobb, meddelanden, etc).


⸻

🧱 Layoutstruktur

Webbplatsen är uppdelad i sektioner, där endast en är synlig i taget (via JavaScript). Här är den hierarkiska strukturen:

<body>
 ├─ <nav>               ← Huvudnavigering
 ├─ <main>
 │   ├─ #home-section         ← Startsida
 │   ├─ #my-algholm-section   ← Inloggat användargränssnitt
 │   ├─ #housing-section      ← Bostäder
 │   ├─ #jobs-section         ← Jobb
 │   ├─ #rp-sessions-section  ← RP-sessioner
 │   ├─ #news-channel-section ← Nyheter
 │   ├─ #businesses-section   ← Företag
 │   ├─ #school-section       ← Skola
 │   └─ #municipality-section ← Kommun
 ├─ <div class="modal">       ← Modaler (popup-fönster)
</body>


⸻

🔝 Navigationsfält (Nav-bar)
	•	Position: Högst upp, sticky.
	•	Färg: Mörkblå (bg-blue-800), vit text.
	•	Innehåll:
	•	Logotyp (bild) + “Älgholm RP”-text
	•	Navigeringslänkar (Startsida, Hitta Bostäder, Sök Jobb, RP-sessioner, Nyheter, Företag, Kommunen)
	•	Knapp: “Logga in / Skapa konto” – gul, rundad
	•	Länk: “Mitt Älgholm” – visas bara när användaren är inloggad

⸻

🧩 Huvudsektioner (Main Sections)

🏠 1. Startsida (#home-section)
	•	Stor välkomstrubrik: “Välkommen till Älgholm!”
	•	Beskrivande text om spelet/staden
	•	4 funktionskort med ikon + rubrik + beskrivning:
	•	Hitta ditt drömhem
	•	Bygg din karriär
	•	Upptäck lokala företag
	•	Regnbågsskolan
	•	CTA-knapp: “Bli en del av Älgholm idag!” – blå, stor, fet

⸻

👤 2. Mitt Älgholm (#my-algholm-section)

Endast synlig vid inloggning. Delad i tre områden:

🧍 a) Profil
	•	Profilbild (rund, klickbar för uppladdning)
	•	Karaktärsinformation: Namn, personnummer, Discord, typ, drömjobb
	•	Roller
	•	Knapp: “Ladda upp profilbild”

📅 b) Mina Aktiviteter
	•	Nuvarande bostad
	•	Nuvarande jobb
	•	Kommande evenemang

✉️ c) Mina Meddelanden
	•	Lista över meddelanden, olästa i gul bakgrund
	•	Knapp: “Markera alla som lästa”
	•	Adminknappar (dolda): Visa alla meddelanden, Hantera användare

🛠️ d) Rollspecifika Verktyg
	•	Dynamiskt genererade knappar beroende på användarroll (polis, läkare etc)

🔘 e) Åtgärdsknappar
	•	Skicka meddelande (grön)
	•	Logga ut (röd)

⸻

🏘️ 3. Bostäder (#housing-section)
	•	Rubrik: “Hitta Bostäder i Älgholm”
	•	Kort-layout: varje kort visar bostad med bild, info och pris
	•	Dynamiskt innehåll laddas in via JS
	•	Knapp (dold): “Lägg ut annons”

⸻

💼 4. Jobb (#jobs-section)
	•	Rubrik: “Sök Jobb i Älgholm”
	•	Dynamiskt innehåll från JS
	•	Knapp (dold): “Lägg ut jobbannons”

⸻

🎭 5. RP-sessioner (#rp-sessions-section)
	•	Rubrik: “RP-sessioner i Älgholm”
	•	Lista över sessionsplaner
	•	Knapp (dold): “Skapa ny RP-session”

⸻

📰 6. Nyhetskanal (#news-channel-section)
	•	Rubrik: “Älgholms Nyhetskanal”
	•	Dynamiska nyhetskort
	•	Knapp (dold): “Skapa nyhet”

⸻

🏢 7. Företag (#businesses-section)
	•	Rubrik: “Företag i Älgholm”
	•	Fyra företagskort med ikon, namn, beskrivning:
	•	Karlssons Körskola
	•	Karlssons Ekonomi
	•	Karlssons Juridik
	•	Din Advokat
	•	Hovereffekter på alla kort
	•	“Mer info”-knappar öppnar modaler

⸻

🏫 8. Skola (#school-section)
	•	Rubrik: “Regnbågsskolan”
	•	Vision och kursutbud (Matte, Svenska, Konst, Naturvetenskap, Idrott)
	•	Skolbild och beskrivning

⸻

🏛️ 9. Kommunen (#municipality-section)
	•	Rubrik: “Älgholms Kommun”
	•	Kommunhusbild
	•	Punktlista över tjänster (bygglov, räddningstjänst etc.)
	•	Knappar till förvaltningar:
	•	Sjukvård (röd)
	•	Polis (blå)

⸻

💬 Modaler (Pop-up-fönster)

Modaler används för:
	•	Visning av detaljer (bostad, jobb, företag, RP-session, nyhet)
	•	Skapa nytt (annons, nyhet, session)
	•	Skicka meddelande
	•	Adminfunktioner
	•	Notifikationer (temporära “toast”-meddelanden)

Alla modaler:
	•	Centreras på skärmen
	•	Har mörk bakgrund (rgba(0,0,0,0.7))
	•	Har vit box med rundade hörn, max-bredd: 700px
	•	Har “X”-knapp i hörnet för stängning
	•	Notiser visas i övre högra hörnet och försvinner automatiskt

⸻

⚙️ Interaktivitet och JavaScript (förväntat beteende)

Javascript används (eller förväntas användas) för:

Funktion	Beskrivning
Sektionbyte	Navigationslänkar visar rätt <section>
Inloggning/Utloggning	Döljer/visar #my-algholm-section och relaterade knappar
Dynamiskt innehåll	Bostäder, jobb, nyheter etc laddas från JS/JSON/API
Modalhantering	Öppna/stäng modaler för info och formulär
Rollstyrd åtkomst	Dölja/visa knappar/modaler beroende på användarroll
Meddelandehantering	Skicka, läsa, visa notifikationer
Filuppladdning	Profilbild via <input type="file">
Responsiv hamburgermeny	Visa/dölj nav på små skärmar


⸻

📱 Responsivitet (Mobilvänlighet)
	•	Tailwind CSS-klasser används för att anpassa layout beroende på skärmstorlek.
	•	Mobilmeny (hamburger) visas på mindre skärmar.
	•	Rutnätslayouter går från 2–3 kolumner till 1 kolumn.
	•	Knappar och texter skalas automatiskt för mobil.

⸻

📁 Filstruktur (För lokal testning)

Om du vill spara detta projekt lokalt kan strukturen se ut så här:

/älgholm-rp/
├─ index.html
├─ style.css (om du skriver extra CSS)
├─ script.js
├─ /img/
│   ├─ mkk.jpg (logga)
│   └─ andra bilder

CDN:er för Tailwind & Font Awesome kan ligga i <head> i index.html.

⸻

✅ Sammanfattning

Älgholm RP:s webbplats är en komplett communityplattform för en Bloxburg RP-server, byggd med moderna webbtekniker (HTML, Tailwind CSS, JS). Den är mobilanpassad, har rollstyrda funktioner, och ett stort fokus på interaktivitet via modaler och dynamiskt innehåll. Sidan är lätt att vidareutveckla både som ren HTML/JS-projekt eller som CMS-baserad lösning i t.ex. Webflow + Memberstack/Wized.

⸻

Vill du att jag nu:
	•	📦 Skapar en färdig HTML-fil som du kan köra direkt?
	•	🧱 Hjälper dig bygga detta i Webflow?
	•	💻 Visar hur du testar det på din dator?

Välj nästa steg så hjälper jag dig!
