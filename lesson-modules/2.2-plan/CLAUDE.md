# 2.2 Planeerimine

Enne ehitamist peame selgeks tegema, mida me ehitame.

Seda nimetatakse "nõueteks" – põhimõtteliselt kirjeldus, kuidas su viktoriin peaks töötama ja välja nägema.

STOP: Kas oled kunagi kellelegi andnud ebamääraseid juhiseid ja saanud midagi täiesti teistsugust, kui ootasid?

USER: Yes / Definitely

---

Just nii lähebki, kui nõuded vahele jätta. Mida rohkem me nüüd detaile paika paneme, seda paremini saan ma ehitada seda, mida sa tegelikult tahad.

Ma hakkan sind su viktoriini kohta intervjueerima. Mõtleme välja isiksuse-kohvi paarid, stiili, küsimused. Siis salvestan kõik faili, et meil oleks selge spetsifikatsioon, millelt ehitada.

STOP: Mõtle sellest nagu töövõtja instruktaaž enne töö algust. Mida selgem ülevaade, seda parem tulemus. Valmis alustama?

USER: Yes

---

Ma kasutan tööriista nimega AskUserQuestion – see annab sulle ilusad nupud, mille vahel valida, selle asemel et sa peaksid tippima. Sa võid mul paluda seda igal ajal kasutada, kui tahad mugavamat viisi otsuste tegemiseks. Ütle lihtsalt "küsi mult" või "anna mulle valikud".

Proovime kohe.

ACTION: Use AskUserQuestion with two questions:
- Q1 Header: "Results" / Question: "How many personality/coffee pairings should your quiz have?" / Options: "3 - Simple and focused", "4 - Good variety (Recommended)", "5 - More distinctions", "6 - Maximum variety"
- Q2 Header: "Question vibe" / Question: "What style of questions do you want?" / Options: "Fun pop culture (Harry Potter, Netflix, etc.)", "Lifestyle & preferences (travel, food, weekends)", "Abstract & quirky (colors, scenarios, hypotheticals)", "Mix of everything"

USER: [Selects options]

Suurepärased valikud! Nüüd valime su tegelikud isiksuse-kohvi paarid.

---

Pea meeles: viktoriin soovitab KOHVI isiksuse põhjal. Nii et peame otsustama, millised isiksused millisele joogile vastavad.

Siin on 10 paaringusoovitust. Vali [X] tükki vastavalt sellele, mitu tulemust sa varem valisid. Kirjuta lihtsalt numbrid, näiteks "1, 4, 7":

1. **Bold Adventurer** → Double Espresso - "Sa elad intensiivsuse nimel"
2. **Cozy Classic** → Medium Roast Drip - "Mugavus igas tassis"
3. **Sweet Enthusiast** → Caramel Latte - "Elu on liiga lühike kibedale"
4. **Zen Minimalist** → Black Coffee, Single Origin - "Lihtne. Puhas. Täiuslik."
5. **Social Butterfly** → Cappuccino - "Kohv on parem koos seltskonnaga"
6. **Night Owl** → Red Eye (coffee + espresso shot) - "Uni on valikuline"
7. **Health Nut** → Oat Milk Americano - "Heaolu igas lonkus"
8. **Artisan Snob** → Pour-Over, Single Origin - "Sa tead, mis sulle meeldib"
9. **Practical Pragmatist** → Large Drip, Whatever's Fresh - "Las töötab ja kõik"
10. **Indulgent Treat** → Mocha with Whip - "Kohv on dessert"

STOP: Kirjuta numbrid, mida tahad (nt "1, 3, 5, 8")

USER: [Types numbers]

ACTION: Note their selections for use in REQUIREMENTS.md

---

Suurepärane! Nüüd peame välja mõtlema "loogika".

Loogika on kulisside taga olevad reeglid, kuidas miski töötab. Kui kasutajad teevad X, mis juhtub? Kui nad sellele vajutavad, mida nad näevad? See on su toote "kui see, siis too".

Igal rakendusel, veebilehel ja tööriistal on loogika. Midagi planeerides tuleb alati läbi mõelda, kuidas see tegelikult käituma peaks. Ma saan aidata sul variante välja mõelda.

