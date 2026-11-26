# Stiliaus gidas: Rytmetys

Čia surinkti visi dizainerio sprendimai: šriftai, spalvos, tarpai ir tai, kaip keičiasi išdėstymas skirtinguose ekranuose. Maketai (`maketai/`) rodo, kaip turi atrodyti rezultatas, o šis failas padeda jį atkartoti tiksliai.

**Maketų mastelis.** 1 paveikslėlio pikselis lygus 1 CSS pikseliui. Kompiuterio maketai yra 1440 px pločio, telefono maketai yra 390 px pločio. Dideli paveikslėliai patogiau žiūrėti dalimis: aplanke `maketai/dalys/` kiekviena sekcija yra atskirame faile. Būsenų pavyzdžiai (hover, fokusas, klaida) yra faile `maketai/busenos.png`.

**Matavimo vienetai.** 1 rem = 16 px. Šiame gide dydžiai rašomi pikseliais, o kode rekomenduojama naudoti `rem` ir `%`.

## 1. Šriftai

Abu šriftai yra iš Google Fonts. Įdėk šias eilutes į kiekvieno puslapio `<head>`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

| Paskirtis | Šriftas | Atsarginis šriftas |
| --- | --- | --- |
| Antraštės (`h1`, `h2`, `h3`) ir logotipo tekstas | DM Serif Display, svoris 400 | Georgia, serif |
| Visas kitas tekstas | Inter, svoriai 400, 500, 600, 700 | system-ui, sans-serif |

DM Serif Display turi tik vieną svorį (400), todėl antraštėms nustatyk `font-weight: 400`. Kitaip naršyklė jį dirbtinai paryškins ir antraštės atrodys kitaip nei makete.

## 2. Spalvos

| Pavadinimas | HEX | Kur naudojama |
| --- | --- | --- |
| Fonas | `#FFFBF2` | puslapio fonas, antraštė |
| Paviršius | `#F4ECDD` | sekcijų "Apie mus" ir "Galerija" fonas, lentelės antraštės eilutė, rezervacijos puslapio viršus |
| Tekstas | `#1E2A28` | pagrindinis tekstas, antraštės, poraštės fonas |
| Pritilęs tekstas | `#566561` | aprašymai, smulkus tekstas |
| Pagrindinė | `#0F5C4D` | mygtukai, kainos, nuorodos, kvietimo bloko fonas, lentelės pavadinimas |
| Pagrindinė tamsi | `#0A4237` | pagrindinių mygtukų hover |
| Akcentas | `#F2B632` | žymės, geltonas mygtukas, hover linija, varnelės |
| Akcentas tamsi | `#D99A14` | geltono mygtuko hover |
| Linija | `#E6DAC3` | kortelių, lentelės ir antraštės rėmeliai, skirtukai |
| Laukų rėmelis | `#8A9894` | formos laukų rėmelis |
| Klaida | `#B3261E` | neteisingai užpildyto lauko rėmelis |
| Balta | `#FFFFFF` | kortelės, formos fonas, tekstas ant žalio fono |
| Poraštės tekstas | `#C9D3CF` | poraštės nuorodos ir tekstas |
| Kvietimo bloko tekstas | `#E6F2EC` | aprašymas ant žalio fono |

Visi šie tekstų ir fonų deriniai turi pakankamą kontrastą (bent 4,5:1), todėl spalvų keisti nereikia. Rekomenduojama visas spalvas aprašyti CSS kintamaisiais.

## 3. Tipografija

