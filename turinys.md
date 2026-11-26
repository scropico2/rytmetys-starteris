# Turinys: visi svetainės tekstai

Šiame faile yra visi tekstai ir nuorodos, kuriuos reikia įdėti į svetainę. Kopijuok juos tiksliai, kaip parašyta (su lietuviškomis kabutėmis „“, euro ženklu ir tarpais). Paveikslėlių `alt` tekstus parašyk pats pagal lentelę apačioje.

Kavinė "Rytmetys" yra išgalvota, todėl adresas, telefonas ir el. paštas yra neegzistuojantys.

## Bendra visiems puslapiams

**Puslapių pavadinimai (`<title>`):**

- `index.html`: Rytmetys - kepyklėlė ir kavinė Vilniuje
- `rezervacija.html`: Rezervacija - Rytmetys

**Antraštė.** Logotipas (`images/logo.svg`) ir tekstas "Rytmetys" (nuoroda į `index.html`). Navigacija:

| Tekstas | Kur veda |
| --- | --- |
| Apie mus | sekcija "Apie mus" (`#apie`) |
| Meniu | sekcija "Mūsų meniu" (`#meniu`) |
| Galerija | sekcija "Iš mūsų kasdienybės" (`#galerija`) |
| Darbo laikas | sekcija "Aplankykite mus" (`#laikas`) |
| Rezervacija | `rezervacija.html` |

Rezervacijos puslapyje nuorodos į sekcijas turi vesti į `index.html` (pavyzdžiui, `index.html#meniu`).

**Poraštė.**

- Logotipas, tekstas "Rytmetys" ir sakinys: Kepyklėlė ir kavinė Vilniaus senamiestyje.
- Stulpelis "Nuorodos": Apie mus, Meniu, Galerija, Darbo laikas, Rezervacija.
- Stulpelis "Kontaktai": Rytmečio g. 12, Vilnius; +370 600 00 000 (nuoroda `tel:+37060000000`); labas@rytmetys.example (nuoroda `mailto:labas@rytmetys.example`).
- Apatinė juosta, du tekstai: © 2026 Rytmetys. Visos teisės saugomos. ir Išgalvota kavinė, sukurta mokomajam projektui.

## index.html

### Hero

- Eilutė virš antraštės: Kepyklėlė ir kavinė Vilniuje
- `h1`: Pradėkite rytą su šviežia duona ir gera kava
- Tekstas: Kepame kasdien nuo 6 valandos ryto, kavą skrudiname patys, o pusryčius patiekiame iki pat pietų.
- Mygtukai: Rezervuoti stalą (veda į `rezervacija.html`) ir Peržiūrėti meniu (veda į `#meniu`)
- Ženkliukas ant paveikslėlio: Šviežia duona kasdien nuo 6:00
- Paveikslėlis: `images/hero.svg`

### Apie mus

- `h2`: Duona, kuri kvepia visam kvartalui
- Pirma pastraipa: „Rytmetys“ gimė 2016 metais kaip maža šeimos kepyklėlė Vilniaus senamiestyje. Šiandien čia kepame raugintą duoną, sviestinius kepinius ir desertus, o šalia jų patiekiame kavą iš vietinės skrudyklos.
- Antra pastraipa: Naudojame sezonines vietines žaliavas, o neparduotus kepinius vakare dovanojame vietos bendruomenei.
- Sąrašas:
  - Duona kepama kiekvieną rytą
  - Kava skrudinama Lietuvoje
  - Pusryčiai iki 12:00, savaitgaliais iki 14:00
- Paveikslėlis: `images/apie.svg`

### Mūsų meniu

- `h2`: Mūsų meniu
- Tekstas: Kiekvieną rytą kepame šviežiai, todėl kai kurie skanėstai baigiasi gerokai anksčiau nei pietūs.

