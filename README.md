# TILs nella mammella · Atlante pratico
### TILs in breast cancer · Practical atlas

**🇮🇹 Italiano** · [🇬🇧 English below](#english)

Web app per la valutazione dei **linfociti infiltranti lo stroma (sTILs)** nel carcinoma mammario secondo le raccomandazioni dell'**International Immuno-Oncology Biomarker Working Group**.

👉 **https://infingardo.github.io/TILS/**

## Cosa contiene

| Sezione | Contenuto |
|---|---|
| **Guida rapida** | Definizione degli sTILs, i tre passaggi (delimita, seleziona, stima), esclusioni, requisiti del campione |
| **Referto e checklist** | Checklist in cinque punti prima della firma; generatore della frase di referto per pezzo operatorio, biopsia, malattia residua post-neoadiuvante e carcinoma in situ, con i limiti da segnalare |
| **Quando refertare** | Rilevanza per sottotipo (triplo negativo, HER2+, luminale), formato del dato, assenza di cut-off clinici validati |
| **Neoadiuvante e in situ** | Regole operative per la malattia residua (letto tumorale residuo come nell'RCB) e per il carcinoma in situ (stroma periduttale, regola dei 2 campi ad alto ingrandimento) |
| **Esercizio alla cieca** | Immagine di riferimento casuale: stima, poi confronto con il valore del Working Group (tolleranza ±10 punti, scarto medio) |
| **Confronto immagini** | Il tuo campo affiancato a un riferimento 0–80%; la foto resta sul dispositivo |
| **Pitfalls** | Intraepiteliali, fronte d'invasione, carcinoma in situ, necrosi, hotspot, imitatori, denominatore |
| **Fonti** | Salgado 2015, Dieci 2018, Denkert 2016, Loi 2019, Leon-Ferre 2024, El Bairi 2021 |

## Uso

- **Bilingue** italiano/inglese: selettore in alto a destra; la scelta viene ricordata. Link diretto in inglese: `?lang=en`.
- **Installabile** come app (Chrome su Android e desktop: menu › *Installa app*; Safari su iOS: Condividi › *Aggiungi alla schermata Home*).
- **Funziona offline**: tutto, immagini comprese, è in un unico file `index.html`.
- Nessun dato inviato a server: le foto caricate per il confronto restano nel browser.

## Struttura del repository

```
index.html              pagina unica (HTML + CSS + JS, immagini incorporate in base64)
manifest.webmanifest    manifest della web app
sw.js                   service worker (cache offline)
icon-*.png, apple-touch-icon.png   icone
```

## Limiti

Strumento di consultazione e formazione, **non è un dispositivo medico** e non calcola lo score dalle immagini. Gli sTILs sono un dato prognostico: non esistono soglie validate per decisioni terapeutiche sul singolo paziente.

## Crediti

Metodo e immagini di riferimento 0–80%: International Immuno-Oncology Biomarker Working Group on Breast Cancer — [tilsinbreastcancer.org](https://www.tilsinbreastcancer.org/). Le immagini restano di proprietà dei rispettivi autori. Progetto indipendente, non affiliato al Working Group.

Autore: **Dr Filippo Bianchi** — SC Anatomia Patologica Fatebenefratelli, Melloni e Territorio, ASST Fatebenefratelli-Sacco, Milano.

---

<a id="english"></a>
## 🇬🇧 English

A web app for scoring **stromal tumour-infiltrating lymphocytes (sTILs)** in breast cancer according to the **International Immuno-Oncology Biomarker Working Group** recommendations.

👉 **https://infingardo.github.io/TILS/?lang=en**

### Contents

| Section | What it does |
|---|---|
| **Quick guide** | sTILs definition, the three steps (delineate, select, estimate), exclusions, specimen requirements |
| **Report & checklist** | Five-point sign-out checklist; report sentence builder for resections, core biopsies, post-neoadjuvant residual disease and carcinoma in situ, with limitations |
| **When to report** | Relevance by subtype (triple-negative, HER2+, luminal), reporting format, no validated clinical cut-offs |
| **Neoadjuvant & in situ** | Practical rules for residual disease (residual tumour bed as in RCB) and carcinoma in situ (periductal stroma, 2 high-power field rule) |
| **Blind exercise** | Random reference image: estimate first, then compare with the Working Group value (±10-point tolerance, mean difference) |
| **Image comparison** | Your field side by side with a 0–80% reference; the photo never leaves the device |
| **Pitfalls** | Intraepithelial TILs, invasive edge, in situ carcinoma, necrosis, hotspots, mimics, denominator |
| **Sources** | Salgado 2015, Dieci 2018, Denkert 2016, Loi 2019, Leon-Ferre 2024, El Bairi 2021 |

### Usage

- **Bilingual** Italian/English with a switch in the top-right corner; the choice is remembered. Direct English link: `?lang=en`.
- **Installable** as an app (Chrome on Android/desktop: menu › *Install app*; Safari on iOS: Share › *Add to Home Screen*).
- **Works offline**: everything, images included, lives in a single `index.html`.
- No data is sent to any server: photos loaded for comparison stay in the browser.

### Disclaimer

A reference and training tool, **not a medical device**; it does not compute scores from images. sTILs are a prognostic biomarker: there are no validated thresholds for treatment decisions in individual patients.

### Credits

Method and 0–80% reference images: International Immuno-Oncology Biomarker Working Group on Breast Cancer — [tilsinbreastcancer.org](https://www.tilsinbreastcancer.org/). Images remain the property of their authors. Independent project, not affiliated with the Working Group.

Author: **Dr Filippo Bianchi** — Pathology Department, Fatebenefratelli, Melloni e Territorio, ASST Fatebenefratelli-Sacco, Milan, Italy.