| Elementas | Iki 767 px | Nuo 768 px | Nuo 1024 px | Papildomai |
| --- | --- | --- | --- | --- |
| `h1` | 36 px | 44 px | 56 px | DM Serif Display, eilutės aukštis 1,15 |
| `h2` | 28 px | 36 px | 40 px | tas pats šriftas ir eilutės aukštis |
| `h3` | 20 px | 20 px | 20 px | tas pats šriftas |
| Pagrindinis tekstas | 16 px | 16 px | 16 px | Inter 400, eilutės aukštis 1,6 |
| Hero įžanginis tekstas | 18 px | 18 px | 18 px | pritilęs tekstas, ne platesnis nei 544 px |
| Navigacijos nuorodos | 13 px | 15 px | 15 px | Inter 500 |
| Mygtukai | 16 px | 16 px | 16 px | Inter 600 |
| Antraštės eilutė virš `h1` | 13 px | 13 px | 13 px | Inter 600, didžiosios raidės, tarpai tarp raidžių 0,08 em, pagrindinė spalva |
| Kortelės aprašymas | 15 px | 15 px | 15 px | pritilęs tekstas |
| Žymė ant kortelės | 12 px | 12 px | 12 px | Inter 600 |
| Lentelės antraštės (`thead`) | 12 px | 12 px | 12 px | didžiosios raidės, tarpai tarp raidžių 0,06 em |
| Poraštės tekstas | 15 px | 15 px | 15 px | apatinė juosta 13 px |

## 4. Tarpai, kampai, šešėliai

| Dalykas | Reikšmė |
| --- | --- |
| Konteineris | didžiausias plotis 1120 px, centruotas; šoniniai tarpai 16 px (telefone) ir 32 px (nuo 768 px) |
| Sekcijų vertikalūs tarpai | 64 px (telefone), 80 px (nuo 768 px), 96 px (nuo 1024 px) |
| Sekcijos antraštės bloko apatinis tarpas | 40 px; blokas centruotas, ne platesnis nei 640 px |
| Kortelių tarpai | 24 px (telefone ir planšetėje), 32 px (nuo 1024 px) |
| Galerijos tarpai | 12 px (telefone), 16 px (nuo 768 px), 20 px (nuo 1024 px) |
| Kampų apvalinimas | 16 px: kortelės, paveikslėliai, lentelė, galerija; 12 px: formos laukai; visiškai apvalūs (pilulės formos): mygtukai, žymės, ženkliukas |
| Kortelės šešėlis | `0 2px 4px rgba(30, 42, 40, 0.04), 0 8px 24px rgba(30, 42, 40, 0.06)` |
| Kortelės šešėlis hover metu | `0 4px 8px rgba(30, 42, 40, 0.06), 0 16px 36px rgba(30, 42, 40, 0.12)` |
| Pereinamieji efektai | 0,2 s `ease`; paveikslėlių priartinimas 0,4 s |

## 5. Kaip keičiasi išdėstymas

Dirbk mobile-first: pirmiausia sukurk telefono vaizdą (390 px), o platesnius ekranus pridėk su `min-width` užklausomis. Makete naudojamos dvi ribos: **768 px** (planšetė) ir **1024 px** (kompiuteris).

| Dalis | Telefonas (iki 767 px) | Nuo 768 px | Nuo 1024 px |
| --- | --- | --- | --- |
| Antraštė | logotipas centre, po juo nuorodos vienoje eilutėje; "Rezervacija" yra paprasta paryškinta nuoroda | logotipas kairėje, nuorodos dešinėje; "Rezervacija" tampa pilnaspalviu mygtuku | tas pats |
| Hero | viena kolonėlė: tekstas, mygtukai vienas po kito per visą plotį, paveikslėlis | mygtukai eilutėje | dvi kolonėlės: tekstas kairėje, paveikslėlis dešinėje, vertikaliai centruoti |
| Apie mus | viena kolonėlė: paveikslėlis (proporcija 4:3) ir po juo tekstas | dvi kolonėlės: paveikslėlis kairėje (proporcija 4:5), tekstas dešinėje | didesnis tarpas tarp kolonėlių (80 px) |
| Meniu kortelės | 1 stulpelis | 2 stulpeliai | 3 stulpeliai |
| Galerija | 2 stulpeliai, eilutės 140 px | 4 stulpeliai, eilutės 160 px | 4 stulpeliai, eilutės 224 px |
| Darbo laikas ir kontaktai | lentelė, po jos žemėlapis | tas pats | dvi kolonėlės greta |
| Poraštė | 1 stulpelis | 3 stulpeliai (pirmas dvigubai platesnis), apatinė juosta eilutėje | tas pats |
| Rezervacijos forma | laukai po vieną | laukai poromis | forma kairėje, šoninė informacija dešinėje (forma dvigubai platesnė) |

