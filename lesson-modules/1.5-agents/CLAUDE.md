# Tund 1.5: Agendid

Mäletad neid konkurentide faile, vanu kampaaniaid ja CSV-d, mida me nägime, aga ei puutunud? Need kõik on kaustas `inherited-chaos/` - vaata üle, kui on vaja meelt värskendada.

Nüüd tegeleme nendega.

Siin läheb asi põnevaks.

STOP: Valmis KÕIKE korraga töötlema?

USER: Yes

---

## Suur Paljastus - Paralleeltöötlus

**Suur Paljastus:** Meil on 10 vana kampaaniafaili, mida analüüsida.

Tavaliselt loeksid sa need ükshaaval läbi. See võtaks igaviku. Isegi minul läheks tükk aega.

Selle asemel saan ma käivitada 10 agenti - 10 iseseisvat koopiat iseendast - ja töödelda KÕIKI samaaegselt.

Mõtle sellest nagu enda kloonimisest. Annan igale kloonile oma ülesande. Kõik kloonid töötavad samal ajal.

Seejärel kombineerin nende tulemused.

STOP: See on üks võimsamaid funktsioone Claude Code'is. Ülesanded, mis käsitsi võtaksid tunde - või kümneid ChatGPT vestlusi - juhtuvad sekunditega. Valmis seda tegevuses nägema?

USER: Yes

---

## Otsustusviktoriin

STOP: Kiire viktoriin - millal peaksid agente kasutama? A) Üks keeruline ülesanne, või B) Palju sarnaseid ülesandeid?

USER: B / Many similar tasks

Täpselt! Agendid on paralleelitavate tööde jaoks - palju sarnast, mida saab iseseisvalt teha.

STOP: Valmis seda tegevuses nägema?

USER: Yes

---

## Kampaaniapäästmine - 10 Agenti

Alustame 10 vana kampaaniaga.

STOP: Palu mul kasutada agente, et analüüsida kõiki faile kaustas @inherited-chaos/old-campaigns/ ja selgitada välja, millised kampaaniaideed on päästmist väärt. Loon igaühe jaoks eraldi agendi ja seejärel kombineerin nende tulemused.

USER: Types command about analyzing campaigns

ACTION: Launch agents to analyze each of the 10 campaign files in parallel. Synthesize results into analysis/campaign-salvage-report.md with findings about each campaign.

**Avastus:** Eelmine juht proovis pidevalt kaasatuse taktikaid, aga need kõik olid tehingupõhised (topeltpunktid, boonuspreemiad). Mitte midagi identiteedi ega kuuluvuse kohta. Iga kampaania püüdis saada ROHKEM TEHINGUID, mitte panna inimesi midagi TUNDMA.

STOP: See just juhtus paralleelselt. 10 faili, analüüsitud samaaegselt, sünteesitud üheks raportiks. Kujuta ette, et teed seda 100 kliendintervjuuga või terve aasta koosolekute märkmetega. Siin hakkab Claude Code tunduma nagu supervõime. Valmis lisaks?

USER: Yes

---

## Edasijõudnud: Ristallika-analüüs

Nüüd teeme midagi edasijõudnumat. Oleme analüüsinud kampaaniaid ja konkurente eraldi. Ühendame nüüd punktid.

Kasutame 4 agenti, igaüks teeb midagi ERINEVAT:

- **Agent 1:** Analüüsi liikmete andmete CSV-d - mida numbrid meile ütlevad?
- **Agent 2:** Ristkontrolli konkurentide tugevusi meie läbikukkunud kampaaniatega - mida nemad teevad, mida meie proovisime ja ebaõnnestusime?
- **Agent 3:** Ühenda klientide tagasiside teemad konkurentide ülevaadetega - kas kliendid küsivad asju, mis konkurentidel juba olemas on?
- **Agent 4:** Tuvasta lüngad - mis töötab mujal, aga mida meie pole veel proovinudki?

Seejärel sünteesime kõik üheks tervikpildiks.

STOP: Palu mul kasutada 4 agenti: analüüsida liikmete andmete CSV-d, ristkontrollida konkurentide tugevusi meie kampaaniatega, ühendada klientide tagasiside konkurentide funktsioonidega ja tuvastada lüngad. Seejärel sünteesida kõik kokku.

USER: Types command for the 4-agent analysis

ACTION: Launch 4 specialized agents:
1. Analyze member-data-summary.csv for trends
2. Compare competitor research to our failed campaigns
3. Connect feedback themes to competitor features
4. Identify gaps in our approach

Synthesize everything into analysis/comprehensive-research-synthesis.md

