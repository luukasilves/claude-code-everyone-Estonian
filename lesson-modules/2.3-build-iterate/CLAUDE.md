# 2.3 Ehitamine ja itereerimine

Nii, see on see hetk. Aeg ehitada su viktoriin.

Ma hoolitsen kogu tehnilise seadistuse eest. Sina lihtsalt vaata, kuidas maagia sünnib.

STOP: Valmis?

USER: Yes

---

Kõigepealt pean ma projekti struktuuri üles seadma – see loob kõik algusfailid, mida meil vaja läheb.

ACTION: Run the following command in the quiz-project folder:
```
npx create-next-app@latest . --typescript --tailwind --eslint --app --no-src-dir --import-alias "@/*" --yes
```
(The --yes flag accepts all defaults automatically)

Valmis! Vaata oma failiuurijat – sa peaksid nägema hunnikut uusi faile kaustas quiz-project.

Ära muretse nende kõigi mõistmise pärast. Kaust `app/` on koht, kus su viktoriin elab. Kõik muu on lihtsalt konfiguratsioon.

STOP: Kas sa näed uusi faile?

USER: Yes

---

Enne ehitamist näitan sulle üht kasulikku asja: planeerimisrežiim.

Suurte ülesannete puhul on kasulik näha, mida ma kavatsen teha, enne kui ma seda teen. Vajuta **Shift+Tab**, et režiime vahetada – sa peaksid nägema valikut "Plan mode".

STOP: Lülitu planeerimisrežiimi ja anna mulle teada, kui oled kohal.

USER: In plan mode

Suurepärane. Planeerimisrežiim tähendab, et ma näitan sulle oma plaani, sina kiidad selle heaks, siis ma viin selle ellu. Teeme nii.

STOP: Palu mul ehitada viktoriin nõuete põhjal.

USER: Build my quiz based on REQUIREMENTS.md

ACTION: Read REQUIREMENTS.md, then create a plan showing:
- Components to create (quiz page, question component, results page)
- Styling approach based on their chosen style
- Quiz logic implementation (how answers map to results)
- Any images/icons to include

Present the plan clearly with bullet points.

Siin on minu plaan. Ma loon viktoriinilehe, küsimuste komponendid, tulemuste lehe ja kujundan kõik vastavalt su eelistustele.

STOP: Kas see tundub õige? Küsimusi, enne kui alustan?

USER: Looks good / [Questions]

ACTION: Answer any questions they have, then tell them to switch back to normal mode (Shift+Tab) and you'll execute the plan.

---

Ehitan nüüd. See võtab minuti-paar. Sa näed, kuidas ma faile loon ja muudan. Lase mul lihtsalt töötada.

ACTION: Build the full quiz application based on REQUIREMENTS.md:
1. Create the main quiz page in app/page.tsx
2. Create quiz components (QuizQuestion, Results, etc.)
3. Implement the quiz logic (tracking answers, calculating results)
4. Apply the visual style they chose
5. Add any images/icons based on their preference
6. Make sure the result display matches their choice (single vs percentages)

Take your time and build it properly. This is the core deliverable.

Valmis! Su viktoriin on ehitatud. Vaatame seda nüüd tegevuses.

---

Panen su viktoriini tööle ja avan selle brauseris.

ACTION: Run `npm run dev` in background in the quiz-project folder

ACTION: Wait a few seconds for the server to start, then bash open http://localhost:3000 in browser

Su viktoriin peaks nüüd brauseris avatud olema!

See "localhost" link töötab ainult SINU arvutis – see on ajutine lokaalne versioon. Teeme selle hiljem avalikuks, kui me deploy'me.

STOP: Kas sa näed oma viktoriini?

USER: Yes! / [Issues]

ACTION: If they have issues:
- Browser didn't open → Tell them to manually go to http://localhost:3000
- Build errors → Check the terminal output, fix errors
- Blank page → Check for JavaScript errors in browser console

---

Vaata seda! Sul on toimiv viktoriin!

Proovi seda läbi – vasta küsimustele ja vaata oma tulemust.

STOP: Proovi viktoriini. Kas see töötab? Kas sa saad lõpus tulemuse?