Prieš pateikiant darbą patikrink 320, 390, 768, 1024 ir 1440 px plotį: puslapis niekada neturi slinkti į šoną.

## 6. Komponentai

### 6.1 Antraštė

- Fonas `#FFFBF2`, apačioje 1 px linija.
- Logotipas: `images/logo.svg` (40 × 40 px) ir tekstas "Rytmetys" (DM Serif Display, 28 px), tarpas tarp jų 10 px. Logotipas yra nuoroda į `index.html`.
- Nuorodos: Apie mus, Meniu, Galerija, Darbo laikas, Rezervacija.
- Nuorodos hover: po nuoroda atsiranda 2 px geltona linija.
- Mygtukas "Rezervacija" (nuo 768 px): tarpai 10 px ir 20 px, pagrindinė spalva, balta 600 svorio raidė, hover metu tamsesnė žalia.

### 6.2 Hero

- Virš `h1` yra eilutė "Kepyklėlė ir kavinė Vilniuje" (žr. tipografiją).
- Du mygtukai: pilnaspalvis "Rezervuoti stalą" ir kontūrinis "Peržiūrėti meniu". Mygtukai pilulės formos, tarpai 12 px ir 24 px, 2 px rėmelis, tarpas tarp jų 12 px.
- Paveikslėlis `images/hero.svg`, proporcija 5:4, kampai 16 px.
- Ant paveikslėlio viršutiniame kairiajame kampe (16 px nuo kraštų) yra baltas ženkliukas su žaliu 8 px tašku ir tekstu "Šviežia duona kasdien nuo 6:00" (13 px, svoris 600), su šešėliu.

### 6.3 Apie mus

- Sekcijos fonas `#F4ECDD`.
- Paveikslėlis `images/apie.svg`, kampai 16 px.
- Tekstas: `h2`, dvi pastraipos ir trijų punktų sąrašas. Sąrašo žymeklis yra geltona varnelė (`images/check.svg`, 24 × 24 px), tarpas tarp žymeklio ir teksto 12 px, tarpas tarp punktų 12 px, tekstas 500 svorio.

### 6.4 Meniu kortelės

- Sekcijos antraštė ir trumpas aprašymas centruoti.
- Kortelė: balta, 1 px linijos rėmelis, kampai 16 px, šešėlis, paveikslėlis viršuje (proporcija 4:3), po juo tekstas su 20 px vidiniais tarpais (apačioje 24 px).
- Eilutėje pavadinimas (`h3`) kairėje ir kaina dešinėje (700 svoris, pagrindinė spalva). Jie sulygiuoti pagal teksto apačią.
- Žymė ("Populiaru", "Naujiena", "Vegetariška") yra kortelėse 1, 3 ir 5: geltona pilulė po aprašymu, 12 px tekstas.
- Vienos eilutės kortelės yra vienodo aukščio.
- Hover: kortelė pakyla 4 px, šešėlis tampa stipresnis, paveikslėlis padidėja iki 1,05 karto (kortelės paveikslėlis neišlenda už kortelės kraštų).

### 6.5 Galerija

Visi šeši paveikslėliai yra 4:3, bet langeliai yra skirtingų proporcijų, todėl paveikslėliai turi užpildyti langelį be iškraipymo. Kiekvienas paveikslėlis turi parašą apačioje: baltas tekstas (14 px, svoris 500) ant tamsėjančio perėjimo, kampai 16 px.

