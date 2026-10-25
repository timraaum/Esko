# Testing og sikkerhet

Notert 19.10.2026 som et punkt som må løses før Oda, og som bør stå i pitchen som "vi har plan for dette", ikke som noe som ikke finnes.

## Hvorfor det er viktig

Produktet er for barn fra 2 år, altså under 3 år. Det utløser de strengeste kravene i leketøysregelverket, og det er det første en innkjøper hos Oda vil spørre om.

## Regelverk (må verifiseres mot gjeldende versjon)

- EUs leketøysdirektiv (2009/48/EF, med nytt leketøysregelverk under innfasing). Gjelder i Norge gjennom EØS, forvaltet av DSB.
- CE-merking er påkrevd for leketøy. Produsent eller importør er ansvarlig.
- EN 71-serien er de harmoniserte standardene:
  - EN 71-1: mekaniske og fysiske egenskaper. Smådeler, kvelningsfare, skarpe kanter. Mest relevant for klypene.
  - EN 71-2: brennbarhet.
  - EN 71-3: migrasjon av visse grunnstoffer (kjemi).
- Smådelstest (small parts cylinder) er avgjørende for barn under 3 år. Klypene og eventuelle løse deler (hengselpinner) må enten ikke passe i sylinderen, eller produktet må merkes for 3 år og oppover. Det siste svekker målgruppen.
- Teknisk dokumentasjon og samsvarserklæring må kunne legges fram.

## Materiale

- PLA er ugiftig i utgangspunktet, men 3D-printede deler har lag og porer der bakterier kan sette seg. "Barn tygger på de" er derfor mer et hygienespørsmål enn et giftspørsmål.
- Ved volumproduksjon (sprøytestøp) forsvinner lagproblemet. Da er det materialets sertifikat som teller.
- Alternativer å vurdere: sprøytestøpt PLA, resirkulert PP eller PE, biokompositter. Valget må henge sammen med bærekraftargumentet.
- Produsenten bør kunne levere materialsertifikat og EN 71-3-test.

## Plan

1. Mål klypene mot smådelssylinderen (31,7 mm diameter, 25,4 til 57,1 mm dybde). Dokumenter resultatet. Status 22.10.2026: minste klype er 60 x 40 x 20 mm, lengre enn sylinderens dypeste punkt og bredere enn åpningen. Bør bestå med god margin, men sylinderens diagonal er ca. 65 mm, så det må testes fysisk med sylinder.
2. Sjekk om hengselvarianten har løse deler. Hvis ja, design om til én del eller fast pinne. Status 22.10.2026: ingen deler som kan løsne.
3. Ved produsentvalg: krev CE-dokumentasjon og EN 71-1/-2/-3-testrapporter som del av tilbudet.
4. Vurder om vi trenger egen testing hos akkreditert laboratorium i Europa (SGS, Intertek, TÜV, eller Nemko i Norge) i tillegg til produsentens.
5. Avklar hvem som er "produsent" juridisk (vi eller Oda) og dermed hvem som er ansvarlig for CE-merkingen. Status 25.10.2026: i piloten printer vi settene selv, og da er vi produsent. Se "CE-merking av pilotsettene" under.
6. Vurder aldersmerkingen på nytt når vi vet mer om hvem som bygger. Hvis barn fra ca. 4 år bygger selv og de minste først og fremst leker i bygget, svekker merking for 3 år og oppover kanskje ikke målgruppen så mye som antatt.

## Stabilitet og bruk

I tillegg til regelverket bør vi dokumentere:

- Hvor stabil strukturen er når en toåring drar i den eller lener seg mot den.
- Hvor lang tid byggingen tar for en vanlig familie. Internt målt til 5 minutter med barn og 2 til 3 minutter alene, men av den som har designet klypene.
- Hvem som klarer å bygge selv i ulike aldre. Antakelse: voksne intuitivt, barn fra ca. 4 år.
- Hvor mange ganger klypene tåler å settes på og tas av før de mister grep. Så langt har ingen av ca. 50 printede klyper knekt eller mistet grep. Pappen blir litt slapp ved gjentatt festing på samme sted.
- At klypene ikke knekker ved misbruk (fall, vridning, trekk, tråkk). Printet PLA er sprøtt, og en flik som brekker av, blir vurdert som smådel. Sprøytestøpte klyper må testes på nytt.

## CE-merking av pilotsettene