USER: Yes it works! / [Something's wrong]

ACTION: If something's wrong, debug together. Common issues:
- Result not showing → Check the logic implementation
- Wrong personality mapping → Review the answer mappings
- Style issues → Can fix in iteration

See on normaalne – esimesed versioonid vajavad tihti parandusi. Paneme kõigepealt tööle, siis lihvime.

Vinge! Sa just ehitasid veebirakenduse. Las see natuke kohale jõuab.

---

Esimene versioon pole kunagi täiuslik. Hakkame itereerima – teeme 2–3 muudatust, kuni sulle päriselt meeldib.

Üks nipp: sa saad teha ekraanipildi, kleepida selle siia **Ctrl+V**-ga (mitte Cmd+V Macil!) ja öelda mulle, mida muuta.

Tõmba millegi ümber ring, osuta sellele, mis iganes – lihtsalt näita mulle, mida tahad teisiti.

See on ka suurepärane viis mulle vigade näitamiseks. Kui miski tundub vale, tee ekraanipilt ja kleebi see siia.

Kui sa pole kindel, mida muuta, siin on mõned ideed:
- Lisa konfetid või animatsioon, kui saad tulemuse
- Muuda värve või fonte
- Kohenda küsimuste või tulemuste sõnastust
- Lisa pildid iga tulemuse juurde
- Muuda paigutust või vahesid
- Lisa edenemisriba

STOP: Tee oma viktoriiist ekraanipilt, kleebi see Ctrl+V-ga ja ütle mulle, mida tahaksid muuta.

USER: [Pastes screenshot and describes change]

ACTION: Make the requested change to the code

Valmis! Värskenda brauserit, et muudatust näha.

STOP: Kuidas on? Tahad veel midagi muuta?

USER: [More changes / Happy with it]

ACTION: Keep iterating until they're satisfied. 2-3 rounds is typical. Common requests:
- Visual tweaks (colors, spacing, fonts)
- Animation additions
- Wording changes
- Layout adjustments

---

Vaata seda – see on SINU viktoriin, täpselt nii, nagu sa tahtsid.

See ongi itereerimistsükkel: ekraanipilt → kirjelda → muuda → värskenda → korda.

Nii toimib päris tootearendus. Ja tehisintellektiga võtab iga iteratsioon sekundeid, mitte päevi.

STOP: Oled rahul, kuidas see välja näeb?

USER: Yes

---

**Mida sa just õppisid:** Kuidas minna nõuetest toimiva tooteni ja siis itereerida, kuni see on täpselt selline, nagu tahad.

**Kus seda veel kasutada saab:**
- Mis tahes veebiprojekti ehitamine – maandumislehed, tööriistad, prototüübid
- Ideede kiire testimine enne "päris" arendusse investeerimist
- Disainerite/arendajatega töötamine – selge visuaalne tagasiside kiirendab kõike

**Järgmisena:** Tunnis 2.4 salvestame su koodi GitHub'i. Praegu on see ainult su arvutis. Paneme selle pilve, et see oleks varundatud ja deploy'miseks valmis.

STOP: Valmis oma tööd salvestama? Ütle "teeme GitHub'i" või kirjuta /start-2-4

USER: Let's do GitHub

---

## Olulised märkmed Claude'ile

- Käsk `npm run dev` peaks jooksma taustal, et kasutaja saaks edasi rääkida
- localhost:3000 on Next.js vaikimisi port – kui midagi seda juba kasutab, Next.js soovitab teist porti
- Kui nad kleeibivad ekraanipilte, vaata neid päriselt ja tee konkreetseid muudatusi
- Ctrl+V märkus on oluline – Maci kasutajad proovivad tihti kõigepealt Cmd+V
- Hoia iteratsioonid fokusseeritud – ära paku korraga liiga palju muudatusi
- Kui viktoriinil on vigu, paranda need enne visuaalset lihvi
- Planeerimisrežiim (Shift+Tab) on päris Claude Code funktsioon – veendu, et nad seda ka päriselt kasutavad

## Edukriteeriumid

- Next.js projekt on kaustas quiz-project üles seatud
- Viktoriin on täielikult ehitatud vastavalt REQUIREMENTS.md-le
- Arendusserver jookseb ja viktoriin on vaadatav aadressil localhost:3000
- Kasutaja on teinud vähemalt 1–2 iteratsiooni
- Kasutaja on rahul, kuidas viktoriin välja näeb
- Kasutaja on valmis GitHub'i jaoks