**Avastused:**
- CSV näitab, et inimesed registreeruvad, käivad 2-3 korda, siis kaovad. Nad ei lahku vihaselt - nad lahkuvad ükskõikselt.
- Konkurentidel, kellel on isikupära-funktsioonid, on 3x parem hoidmine kui ainult punktipõhistel programmidel.
- Kliendid küsivad pidevalt "midagi enamat", aga ei oska sõnastada, mida täpselt.
- Lünk: mitte keegi meie turul pole proovinud isikupõhist lähenemist.

STOP: Näed, kuidas erinevate allikate ühendamine paljastab asju, mida eraldi vaadates ei märkaks?

USER: Yes

---

## Põhiavastus

Ühendades selle üldise looga:

**PÕHIAVASTUS:** "Programmil puudub isikupära. See on tehingupõhine. Liikmed ei osale, sest pole millega osaleda. Punktidest ei piisa - inimesed vajavad identiteeti, kuuluvust, põhjust hoolida."

See ühendub tagasi seemnega tunnist 1.3: "kohviisiksused"... see pooltoores idee hakkab mõtet andma.

STOP: Kas sa näed seda? Programm vajab ISIKUPÄRA.

USER: Yes

---

## Agentide Otsustusraamistik

Nii et millal peaksid agente kasutama?

**Kasuta agente, kui:**
- Sul on palju sarnaseid faile
- Paralleelitavad ülesanded
- Uurimistöö mitme allika lõikes

**Ära kasuta agente, kui:**
- Sul on üks keeruline ülesanne
- Järjestikune töö
- Asjad, mis sõltuvad üksteisest

STOP: Mõttemudel: kui sa saaksid anda samad juhised 10 praktikandile ja lasta igaühel iseseisvalt töötada, on agendid ideaalsed. Kui töö nõuab edasi-tagasi suhtlust või iga samm tugineb eelmisele, jää tavalise vestluse juurde. Selge?

USER: Yes

---

## Kokkuvõte

**Metaoskus:** Paralleeltöötlus - paljude sarnaste ülesannete samaaegne käsitlemine ühekaupa tegemise asemel.

**Millal agente kasutada:** Sul on mitu sarnast asja, mis vajavad samatüübilist analüüsi. Töö on paralleelitav - iga osa saab teha iseseisvalt.

**Kus seda veel kasutada:**
- 10 tööpakkumist ametikohtade jaoks, mida kaalud - analüüsi kõiki korraga, võrdle nõudeid
- 5 tarnijat, keda hindad - uuri igaüht paralleelselt, sünteesi võrdluseks
- 20 artiklit, mis oled lugemiseks salvestanud - lase agentidel igaüks kokku võtta, siis sünteesi peamised oivamused
- Korteriotsing - 8 kuulutust, mida analüüsida plusside/miinuste/ohumärkide suhtes samaaegselt
- Konkurentsianalüüs - uuri 6 konkurenti korraga, mitte ükshaaval
- Reisi planeerimine - agendid uurivad lende, hotelle, tegevusi, restorane kõiki korraga

**Järgmisena:** Tunnis 1.6 kohtud oma nõuandemeeskonnaga. Kohandatud alamagendid erinevate vaatenurkadega - juht, disainer, eesliini töötaja - igaüks annab sulle tagasisidet oma vaatenurgast. Siin selgitame välja, mida lojaalsusprogrammi probleemiga tegelikult ETTE VÕTTA.

STOP: Valmis tunniks 1.6?

USER: Yes / /start-1-6

---

## Olulised Märkmed Claude'ile

- **Kasuta tegelikult agente**: Ära teeskle paralleeltöötlust - käivita päriselt mitu agenti
- **Loo päris failid**: campaign-salvage-report.md ja comprehensive-research-synthesis.md tuleb luua kausta analysis/
- **Põhiavastuse rõhutamine**: Veendu, et "isikupära puudumine" ülevaade jõuab selgelt kohale
- **Kohviisiksuse tagasiviide**: Viita selgesõnaliselt tagasi ideele failist previous-manager-notes.md

## Edukriteeriumid

- [ ] Õpilane nägi 10 agenti kampaaniaid paralleelselt töötlemas
- [ ] Õpilane nägi 4 spetsialiseeritud agenti tegemas ristallika-analüüsi
- [ ] Õpilane mõistab, millal agente kasutada (paralleelsed, sarnased ülesanded)
- [ ] Õpilane mõistab, millal MITTE agente kasutada (järjestikused, sõltuvad ülesanded)
- [ ] Õpilane haaras põhiavastuse: "programmil puudub isikupära"
- [ ] Õpilane nägi kohviisiksuse idee taas esile kerkimas
- [ ] analysis/campaign-salvage-report.md loodud
- [ ] analysis/comprehensive-research-synthesis.md loodud
- [ ] Õpilane on valmis tunniks 1.6
