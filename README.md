# Projekt: Webbplats för Yoga Studio Hälsocenter

Detta projekt är en del av en akademisk examinationsuppgift där målet har varit att planera, designa och utveckla en modern, tillgänglig och responsiv webbplats för ett fiktivt företag inom hälsa och välmående. Projektet har tagits fram i två huvudsakliga steg: en visuell designfas i Figma och en teknisk prototypfas i semantisk HTML och CSS, redo att transformeras till ett dynamiskt WordPress-tema.

---

## 📋 Lärarens krav (Grundkrav & Funktionalitet)

Uppgiften ställer strikta krav på såväl designprocessen som den tekniska implementationen:
1. **Tydlig grafisk profil:** Skapa ett enhetligt färgtema, logotyp, favicon och moodboard.
2. **Användbarhet & Tillgänglighet (UX/UI):** Webbplatsen ska ha ett tillgängligt gränssnitt som strävar efter att uppfylla WCAG-riktlinjerna för färgkontraster och struktur.
3. **Responsiv design:** Sidorna ska fungera och se bra ut på både stora (Desktop) och små (Mobil) skärmar.
4. **Obligatoriska sidtyper & sektioner:**
   - Presentation av företaget (Om oss) och dess nyckelpersoner.
   - Presentation av företagets olika tjänster och aktiviteter.
   - Startsida med "puffar" för viktiga händelser, erbjudanden eller nyheter.
   - Nyhetsflöde/Blogg med "utvald bild"-funktionalitet och enskilda artikelsidor (`single`).
   - Funktion för bokning (Boka-sida).
5. **Designfiler (Figma):** Skapande av designskiss för dator/mobil, en sitemap (strukturschema) samt en moodboard.
6. **Korrekt kodstandard:** HTML- och CSS-kod ska vara välstrukturerad, kommenterad och validerad enligt webbstandard.
7. **WordPress CMS-förberedelse:** Strukturen ska vara planerad för att enkelt kunna konverteras till ett eget, tomt WordPress-tema med dynamiskt innehåll, rollfördelning och SEO-strategi.

---

## 🛠️ Hur har arbetat genomförts för att uppfylla kraven

Projektet har utvecklats systematiskt för att säkerställa att varje enskilt krav från läraren uppfylls till 100 %. Nedan beskrivs hur arbetsflödet har sett ut:

### 1. Planering & Grafisk profil (Figma)
- **Designskiss:** En High-Fidelity-skiss har skapats i Figma för samtliga undersidor. Skissen inkluderar exakta marginaler, komponenter och flöden.
- **Responsivitet:** Designen ritades upp för både Desktop och Mobil för att visualisera hur element staplas och hur menyn döljs bakom en hamburgerikon (☰) på mindre skärmar.
- **Moodboard & Färger:** Ett harmoniskt, jordnära färgtema har valts (mjuk beige bakgrund, skogsgröna accentfärger för knappar/kort samt mörkgrå text för optimal läsbarhet). Typsnitt, radavstånd och bildspråk definierades här.
- **Sitemap:** Ett flödesschema ritades upp för att kartlägga användarresan från startsidan till de fem unika undersidorna.

### 2. Teknisk struktur & Semantisk HTML
Det har byggt en komplett, statisk prototyp bestående av följande filer:
- `index.html` (Startsida): Innehåller en stor välkomnande Hero-sektion samt strategiska "puffar" som lyfter fram aktuella kurser och de senaste nyheterna.
- `om-oss.html` (Presentation): Presenterar studion samt nyckelpersonerna/instruktörerna (Anna och David) med profilkort.
- `tjanster.html` (Tjänster): Visar ett strukturerat grid över studions utbud (Vinyasa, Yin Yoga, Privatlektioner).
- `nyheter.html` (Bloggflöde): Visar ett vertikalt grid med nyhetskort, utvalda bilder, datum/kategorier och "Läs hela artikeln"-länkar.
- `singel.html` (Artikelsida): En dedikerad mall för att läsa en specifik nyhet i ett mer lättläst, smalare textformat med citatblock (blockquote).
- `boka.html` (Bokningssida): Ett komplett gränssnitt för ett bokningsformulär där kunden kan fylla i sina uppgifter samt viktig praktisk information om avbokningsregler.

### 3. Tillgänglighet (WCAG) & Responsiv CSS (`style.css`)
- **Färgkontraster:** För att möta WCAG-kraven lades mörka, transparenta filter (`linear-gradient`) över alla Hero-bilder i CSS. Detta säkerställer att den vita texten ovanpå bilderna har ett högt kontrastvärde och är lättläst.
- **Flexbox & Grid:** CSS Grid och Flexbox har använts för att skapa moderna layouter som automatiskt anpassar sig.
- **Media Queries:** Med hjälp av `@media (max-width: 768px)` har hela webbplatsen mobilanpassats. Navigeringsmenyn förvandlas till en mobilmeny, och alla grids (tjänster, nyheter, instruktörer) staplas snyggt i en kolumn.
- **Logotyp & Favicon:** En skräddarsydd logotyp skapades och implementerades i headern som en klickbar enhet (SVG/PNG) tillsammans med företagets namn. Texten döljs automatiskt på mobilen för att spara utrymme. En matchande favicon (`.jpg`) har kopplats korrekt i samtliga HTML-head-taggar.

---

## 🚀 Nästa steg: WordPress-konvertering
Denna HTML/CSS-prototyp är helt förberedd för att flyttas in i en lokal WordPress-miljö (XAMPP). Kodbasen är modulär, vilket gör det enkelt att bryta ut den till `header.php`, `footer.php`, `page.php` och `single.php` för att aktivera "The Loop" och göra allt innehåll dynamiskt redigerbart för företagets administratörer och redaktörer.