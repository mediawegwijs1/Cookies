# 🍪 Demo cookies en privacy

Een interactieve, educatieve webdemo die **kinderen (ca. 8–12 jaar)** laat zien wat er gebeurt als je op websites cookies accepteert. De demo maakt zichtbaar **welke bedrijven (trackers) meekijken**, hoe ze je volgen over meerdere websites en **welk profiel** ze van je kunnen opbouwen.

De demo bestaat uit één los HTML-bestand. Je hebt geen installatie, server of internetverbinding nodig.

---

## 📑 Inhoud

- [Doel](#-doel)
- [Snel starten](#-snel-starten)
- [Bestanden in deze repository](#-bestanden-in-deze-repository)
- [Hoe werkt de demo?](#-hoe-werkt-de-demo)
- [Onderdelen van het scherm](#-onderdelen-van-het-scherm)
- [Gebruik in de klas](#-gebruik-in-de-klas)
- [Technische werking](#-technische-werking)
- [Aanpassen](#-aanpassen)
- [Privacy van de demo zelf](#-privacy-van-de-demo-zelf)
- [Bekende beperkingen](#-bekende-beperkingen)

---

## 🎯 Doel

Veel kinderen (en volwassenen) klikken een cookiebanner automatisch weg met **"Alles accepteren"**. Met deze demo zie je wat dat betekent:

- 🔵 **Blauw** = websites die je bezoekt
- 🟠 **Oranje** = trackers: bedrijven die informatie over jou krijgen
- Een **netwerk van lijnen** laat zien welke trackers op welke websites zitten
- Een **Privacy-Paspoort** laat zien wat bedrijven over je kunnen afleiden, zoals je hobby's, interesses en leeftijdsgroep

De belangrijkste les staat aan het eind:
> **Tip:** kies vaker *Alleen noodzakelijke cookies* als je minder gevolgd wilt worden.

---

## 🚀 Snel starten

1. Download of clone deze repository:
   ```bash
   git clone https://github.com/mediawegwijs1/Cookies.git
   ```
2. Open het bestand **`demo_cookies_en_privacy_v7 (1).html`** in een moderne browser (Chrome, Edge, Firefox of Safari).
3. Klik op een website in de linkerkolom en maak een keuze in de cookiebanner.

Je hoeft niets te installeren. Alles draait lokaal in de browser.

> 💡 Gebruik voor de beste weergave een breed scherm, bijvoorbeeld een laptop, desktop of digibord. De lay-out bestaat uit drie kolommen van samen ongeveer 1100 px breed of meer.

---

## 📁 Bestanden in deze repository

| Bestand | Beschrijving |
|---|---|
| `demo_cookies_en_privacy_v7 (1).html` | **De volledige, werkende demo** (HTML + CSS + JavaScript in één bestand). Dit bestand open je. |
| `cookies demo.txt` | Een onvolledige versie van de HTML/CSS-opmaak. Het JavaScript-gedeelte ontbreekt hierin (er staat alleen een placeholder), dus dit bestand werkt **niet** als demo. Het is alleen handig als referentie. |
| `README.md` | Deze documentatie. |

---

## 🕹️ Hoe werkt de demo?

1. **Kies een website.** Links staan 49 kindvriendelijke, fictieve websites, zoals `GameFun.com`, `VoetbalArena.nl`, `KinderKrant.nl` en `SpaceNerds.nl`.
2. **Er verschijnt een cookiebanner.** Daarin kies je:
   - **Alleen noodzakelijke cookies**: geen trackers toegestaan.
   - **Alle cookies accepteren**: de trackers op die website krijgen je gegevens.

   De tekst van de banner wisselt steeds af tussen drie varianten, net als bij echte websites waar de vraag telkens anders wordt gesteld.
3. **Bekijk wat er gebeurt:**
   - Bij *Alles accepteren* worden de lijnen van die website naar de trackers **dikgedrukt** in het netwerk.
   - In het logboek **"Wat is er zojuist gebeurd?"** zie je welke bedrijven je op die site zagen.
   - De teller **"keer jou gezien"** van de betreffende trackers gaat omhoog.
   - Je **Privacy-Paspoort** wordt verder ingevuld.
4. **Een bezochte website wordt grijs** en kan niet nog een keer worden aangeklikt.
5. Klik op **Eindresultaat** voor een samenvatting.
6. Klik op **Reset** om opnieuw te beginnen.

---

## 🧩 Onderdelen van het scherm

### 1. Websites (linkerkolom)
Een lijst met knoppen voor alle websites. Daaronder staan:
- **Reset**: zet alle tellers, het logboek, het paspoort en de knoppen terug.
- **Eindresultaat**: opent een overzicht van je sessie.

### 2. "Wie kijkt er mee?" (middenkolom)
- **Netwerkdiagram (SVG):** websites links (blauw) en trackers rechts (oranje), verbonden met lijnen. **Hoe groter een oranje bol, hoe meer websites die tracker volgt.**
- **Logboek:** een tijdlijn van je keuzes met tijdstip. De nieuwste melding staat bovenaan.
- **Trackerkaarten:** per tracker zie je hoe vaak die jou heeft gezien en op hoeveel sites die aanwezig is.

De 12 fictieve trackers zijn:
`ReclameMaatje`, `SocialKijker`, `DataSnuffel`, `LikeVrienden`, `ShopVolger`, `VideoAnalist`, `KlikMeter`, `ProfielBouwer`, `AdRaketten`, `SuperStatistiek`, `BannerBooster`, `TrendTeller`.

### 3. Jouw Privacy-Paspoort (rechterkolom)
Een "paspoort" dat laat zien wat bedrijven over jou te weten kunnen komen:

| Veld | Voorbeeld |
|---|---|
| **Hobby** | Sport (voetbal), Gamen, Skaten, Zwemmen |
| **Interesses** | Muziek, Ruimte, Wetenschap, Honden |
| **Leeftijdsgroep** | Kind (8–12) |
| **Onthouden** | Je taal, Je voorkeuren, Je login, Je locatie |

Daaronder staat een **scorebord**:
- aantal **sites bezocht**
- aantal **sites waar je gevolgd bent**
- aantal **bedrijven die jou nu volgen**

### 4. Eindresultaat (pop-up)
Een samenvatting met:
- de statistieken van het scorebord
- de **meest actieve tracker** (die jou het vaakst heeft gezien)
- je volledige profiel als labels (chips)
- de tip om vaker voor *Alleen noodzakelijke cookies* te kiezen

---

## 🏫 Gebruik in de klas

Een mogelijke lesopzet van 20–30 minuten:

1. **Introductie (5 min).** Vraag: *"Wat doe jij als je een cookiemelding ziet?"*
2. **Ronde 1: alles accepteren (5–10 min).** Laat leerlingen 10 websites bezoeken die bij hun eigen hobby's passen en steeds **Alle cookies accepteren** kiezen. Bekijk daarna het **Eindresultaat**.
3. **Bespreken.** Welke bedrijven volgden je het meest? Klopt je paspoort? Hoe kan een bedrijf dat weten?
4. **Ronde 2: alleen noodzakelijk (5–10 min).** Klik op **Reset** en bezoek dezelfde websites, maar kies nu **Alleen noodzakelijke cookies**. Vergelijk het scorebord met ronde 1.
5. **Afsluiting.** Bespreek de tip en wat leerlingen voortaan anders gaan doen.

**Gespreksvragen:**
- Waarom zitten sommige trackers op heel veel websites?
- Wat is het verschil tussen *noodzakelijke* cookies en *tracking*cookies?
- Waarom zouden bedrijven willen weten hoe oud je bent of wat je hobby's zijn?

> ℹ️ Bij elke pagina-herlaadactie worden trackers **willekeurig** over de websites verdeeld. Elke leerling ziet dus een iets ander netwerk. Dat is handig om resultaten met elkaar te vergelijken.

---

## ⚙️ Technische werking

De demo is gebouwd met **vanilla HTML, CSS en JavaScript**, zonder frameworks of externe bibliotheken.

### Willekeurige verdeling van trackers
Bij het laden krijgt elke website een willekeurig aantal trackers:

| Aantal trackers | Kans |
|---|---|
| 0 | 10% |
| 1 | 20% |
| 2 | 40% |
| 3 | 30% |

Daarna worden **twee "populaire" trackers** gekozen die elk op **10 tot 19 extra websites** worden geplaatst. Zo ontstaat een realistisch beeld waarin een paar grote bedrijven je bijna overal volgen.

### Opbouw van het Privacy-Paspoort
- Veel websites hebben een vaste **profielhint** (`PROFILE_HINTS`). `SkatePark.nl` voegt bijvoorbeeld de hobby *Skaten* toe.
- Websites zonder hint voegen een **willekeurige** hobby, interesse of "onthouden"-item toe (`EXTRA_HOBBIES`, `EXTRA_INTERESTS`, `EXTRA_REMEMBER`).
- **Leeftijdsinschatting:** na het bezoeken van 2 of meer typische kindersites (`AGE_SITES`) wordt *Kind (8–12)* ingevuld.

### Belangrijke functies

| Functie | Wat doet het? |
|---|---|
| `init()` | Maakt de knoppen en nodes, verdeelt de trackers en tekent het netwerk. |
| `randomizeAssignment()` | Verdeelt trackers willekeurig over de websites. |
| `renderSvg()` | Tekent het netwerk (lijnen, websites, trackers) in SVG. |
| `attemptVisit()` | Opent de cookiebanner voor een website. |
| `visitSite()` | Verwerkt de keuze: markeert lijnen, werkt tellers, logboek en paspoort bij. |
| `updatePassport()` | Vult het Privacy-Paspoort aan. |
| `updateTrackerSizes()` | Past de grootte van trackerbollen aan op basis van hun bereik. |
| `hardResetCounters()` | Zet alles terug naar de beginstand (de trackerverdeling blijft gelijk). |

---

## 🛠️ Aanpassen

Alle instellingen staan bovenaan het `<script>`-blok onder `// ---------- Config ----------`:

- **`SITES`**: de lijst met websites. Voeg namen toe of verwijder ze.
- **`TRACKERS`**: de lijst met trackerbedrijven.
- **`PROFILE_HINTS`**: welke website wat aan het paspoort toevoegt, bijvoorbeeld:
  ```js
  "MijnSite.nl": {hobby: "Tekenen"}
  // mogelijke sleutels: hobby, interest, age, remember
  ```
- **`EXTRA_HOBBIES` / `EXTRA_INTERESTS` / `EXTRA_REMEMBER`**: willekeurige aanvullingen voor websites zonder hint.
- **`AGE_SITES`**: websites die meetellen voor de leeftijdsinschatting.
- **Kleuren**: aan te passen via de CSS-variabelen in `:root` (`--blue`, `--orange`, `--bg`, `--reset`, `--result`).

> Tip: geef het bestand een eenvoudigere naam, bijvoorbeeld `index.html`. Dan kun je het ook via **GitHub Pages** publiceren.

---

## 🔒 Privacy van de demo zelf

- De demo **plaatst zelf geen cookies** en gebruikt geen `localStorage`.
- Er worden **geen gegevens verzonden**. Alles gebeurt lokaal in de browser.
- Alle websites en trackers zijn **fictief**.
- Na het sluiten of herladen van de pagina is alles weg.

---

## ⚠️ Bekende beperkingen

- **Het paspoort groeit ook bij "Alleen noodzakelijke cookies".** Het Privacy-Paspoort wordt bij elk websitebezoek aangevuld, ongeacht je keuze. Alleen de trackers, lijnen en het scorebord houden rekening met de keuze. Benoem dit in de klas, of pas `visitSite()` aan zodat `updatePassport()` alleen wordt aangeroepen als `allowTrackers` waar is.
- **Geen responsieve lay-out.** De vaste drie-koloms indeling werkt niet goed op telefoons.
- De code bevat de opmerking "50 kindgerichte websites", maar de lijst bevat er **49**.
- `cookies demo.txt` is onvolledig. Gebruik altijd het HTML-bestand.
- **Reset** maakt geen nieuwe trackerverdeling aan. Herlaad de pagina (F5) voor een nieuw willekeurig netwerk.

---

## 📄 Licentie

Er is nog geen licentie opgegeven. Neem contact op met de eigenaar van de repository (**mediawegwijs1**) als je de demo wilt hergebruiken of aanpassen.