Notert 25.10.2026. Reglene gjelder også for et lite opplag så lenge settene selges til kunder. Når vi printer selv, er vi produsent. Bruker vi EN 71 fullt ut, kan vi erklære samsvar selv uten godkjenningsorgan, men vi må kunne dokumentere det.

1. **Sikkerhetsvurdering.** Skriftlig vurdering av alle farer og hvordan barn kan bli utsatt for dem:
   - Mekanisk og fysisk: smådeler, skarpe kanter, klemfare i hengselen, hva som skjer hvis en klype knekker.
   - Brennbarhet.
   - Kjemi: innholdet i filament og fargestoffer.
   - Hygiene: leker for barn under 3 år skal kunne rengjøres. Printet PLA har lag og porer, så vi må vise at klypene kan vaskes og skrive hvordan i bruksanvisningen.
2. **Testing mot EN 71.**
   - EN 71-1 (mekanisk): smådelstest, kanter, fall og misbruksprøver. Bør gjøres på laboratorium for det ferdige produktet, fordi en rapport står sterkere overfor Oda.
   - EN 71-2 (brennbarhet): se eget punkt under.
   - EN 71-3 (kjemi): kan trolig dekkes av testrapport fra filamentleverandøren, se eget punkt under.
3. **Teknisk dokumentasjon**, som oppbevares i 10 år: beskrivelse med tegninger og bilder, sikkerhetsvurderingen, standarder vi har brukt, testrapporter, materialer med datablad og leverandørerklæringer, og hvordan klypene produseres.
4. **EU-samsvarserklæring** på en til to sider: produkt, produsent, regler og standarder, dato og signatur.
5. **Merking:** CE-merke på produkt eller emballasje, produsentens navn og postadresse, parti- eller produktnummer, bruksanvisning og eventuelle advarsler på norsk. Advarselen "Ikke egnet for barn under 3 år" kan ikke brukes på et produkt som åpenbart er laget for de minste. Velger vi 3 år og oppover, må markedsføring og bilder også vise eldre barn.
6. **Kontroll av produksjonen:** noter filament, farge og printinnstillinger, og sjekk hver klype for sprekker og skarpe kanter før pakking. Bytte av filamenttype kan kreve ny testing.

I tillegg: selskap med organisasjonsnummer før salg, og produktansvarsforsikring før salget starter. EU har vedtatt en ny forordning om leketøy med blant annet digitalt produktpass. Så vidt vi vet gjelder den ikke før om noen år, så den påvirker ikke piloten, men kan påvirke et større opplag.

### Filament og kjemi (EN 71-3)

PLA er i seg selv ganske standardisert, men det er fargestoffene og tilsetningene som avgjør EN 71-3, og de varierer mellom produsenter og farger. Noen filamentprodusenter dokumenterer dette selv. Bambu Lab lanserte i juni 2026 PLA Pure, som de sier har bestått EN 71-3. Vi har bare sett påstanden i markedsføring og hos forhandlere, ikke selve rapporten, og sertifiseringen gjelder filamentet, ikke ferdige leker.

Plan: velg ett filament med dokumentert EN 71-3, hent inn testrapporten fra et akkreditert laboratorium for den fargen vi bruker, og hold oss til det filamentet.

### Brennbarhet (EN 71-2)

For små, stive plastklyper gjelder trolig bare de generelle kravene, som PLA lett oppfyller. Men EN 71-2 har strengere krav til leker barn kan gå inn i, som lekehus og telt. Vi selger bare klypene og pappen kommer fra Oda, men bruksanvisningen viser hus barna kryper inn i. Om det påvirker vurderingen, må avklares med laboratorium eller DSB.

## Ting vi må sjekke opp før pitch

- [ ] Hent EN 71-3-testrapport for filamentet vi vil bruke (f.eks. Bambu Lab PLA Pure), og sjekk at den gjelder vår farge og kommer fra et akkreditert laboratorium.
- [ ] Be et laboratorium (Nemko, SGS, Intertek eller TÜV) om tilbud. Legg ved filamentrapporten og spør hvilke tester som gjenstår.
- [ ] Spør laboratoriet eller DSB om klyper som brukes til lekehus barn kan gå inn i, faller inn under de strengere kravene i EN 71-2.
- [ ] Les DSBs veiledning for leketøy.
- [ ] Bestem aldersmerking for piloten (fra 2 år eller fra 3 år), med tanke på hygiene ved printet PLA.
- [ ] Sjekk pris på produktansvarsforsikring.
- [ ] Test klypene fysisk med smådelssylinder.