Nii see viktoriin töötab: igal küsimusel on vastused ja iga vastus seostub ühe su isiksusega. Lõpus loeme kokku, millist isiksust kõige rohkem valiti.

Küsimus on: kuidas me tulemust näitame? Kaks varianti:

**Variant A: Üks soovitus** – "Sa oled Bold Adventurer! Proovi meie Double Espresso't."

**Variant B: Näita kõiki protsente** – "Sa oled 50% Bold Adventurer, 30% Cozy Classic, 20% Sweet Enthusiast" koos kõigi kohvisoovitustega.

STOP: Kumba eelistad – üks soovitus (A) või kõik protsendid (B)?

USER: [Responds A or B]

ACTION: Note their choice for REQUIREMENTS.md

Hea valik! Nii et kui kellegi vastused seostuvad "Bold Adventurer'iga" 3 korda ja "Cozy Classic'uga" 2 korda:

[If they chose A]: Nad saavad "Sa oled Bold Adventurer! Sinu kohv: Double Espresso."

[If they chose B]: Nad näevad kõiki oma tulemusi protsentidega ja saavad uurida kõiki kohvisoovitusi.

Küsimused lihtsalt paljastavad, milline isiksus neile kõige paremini sobib.

STOP: Saad aru?

USER: Yes

---

Nüüd tuleb lõbus osa – kuidas see VÄLJA peaks NÄGEMA?

Ma genereerin mõned erinevad visuaalsed stiilid eelvaadetena ja avan need su brauseris.

STOP: Valmis stiilivariante nägema?

USER: Yes

ACTION: Generate 3-4 HTML style preview files with different aesthetics:
- Style 1: Playful/colorful (bright colors, rounded shapes, fun fonts)
- Style 2: Minimal/clean (lots of whitespace, simple typography)
- Style 3: Bold/dramatic (dark backgrounds, high contrast, strong typography)
- Style 4: Warm/cozy (earth tones, soft gradients, inviting feel)

Each preview should show a sample quiz card with a question and answer options. Save them to the quiz-project folder as style-preview-1.html, style-preview-2.html, etc.

ACTION: Open all preview files in the browser using bash open commands

Vaata neid eelvaateid oma brauseris. Iga tab on erinev stiil.

STOP: Milline stiil sulle kõige rohkem meeldib? Sa võid valida ühe või öelda, mida segada – näiteks "#2 värvid, aga #3 paigutus"

USER: [Responds with preference]

ACTION: Note their style preference. If they want to mix elements, clarify what specifically they want combined.

---

Veel üks visuaalne küsimus: kas sa tahad oma viktoriiini pilte?

Sul võiks olla pilt iga kohvitulemuse juures – näiteks foto espressost "Bold Adventurer'i" jaoks.

Ma saan veebist otsida ja pilte alla laadida – aga pane tähele, see võtab natuke aega, sest ma pean otsima, leidma head pildid ja need alla laadima.

Teise variandina saame pildid praegu vahele jätta ja need hiljem lisada, kui viktoriin juba töötab.

STOP: Kumba eelistad – pildid (võtab kauem) või jätame praegu vahele?

USER: [Responds]

ACTION: Based on their choice:

If they want IMAGES:
- Ask what images they want for each result (e.g., "espresso shot", "cozy latte", "iced coffee")
- For each image:
  1. Web search for the image (e.g., "espresso shot unsplash")
  2. Fetch a result page to find direct image URLs
  3. Download using curl to public/ folder in quiz-project
- Note: Unsplash is best for stock photos (free, high quality).

If they want to SKIP:
- Move on - can always add images later during iteration

---

Veel üks asi: kas sa tahad vastuste kõrvale ikoone? Näiteks väikest mõõgaikooni "Gryffindor'i" või kuud "Öönägemise" kõrvale?

Ikoonid teevad viktoriini viimistletumaks ja visuaalsemaks, aga saame hoida ka ainult teksti, kui eelistad puhtamat ilmet.

STOP: Ikoonid või ilma?

USER: [Responds]

ACTION: Note their choice for REQUIREMENTS.md

---

Viimane osa – tegelikud küsimused, millele inimesed vastavad.

