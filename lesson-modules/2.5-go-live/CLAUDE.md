# 2.5 Ellu minek

Nii, see on see. Viimane samm.

Su viktoriin on ehitatud, lihvitud ja GitHub'i salvestatud. Nüüd paneme selle internetti, et igaüks saaks seda külastada.

Arendajad nimetavad seda "deploy'miseks" – sa deploy'd oma rakenduse veebi. Sa kuuled seda sõna palju.

STOP: Valmis ellu minema?

USER: Yes

---

Vercel on tasuta teenus, mis paneb su koodi internetti.

See on põhimõtteliselt vibecoding'u kodukants.

Sa annad sellele oma GitHub'i projekti ja see muudab selle päris veebileheks päris URL-iga.

Selle tegid samad inimesed, kes tegid Next.js (raamistik, mida me kasutasime), nii et need töötavad ideaalselt koos.

STOP: Kõlab hästi?

USER: Yes

---

Kõigepealt on sul vaja Vercel'i kontot.

STOP: Kas tahad, et ma avaksin vercel.com sulle? Soovitan registreeruda oma GitHub'i kontoga – nii ühendub kõik automaatselt.

USER: Yes / I'll do it myself

ACTION: If they want it opened, run: `open https://vercel.com`

STOP: Anna mulle teada, kui oled konto loonud. Veendu, et registreerud GitHub'iga!

USER: Done

---

Nagu GitHub'i puhul, laadin ma alla tööriistad, mis lasevad mul otse Vercel'iga töötada.

See avab su brauseri sisselogimiseks – lihtsalt järgi juhiseid.

ACTION: Set up Vercel CLI:

1. Check if already installed:
```
vercel --version
```

2. If NOT installed:
```
npm i -g vercel
```

3. Once installed, authenticate (run in background to avoid blocking):
```bash
vercel login > /tmp/vercel-auth.log 2>&1 &
sleep 3
cat /tmp/vercel-auth.log
```

4. Read the output to get the device URL with code, then open it:
```bash
open "https://vercel.com/oauth/device?user_code=[CODE FROM OUTPUT]"
```

5. Tell user: "I just opened Vercel in your browser. Click Authorize, then let me know when you're done."

STOP: Anna mulle teada, kui oled autoriseerinud.

USER: Done

ACTION: Verify authentication worked:
```bash
vercel whoami
```

If successful, continue. If not authenticated, troubleshoot:
- They may not have completed the browser flow - ask them to try again
- The background process may have timed out - run the login command again

---

Nüüd paneme su viktoriini internetti.

ACTION: Deploy to Vercel:

1. Navigate to the quiz-project folder:
```
cd [path to quiz-project]
```

2. Deploy to production:
```
vercel --prod --yes
```

Lipp `--yes` aktsepteerib kõik vaikeväärtused, et sa ei peaks küsimustele vastama. Lipp `--prod` tähendab, et see läheb kohe ellu.

Oota, kuni deploy lõpeb – see võtab umbes minuti. Jälgi väljundis URL-i.

Vercel ehitab su viktoriini ja paneb seda praegu internetti...

Valmis! Otsi väljundist URL-i – see näeb välja umbes nii: `quiz-project-abc123.vercel.app`.

---

Su URL on: [Copy the URL from the deploy output]

See on SINU veebileht. Päris internetis. Igaüks saab seda külastada.

Avan selle sulle.

ACTION: Open the deployed URL in the browser using bash open

STOP: Kas sa näed oma viktoriini päriselt internetis?

USER: Yes!

---

Ava see URL oma telefonis. See peaks ka seal töötama – sama viktoriin, mis tahes seadmel.

STOP: Kas see töötab su telefonis?

USER: Yes!

---

Nüüd tuleb päris test: saada see link sõbrale. Saada see kellelegi kohe. Kui nad reageerivad, siis see ongi see tunne, kui sa midagi päriselt välja lased.

Tunnistame, mis just juhtus.

Sa ehitasid päris veebirakenduse. Sa panid selle internetti. Sul on URL, mis töötab igal seadmel. Sa tegid seda ilma ühtegi koodirida ise kirjutamata.

See ongi vibecoding. See on tulevik.

STOP: Kuidas see tundub?

USER: [Response]

---

Nii, siin on, mida sa nüüd tead:

**Planeeri** → Tee selgeks, mida sa ehitad
**Ehita** → Lase tehisintellektil see luua
**Iteeri** → Lihvi, kuni on õige
**Salvesta** → Varunda GitHub'i
**Mine ellu** → Pane internetti (deploy)

See ongi tsükkel. Sa saad selle tsükliga ehitada mida iganes.

STOP: Selge?

USER: Yes

---

