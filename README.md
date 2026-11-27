# Rytmetys: kavinės svetainė

HTML ir CSS atsiskaitymas, Vilnius Coding School.

- **Vardas, pavardė:** (Simas, Cicėnas)
- **Grupė:** (261019JVS492VAK)
- **GitHub Pages nuoroda (nebūtina):** (https://scropico2.github.io/rytmetys-starteris/)

## Kaip peržiūrėti

Atsisiųsk arba nusiklonuok repozitoriją ir atidaryk `index.html` naršyklėje. Rezervacijos puslapis yra `rezervacija.html`.

## Kas padaryta

Pažymėk `x` tai, ką baigei (`- [x]`). Ko nespėjai arba nepavyko, palik nepažymėta.

### 1 etapas: pagrindas

- [ `x`] Dokumento karkasas: `lang="lt"`, `charset`, `viewport`, `title`, šriftai, `css/style.css`
- [ `x`] Semantinė struktūra: `header`, `nav`, `main`, `section`, `footer`, viena `h1`
- [ `x` ] Visos `index.html` sekcijos pagal maketą (darbo laiko lentelę palik 2 etapui)
- [ ] Paveikslėliai su `alt`, `width` ir `height`; galerijoje `figure` ir `figcaption`
- [ `x` ] Telefono vaizdas (390 px) pagal maketą
- [ `x` ] Planšetės (768 px) ir kompiuterio (1024 px ir 1440 px) vaizdai pagal maketą
- [ `x` ] Flexbox (antraštė, mygtukai, kortelės vidus) ir Grid (meniu kortelės, galerija)

### 2 etapas: pilnas projektas

- [ `x` ] Darbo laiko lentelė (`caption`, `thead`, `tbody`, `tfoot`, `th scope`, `colspan`)
- [ `x` ] `rezervacija.html` su forma pagal maketą ir turinį
- [ `x` ] Formos laukai: tinkami `type`, `label for`, `fieldset` ir `legend`, `required`, `min`, `max`, `pattern`
- [ `x` ] CSS kintamieji (`:root`): spalvos, kampai, šešėlis, šriftai
- [ `x` ] Hover, fokuso ir klaidos būsenos pagal `maketai/busenos.png`, su `transition`
- [ `x` ] Spalvos, šriftai, tarpai ir smulkmenos atitinka maketą
- [ `x` ] Šis README užpildytas

### 3 etapas: mano dalis

- **Pasirinkta idėja:** (Animacijų papildymas.)
- **Ką padariau:** (Pasirinkau išskirtines korteles paryškindamas jų etiketes, taip jos dabar pulsuoja ir leidžia žinoti išskirtinumą vartotojui. Taip pat table sekcijoje, pridejau savaitgalio eilutėms animaciją, kuri atspindi, kad tai svaitgaliais tik.)
- **Kur kode:** (hoursTable tbody tr:nth-child(2),
  .hoursTable tbody tr:nth-child(3) // lentelių animacija;

cardBadge etikečių pulsavimas ;

heroBadge::before skrituliuko pulsavimas; )

## Kas nepavyko arba ką darytum toliau

Rėmiausi ankstesnėmis kurtomis svetainėmis ir patirtimi, nėra panaudotos topografijos taisyklių iš :root.