| Nr. | Paveikslėlis | Pavadinimas | Aprašymas | Kaina | Žymė |
| --- | --- | --- | --- | --- | --- |
| 1 | `kruasanas.svg` | Sviestinis kruasanas | Traškus, daugiasluoksnis, kepamas kiekvieną rytą su sviestu. | 2,80 € | Populiaru |
| 2 | `sumustinis.svg` | Avokado skrebutis | Raugintos duonos riekė su avokadu, keptu kiaušiniu ir citrinos sultimis. | 6,50 € | |
| 3 | `suktinukas.svg` | Cinamono suktinukas | Minkštas mielinis suktinukas su cinamonu ir cukraus glaistu. | 3,20 € | Naujiena |
| 4 | `kapucinas.svg` | Kapučinas | Dvigubas espresso su šilto pieno puta. Galima rinktis augalinį pieną. | 3,40 € | |
| 5 | `kose.svg` | Avižinė košė | Virta ant pieno ar vandens, su sezoninėmis uogomis ir medumi. | 5,80 € | Vegetariška |
| 6 | `pyragas.svg` | Morkų pyragas | Drėgnas pyragas su graikiniais riešutais ir kreminio sūrio kremu. | 4,20 € | |

### Iš mūsų kasdienybės (galerija)

- `h2`: Iš mūsų kasdienybės
- Šeši paveikslėliai su parašais, eilės tvarka:

| Nr. | Paveikslėlis | Parašas |
| --- | --- | --- |
| 1 | `galerija-krosnis.svg` | Rytinė krosnis |
| 2 | `galerija-pusryciai.svg` | Pusryčių stalas |
| 3 | `galerija-baras.svg` | Kavos baras |
| 4 | `galerija-vitrina.svg` | Desertų vitrina |
| 5 | `galerija-terasa.svg` | Terasa saulėtą dieną |
| 6 | `galerija-lentyna.svg` | Duonos lentyna |

### Aplankykite mus (darbo laikas ir kontaktai)

- `h2`: Aplankykite mus
- Tekstas: Mus rasite Vilniaus senamiestyje, ramioje gatvelėje netoli centro.
- Pirmas blokas, `h3`: Darbo laikas. Lentelė:

| Lentelės dalis | Turinys |
| --- | --- |
| Pavadinimas (`caption`) | Savaitės darbo laikas |
| Antraštės eilutė (`thead`) | Diena, Atidarome, Uždarome |
| Eilutė 1 | Darbo dienomis, 07:00, 19:00 |
| Eilutė 2 | Šeštadieniais, 08:00, 20:00 |
| Eilutė 3 | Sekmadieniais, 08:00, 16:00 |
| Pastaba (`tfoot`, vienas langelis per visus tris stulpelius) | Šventinėmis dienomis darbo laikas gali skirtis. |

- Antras blokas, `h3`: Kur mus rasti. Žemėlapis (`images/zemelapis.svg`) ir adresas: Rytmečio g. 12, Vilnius; +370 600 00 000; labas@rytmetys.example (telefonas ir el. paštas yra nuorodos).

### Kvietimo blokas

- `h2`: Norite staliuko savaitgalį?
- Tekstas: Savaitgaliais vietų greitai neužtenka, todėl rezervuokite iš anksto.
- Mygtukas: Rezervuoti stalą (veda į `rezervacija.html`)

## rezervacija.html

### Puslapio viršus

- Trupinių kelias: Pradžia (nuoroda į `index.html`) / Rezervacija
- `h1`: Rezervuokite stalą
- Tekstas: Užpildykite formą, o per dvi valandas patvirtinsime rezervaciją. Jei reikia skubiai, skambinkite.

### Forma

Forma turi tris grupes. Laukų pavadinimai (`label`) ir reikalavimai:

| Grupė (`legend`) | Laukas | Tipas | Reikalavimai |
| --- | --- | --- | --- |
| Jūsų duomenys | Vardas ir pavardė | tekstas | privalomas; užuomina: Jonas Jonaitis |
| Jūsų duomenys | El. paštas | el. paštas | privalomas; užuomina: jonas@pastas.lt |
| Jūsų duomenys | Telefono numeris | telefonas | privalomas; 8-16 simbolių iš skaitmenų, tarpų ir pliuso; užuomina: +370 600 00 000 |
| Rezervacijos informacija | Data | data | privaloma |
| Rezervacijos informacija | Laikas | laikas | privalomas; nuo 07:00 iki 19:00, kas 15 minučių |
| Rezervacijos informacija | Svečių skaičius | skaičius | privalomas; nuo 1 iki 10; pradinė reikšmė 2 |
| Rezervacijos informacija | Pageidaujama vieta | pasirinkimas (`select`) | parinktys: Nesvarbu, Salėje, Terasoje, Prie lango |
| Papildomai | Kaip patvirtinti rezervaciją? | du radio mygtukai | El. paštu (pažymėtas iš anksto), SMS žinute |
| Papildomai | Pageidavimai | trys žymimieji langeliai | Reikia vaikiškos kėdutės; Švenčiame gimtadienį; Turime alergijų (parašysiu komentare) |
| Papildomai | Komentaras | kelių eilučių laukas | neprivalomas; 4 eilutės; iki 300 simbolių; užuomina: Pvz., atvyksime su vežimėliu |
| Papildomai | Sutikimas | žymimasis langelis | privalomas; tekstas: Sutinku, kad mano duomenys būtų naudojami rezervacijai patvirtinti |