Langelių numeriai atitinka HTML eilės tvarką: 1 Rytinė krosnis, 2 Pusryčių stalas, 3 Kavos baras, 4 Desertų vitrina, 5 Terasa saulėtą dieną, 6 Duonos lentyna.

Telefonas (2 stulpeliai):

```
+-----------+
|           |
|     1     |
|           |
+-----+-----+
|     |  3  |
|  2  +-----+
|     |  4  |
+-----+-----+
|     5     |
+-----------+
|     6     |
+-----------+
```

Nuo 768 px (4 stulpeliai):

```
+-----------+-----+-----+
|           |     |  3  |
|     1     |  2  +-----+
|           |     |  4  |
+-----------+-----+-----+
|     5     |     6     |
+-----------+-----------+
```

Hover: paveikslėlis padidėja iki 1,06 karto (langelio ribose).

### 6.6 Darbo laikas ir kontaktai

- Sekcijos antraštė "Aplankykite mus" ir sakinys po ja centruoti. Toliau du blokai su `h3` antraštėmis: "Darbo laikas" ir "Kur mus rasti".
- Lentelė balta kortelėje (1 px linija, kampai 16 px, šešėlis). Lentelės pavadinimas (`caption`) yra žalia juosta su balta 600 svorio raide. Po juo antraštės eilutė ant `#F4ECDD` fono, o apačioje pastaba (`tfoot`) 14 px pritilusia spalva. Eilučių skirtukai yra 1 px linijos. Lentelės langelių vidiniai tarpai: 12 px vertikaliai ir 16 px horizontaliai (nuo 768 px horizontalūs tarpai 20 px).
- Dienų pavadinimai (`th` eilutėse) yra 600 svorio. Hover: eilutės fonas pasikeičia į `#FFFBF2`.
- Žemėlapis `images/zemelapis.svg`, proporcija 16:9, kampai 16 px. Po juo adresas (nekursyvinis), telefonas ir el. paštas kaip nuorodos (`tel:` ir `mailto:`).

### 6.7 Kvietimo blokas

Žalias (`#0F5C4D`) blokas per visą plotį. Centruotas baltas `h2`, po juo aprašymas (`#E6F2EC`) ir geltonas mygtukas "Rezervuoti stalą" (geltonas fonas, tamsus tekstas). Turinio plotis ne didesnis nei 704 px. Vertikalūs tarpai: 64 px, nuo 1024 px - 80 px.

### 6.8 Poraštė

- Fonas `#1E2A28`, tekstas `#C9D3CF`, 15 px; nuorodos be pabraukimo, hover metu baltos ir pabrauktos.
- Pirmas stulpelis: logotipas su baltu tekstu ir sakinys "Kepyklėlė ir kavinė Vilniaus senamiestyje." (ne platesnis nei 288 px). Antras: "Nuorodos" ir penkių nuorodų sąrašas. Trečias: "Kontaktai" ir adresas.
- Stulpelių pavadinimai: 13 px, 600 svoris, didžiosios raidės, tarpai tarp raidžių 0,08 em, balti.
- Apačioje 1 px skiriamoji linija (balta, 14 % nepermatomumo) ir du tekstai (13 px): telefone vienas po kito, nuo 768 px eilutėje: vienas kairėje, kitas dešinėje.

### 6.9 Rezervacijos puslapis