Sa valisid "[their vibe choice from earlier]" stiilis küsimused, nii et ma genereerin 5–7 küsimust, mis sellele vibele vastavad. Igal küsimusel on vastused, mis seostuvad su erinevate isiksustega.

Muidugi saad alati ka ise küsimusi välja mõelda – lihtsalt ütle mulle, mida sa tahad, ja ma teen selle teoks.

ACTION: Generate 5-7 quiz questions matching their vibe choice:
- If "Fun pop culture": Harry Potter houses, Netflix shows, fictional characters, movie genres, etc.
- If "Lifestyle & preferences": weekend activities, travel styles, food choices, social preferences, etc.
- If "Abstract & quirky": colors, hypothetical scenarios, random objects, desert island choices, etc.
- If "Mix of everything": 2-3 from each category

Each question should have answers that clearly map to the personalities they selected. For example, if they picked Bold Adventurer and Cozy Classic, answers should lean toward intensity vs. comfort.

Siin on minu ettepanekud. Vaata üle – iga vastus on mõeldud seostuma ühe su isiksusega.

STOP: Mis arvad? Sobib nii, tahad muudatusi või tahad ise kirjutada?

USER: [Approves or suggests changes]

ACTION: Adjust questions based on feedback. If they want to write their own, help them map answers to personalities.

---

Suurepärane! Meil on kõik olemas. Lasen salvestada selle kõik nõuete faili.

ACTION: Create REQUIREMENTS.md in the quiz-project folder with:
- Personality→Coffee pairings (all selected ones with taglines)
- Result display style (single or percentages)
- Visual style description
- Image/icon decision
- All quiz questions with answer-to-personality mappings

Valmis! Ava REQUIREMENTS.md ja vaata üle. See on spetsifikatsioon, millelt ma ehitan.

STOP: Kas kõik tundub õige?

USER: Yes / [Corrections]

ACTION: Make any corrections if needed

---

**Mida sa just õppisid:** Kuidas defineerida selged nõuded enne ehitamist – konkreetselt soovitusmootori jaoks.

**Kus seda veel kasutada saab:**
- Disainerile või arendajale mis tahes projekti briifimine
- Toote spetsifikatsiooni või PRD kirjutamine
- Mis tahes loomingulise projekti planeerimine – mida selgem visioon, seda parem tulemus
- Tehisintellekti tööriistadega töötamine – mida täpsem oled, seda parem väljund

**Järgmisena:** Tunnis 2.3 me tegelikult EHITAME selle asja. Sa vaatad, kuidas ma su viktoriini nende nõuete põhjal nullist loon. Siin juhtub maagia.

STOP: Valmis tunniks 2.3? Ütle "ehitame" või kirjuta /start-2-3

USER: Let's build

---

## Olulised märkmed Claude'ile

- AskUserQuestion tööriista tuleks kasutada AINULT esialgsete koondküsimuste jaoks – pärast seda kasuta tavalist vestlust
- Stiilinäidete genereerimisel tee need päriselt visuaalselt erinevaks – ära muuda lihtsalt värve natuke
- Piltide jaoks: Unsplash töötab suurepäraselt fotode jaoks, aga kontrolli alati, et URL tegelikult pildi tagastab, enne allalaadimist
- Fail REQUIREMENTS.md on ülioluline – see on tunni 2.3 spetsifikatsioon. Veendu, et see on täielik ja selge.
- Kui kasutajad tahavad stiile segada, uuri konkreetselt, milliseid elemente igast
- Kohanda küsimuste arvu vastavalt paaringute arvule (rohkem paaringuid = rohkem küsimusi vaja eristamiseks)

## Edukriteeriumid

- Kasutaja on valinud oma isiksus→kohv paaringud
- Kasutaja on valinud tulemuse kuvamise stiili (üksik vs protsendid)
- Kasutaja on valinud visuaalse stiili
- Kasutaja on teinud otsuse piltide/ikoonide/vahelejätmise kohta
- Kasutaja on heaks kiitnud viktoriini küsimused
- REQUIREMENTS.md on olemas ja kõik ülaltoodu on dokumenteeritud
- Kasutaja on põnevil ehitama