Mygtukas: Siųsti rezervaciją

### Šoninė informacija

Pirmas blokas, `h2`: Prieš rezervuojant. Sąrašas:

- Staliuką laikome 15 minučių nuo rezervacijos laiko.
- Grupėms nuo 8 svečių prašome skambinti.
- Patvirtinimą atsiųsime el. paštu arba SMS žinute.
- Į terasą galite ateiti su augintiniu.

Antras blokas, `h2`: Skubus klausimas? Tekstas: Skambinkite darbo valandomis: ir telefonas +370 600 00 000 (nuoroda).

## Paveikslėliai

Visi failai yra aplanke `images/`. Kiekvienam `<img>` nurodyk `alt` tekstą (kas pavaizduota) ir `width` bei `height` atributus pagal žemiau esančius matmenis. Jei paveikslėlis yra grynai dekoratyvus (šalia jau yra tas pats tekstas), `alt` gali būti tuščias.

| Failas | Matmenys | Kur naudojamas | Kas pavaizduota |
| --- | --- | --- | --- |
| `logo.svg` | 64 × 64 | antraštė, poraštė, svetainės piktograma (favicon) | tekanti saulė virš horizonto, šalia yra tekstas "Rytmetys" |
| `hero.svg` | 1000 × 800 | hero | kavos puodelis ir sviestinis kruasanas ant medinio stalo, fone teka saulė |
| `apie.svg` | 800 × 1000 | Apie mus | kepyklos vidus: duonos kepalai ant lentynos, langas, prekystalis |
| `kruasanas.svg` | 800 × 600 | meniu kortelė 1 | sviestinis kruasanas ant baltos lėkštės |
| `sumustinis.svg` | 800 × 600 | meniu kortelė 2 | raugintos duonos skrebutis su avokadu ir keptu kiaušiniu |
| `suktinukas.svg` | 800 × 600 | meniu kortelė 3 | du cinamono suktinukai ant kepimo popieriaus |
| `kapucinas.svg` | 800 × 600 | meniu kortelė 4 | kapučino puodelis su putos širdele, vaizdas iš viršaus |
| `kose.svg` | 800 × 600 | meniu kortelė 5 | dubuo avižinės košės su uogomis ir medumi |
| `pyragas.svg` | 800 × 600 | meniu kortelė 6 | morkų pyrago riekė su graikiniais riešutais |
| `galerija-krosnis.svg` | 800 × 600 | galerija 1 | krosnis su šviežiai iškeptais kepalais |
| `galerija-pusryciai.svg` | 800 × 600 | galerija 2 | pusryčių stalas: kruasanas, kava ir uogienė |
| `galerija-baras.svg` | 800 × 600 | galerija 3 | kavos baras su espresso aparatu |
| `galerija-vitrina.svg` | 800 × 600 | galerija 4 | desertų vitrina su pyragaičiais ir sausainiais |
| `galerija-terasa.svg` | 800 × 600 | galerija 5 | kavinės terasa su skėčiu ir staliukais |
| `galerija-lentyna.svg` | 800 × 600 | galerija 6 | duonos lentyna su kepalais ir batonais |
| `zemelapis.svg` | 800 × 450 | kontaktai | žemėlapis su kavinės vieta Vilniaus senamiestyje |
| `check.svg` | 24 × 24 | sąrašo žymeklis "Apie mus" sekcijoje (per CSS) | geltona varnelė |