Veel üks asi: mis siis, kui sa tahad oma viktoriini hiljem uuendada?

Siin on voog: tee muudatused oma arvutis, palu mul "push'i GitHub'i" ja Vercel uuendab automaatselt su elus veebilehte.

See on kõik. Vercel jälgib su GitHub'i ja deploy'b automaatselt, kui sa muudatusi push'id. Maagia.

STOP: Päris lahe, jah?

USER: Yes

---

Mis siis, kui sa tahaksid koguda emaile inimestelt, kes viktoriini teevad? Selleks oleks vaja andmebaasi nende salvestamiseks. See on tulevane moodul.

Mis siis, kui sa tahaksid veenduda, et see ei lähe katki? Selleks oleks vaja testimist. Ka tulevane moodul.

Mis siis, kui sa tahaksid kohandatud domeeni nagu suviktoriin.com? Täiesti teostatav – Vercel teeb selle lihtsaks.

Mõte on: sul on nüüd vundament olemas. Kõik muu ehitub sellele peale.

STOP: Tunned end võimekana?

USER: Yes

---

Tahad midagi muud ehitada? Loo uus projekti kaust ja järgi sama protsessi.

Peamised asjad, mida Claude'ile öelda: sa tahad Vercel'ile deploy'da ja et tal on ligipääs Vercel CLI-le. Ta teab, mida teha.

STOP: Mõtteid haudumas?

USER: [Response]

---

## Kiired soovitused

**Tulevaste moodulite jaoks:** Telli Claude Code for Everyone uudiskiri aadressil ccforeveryone.com. Seal leiad ka põhjalikke juhendeid ja kogukonna mittetehnilisi Claude Code kasutajaid nagu sina ise.

STOP: Kas tahad, et ma avaksin selle saidi, et saaksid tellida?

USER: Yes / No

ACTION: If yes, open https://ccforeveryone.com in browser

Selle kursuse lõi Carl Vellotti. Kui sul on tagasisidet, küsimusi või tahad lihtsalt tere öelda, ta kuulab alati hea meelega: [X](https://x.com/carlvellotti) / [LinkedIn](https://www.linkedin.com/in/carlvellotti/)

Kui sulle meeldis, jaga seda sõprade ja kolleegidega, kes võiksid neid oskusi kasutada!

---

**Moodul 2 läbitud!**

Sa läksid nullist deploy'tud veebirakenduseni. Sa õppisid planeerimist, ehitamist, itereerimist, GitHub'i ja ellu minemist.

See on vibecoding. See on su uus supervõime.

**Mis edasi:** Tulevased moodulid käsitlevad andmebaase, API-sid, keerukamaid rakendusi ja Claude'i ühendamist kõigega. Aga sul on nüüd põhioskus käes – sa oskad asju ehitada ja välja lasta.

Vahepeal proovi ise midagi ehitada. Parim viis õppida on teha midagi, mida sa päriselt tahad.

STOP: Aitäh, et koos ehitasime. Nüüd mine ja tee midagi ägedat.

USER: (exits or explores)

---

## Olulised märkmed Claude'ile

- **CC4PMs versiooni jaoks:** Muuda ccforeveryone.com → ccforpms.com
- Lipud `vercel --prod --yes` on kriitilised – `--yes` jätab kõik interaktiivsed küsimused vahele, `--prod` deploy'b kohe toodangusse
- Vercel ühendub automaatselt GitHub'i repoga, mille nad tunnis 2.4 lõid – seepärast oli GitHub'iga registreerumine oluline
- URL-i formaat on tavaliselt `[projekti-nimi]-[suvaline].vercel.app`
- Automaatne deploy seadistatakse automaatselt, kui nad ühendavad GitHub'i Vercel'i registreerumise ajal
- Kui deploy ebaõnnestub, levinud probleemid:
  - Ehitusvead → Kontrolli Vercel'i juhtpaneelilt logisid
  - Pole õiges kaustas → Veendu, et oled quiz-project'is
- Tähistamise hetk (sõbrale saatmine) on ülioluline – lase sel hingata, ära kiirusta sellest üle

## Edukriteeriumid

- Kasutajal on Vercel'i konto (ühendatud GitHub'iga)
- Vercel CLI on paigaldatud ja autenditud
- Viktoriin on deploy'tud ja elus internetis
- Kasutaja pääseb viktoriiinile ligi oma telefonist
- Kasutaja on lingi vähemalt ühele inimesele saatnud
- Kasutaja mõistab tsüklit: Planeeri → Ehita → Iteeri → Salvesta → Mine ellu
- Kasutaja teab, kuidas uuendada: tee muudatused → push'i GitHub'i → deploy'b automaatselt
- Kasutaja tunneb end võimekana rohkem asju ehitama
