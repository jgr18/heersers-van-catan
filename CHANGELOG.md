# Wijzigingen Catan-competitie

Nieuwste versie bovenaan. Het versienummer staat onderaan in de app.

## v1.9

- Thema-figuren: Sinterklaas (plek 1 t/m 3, van 27 nov t/m 5 dec, zodra er in die periode een duel is ingevoerd) en kerst (alle plekken, van 6 t/m 26 dec). Daarna zijn de gewone figuren weer terug.
- Bestandsnamen in de map `spelers`: `jan_sint_1.png` en `jan_kerst_1.png` (cijfer = plek, 3 geldt voor plek 3 en lager). Ontbreekt een thema-figuur, dan wordt de gewone figuur getoond.
- Voorbeeld bekijken met `?thema=sint`, `?thema=kerst` of `?thema=geen` achter de link.

## v1.8

- Jan zit als 3e met zijn billen op de voorrand van het podium en als 4e (of lager) op een krukje naast het podium.

## v1.7

- Podium is twee keer zo diep, zodat een zittend figuur genoeg ruimte heeft. Spelers vanaf plek 4 staan iets verder van het podium af.
- Figuren worden op de werkelijke onderkant van het plaatje geplaatst, zodat ze op alle plekken netjes op het blok staan.

## v1.6

- Podium is nu één aaneengesloten geheel in 3D (goud, zilver, brons) met schaduw en glansrand. De figuren staan op het blok. Plek 4 en lager staan zonder voetstuk naast het podium.

## v1.5

- Podium boven de stand met de uitslag van het laatste duel: winnaar in het midden, de rest op lagere treden, 4e plek en lager staan naast het podium. Gedeelde plekken staan op dezelfde trede.
- Ook een podium in het seizoensarchief (eindstand van een afgesloten seizoen) en bij de beker (totaalstand).
- Eigen figuren per speler en per plek in de map `spelers` (bijvoorbeeld `jan_1.png`, `jan_2.png`, `jan_3.png`). Plek 3 en lager gebruikt figuur 3. Spelers zonder figuren krijgen een stripfiguurtje in hun kleur.

## v1.4

- De hele knop **Meldingen aan/uit** is nu aan te tikken, dus ook de tekst en niet alleen het belletje. De knop is groter en toont wanneer meldingen aan staan.
- Aanzetten van meldingen is betrouwbaarder: de knop toont "Bezig..." en voorkomt dubbel tikken, de app haalt eerst de nieuwste versie van `sw.js` op, en een ontbrekende reactie geeft na 10 seconden een duidelijke melding.
- Duidelijkere foutmeldingen, bijvoorbeeld bij een verouderde toegangscode of een browser die de meldingsdienst niet bereikt.

## v1.3

- Pushmeldingen per competitie. Deelnemers zetten ze zelf aan met **🔔 Meldingen** bovenaan een competitie.
- Als beheerder stuur je automatisch een melding bij een nieuwe uitslag (met de stand en een eventuele kampioen), bij een beslist seizoen en bij een nieuw "Volgend duel". Met het vinkje **Stuur melding naar de deelnemers** kun je dat per keer uitzetten, bijvoorbeeld bij het corrigeren van een stand.
- Bij een nieuwe toegangscode vervallen alle aanmeldingen voor meldingen.
- Nieuw: `sw.js`, `supabase-meldingen.sql` en de Edge Function `send-push`.

## v1.2

- Seizoensgrafiek: op de horizontale as staat nu "Duels" en op de verticale as "Punten".

## v1.1

- Seizoensarchief toont nu de volledige tabel per seizoen: punten, gespeeld, W, G en V. Seizoenen die zijn afgesloten zonder bewaarde potjes tonen een streepje bij G en V.
- In de hele app heet een potje nu een duel, bijvoorbeeld "Gespeelde duels" en "Uitslag duel 5".

## v1.0

Eerste volledige versie.

### Competities
- Meerdere competities naast elkaar (3 tot 6 spelers).
- Elke speler heeft een kleur: Rood, Blauw, Wit, Groen, Geel of Bruin. Die kleur komt terug in de stand.
- Instellingen per competitie: naam, spelers, kleuren, punten per plek en verwijderen.
- Punten per plek instelbaar. Standaard 3-1-0 bij 3 spelers en 3-2-1-0 bij 4 tot 6 spelers.

### Potjes en stand
- Uitslag invoeren per potje. Eén winnaar, andere plekken mogen gedeeld zijn.
- Stand met punten, gespeeld, W, G en V.
- Wie deelt: de laatste deelt het volgende potje, bij gelijk wordt gedobbeld.
- Vorm: de laatste 5 potjes als gekleurde rondjes.
- Reeksen: langste zegereeks, langste verliesreeks, huidige zegereeks en huidige verliesreeks.
- Lijst met gespeelde potjes. Het laatste potje kan worden verwijderd.
- Volgend duel: datum, locatie en tijd noteren (optioneel).

### Seizoenen en beker
- Een seizoen duurt 10 potjes. Bij gelijke stand volgt potje 11 of 12.
- Melding als de koploper niet meer kan worden ingehaald, met de keuze om het seizoen af te sluiten of door te spelen.
- Beker per competitie, geteld per seizoenswinnaar.
- Seizoensgrafiek met de puntenstand per potje.
- Seizoensarchief met per afgesloten seizoen de eindstand en de grafiek.
- Bekerstand aanpassen of op 0 zetten, en de seizoensstand op 0 zetten, met waarschuwing.

### Toegang en app
- Beheerder logt in met e-mail en wachtwoord en voert de uitslagen in.
- Vrienden kijken alleen mee met een gezamenlijke toegangscode of link. Een nieuwe code maken kan onder Toegang.
- De stand ververst zichzelf voor meekijkers.
- Te installeren als app op Android en iPhone, met eigen icoon.
- Achtergrond in Catan-stijl.