- Viršus ant `#F4ECDD` fono: trupinių kelias (Pradžia / Rezervacija, 14 px, pritilusi spalva), `h1` ir aprašymas.
- Forma baltoje kortelėje (rėmelis, kampai 16 px, šešėlis), vidiniai tarpai 24 px (telefone) ir 32 px (nuo 768 px). Tarpas tarp grupių 28 px.
- Grupių pavadinimai (`legend`): DM Serif Display, 20 px. Vidinių grupių (patvirtinimo būdas, pageidavimai) `legend` yra Inter 15 px, svoris 600.
- Laukas: pavadinimas (15 px, svoris 600) virš laukelio, tarpas 6 px. Laukelis: tarpai 12 px ir 14 px, 1 px rėmelis `#8A9894`, kampai 12 px, šriftas paveldimas iš puslapio. Laukelių plotis 100 %.
- Komentaro laukas (`textarea`): bent 112 px aukščio, keičiamas tik vertikaliai.
- Radio ir checkbox: 18 × 18 px, pagrindinė spalva, tarpas iki teksto 10 px. Patvirtinimo būdo radio mygtukai eilutėje, pageidavimai vienas po kito.
- Sutikimo tekstas: 15 px, pritilusi spalva. Mygtukas "Siųsti rezervaciją": pilnaspalvis, kaip hero mygtukas.
- Šoninė informacija: du blokai. "Prieš rezervuojant" (fonas `#F4ECDD`, kampai 16 px, tarpai 24 px, sąrašas su taškeliais) ir "Skubus klausimas?" (žalias fonas, baltas tekstas, telefonas 20 px, svoris 700).
- Forma niekur nesiunčiama (nėra serverio): `action` gali rodyti į patį puslapį, o `method` yra `get`.

## 7. Būsenos ir efektai

Visi pavyzdžiai yra faile `maketai/busenos.png`.

| Elementas | Hover | Fokusas arba klaida |
| --- | --- | --- |
| Pilnaspalvis mygtukas | fonas `#0A4237`, mygtukas pakyla 2 px | 3 px apvadas pagrindine spalva, atokiau 3 px |
| Kontūrinis mygtukas | užsipildo pagrindine spalva, tekstas baltas, pakyla 2 px | toks pat apvadas |
| Geltonas mygtukas | fonas `#D99A14`, pakyla 2 px | apvadas geltonas (ant žalio ir tamsaus fono) |
| Navigacijos nuoroda | 2 px geltona linija apačioje | toks pat apvadas |
| Meniu kortelė | pakyla 4 px, stipresnis šešėlis, paveikslėlis 1,05x | |
| Galerijos paveikslėlis | paveikslėlis 1,06x | |
| Lentelės eilutė | fonas `#FFFBF2` | |
| Formos laukas | rėmelis tampa pagrindinės spalvos | rėmelis pagrindinės spalvos ir 3 px šviesus žiedas (`rgba(15, 92, 77, 0.25)`) |
| Neteisingas laukas (po įvedimo) | | rėmelis `#B3261E` ir 3 px šviesus raudonas žiedas (`rgba(179, 38, 30, 0.18)`) |

Visi pereinamieji efektai turi būti glotnūs (`transition`), o ne šuoliu.

## 8. Kontroliniai matmenys

Šie matmenys paimti iš maketo. Mažas skirtumas (iki kelių pikselių) yra normalus.

| Dalis | 1440 px ekrane | 390 px ekrane |
| --- | --- | --- |
| Antraštės aukštis | 85 px | 116 px |
| Hero paveikslėlis | 472 × 378 px | 358 × 286 px |
| Apie mus paveikslėlis | 444 × 555 px | 358 × 269 px |
| Meniu kortelė | 331 × 409 px | 358 × 430 px |
| Galerija (visa) | 1056 × 712 px | 358 × 900 px |
| Galerijos langeliai: didelis, mažas | 518 × 468 ir 249 × 224 px | 358 × 292 ir 173 × 140 px |
| Darbo laiko lentelė | 496 × 298 px | 358 × 324 px |
| Žemėlapis | 496 × 279 px | 358 × 201 px |
| Kvietimo bloko aukštis | 315 px | 295 px |
| Poraštės aukštis | 329 px | 628 px |
| Rezervacijos forma | 672 × 1082 px | 358 × 1407 px |
| Rezervacijos šoninė informacija (plotis) | 336 px | 358 px |
