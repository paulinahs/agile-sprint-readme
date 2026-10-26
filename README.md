# CheckoutLite - Sprintplanering

## Scrum-roller

- **Product Owner:** [Paulina] (även Utvecklare)
- **Scrum Master:** [Claudia] (även Utvecklare)
- **Utvecklare:**
  - [Paulina]
  - [Claudia]
  - [Filo]
  - [Pia]

---

## Sprintmål

[Vid sprintens slut ska kunden kunna använda en enkel kassaöversikt i CheckoutLite där butiksinformation visas tydligt, totalsumman räknas ut automatiskt, information om fri frakt visas och rabattkoder kontrolleras innan köp.]

### Agil motivering

[Genom att leverera funktionalitet stegvis kan vi testa att allt fungerar innan fler delar byggs på. Om något inte fungerar som tänkt får vi snabb feedback och kan justera lösningen tidigt istället för att behöva göra stora ändringar i slutet av projektet.]

---

## Produktbacklog

### US-1: Butiksidentitet

- **User Story:** Som kund vill jag kunna se butikens namn och vilken valuta som används så att jag känner mig trygg med mitt köp.
- **Acceptanskriterier:** Funktionen hamtaButikInfo() returnerar butikens namn och valuta, exempelvis "TechStore (SEK)".
- **Ansvarig:** [Pia]

### US-2: Totalberäkning

- **User Story:** Som kund vill jag automatiskt få se totalsumman inklusive moms så att jag vet vad jag faktiskt kommer att betala.
- **Acceptanskriterier:** Funktionen beraknaPris(summa) lägger på 25 % moms och returnerar det slutliga priset.
- **Ansvarig:** [Claudia]

### US-3: Fraktgräns

- **User Story:** Som kund vill jag veta om min order kvalificerar sig för fri frakt så att jag kan avgöra om jag vill handla mer.
- **Acceptanskriterier:** Funktionen kontrolleraFrakt(total) returnerar "Fri frakt" när ordervärdet är över 500 kr, annars "49 kr fraktavgift".
- **Ansvarig:** [Filo]

### US-4: Kuponghantering

- **User Story:** Som kund vill jag kunna ange en rabattkod så att systemet kan kontrollera att koden följer rätt format.
- **Acceptanskriterier:**  Funktionen verifieraKod(kod) returnerar true om rabattkoden innehåller minst fyra tecken, annars false.
- **Ansvarig:** [Paulina]

---

## Daily Standup & Sprint-anpassning

### Standup-notering

[Under dagens standup rapporterade teamet att arbetet går enligt plan. Funktionerna för prisberäkning och fraktstatus är nästan klara, medan rabattkodsfunktionen fortfarande testas.]

### Sprint-anpassning (Kravändring)

- **Vad:** [Kunden vill att rabattkoder ska fungera oavsett om användaren skriver med stora eller små bokstäver.]
- **Vem:** [Product Owner uppdaterar kravet och Claudia ansvarar för att justera funktionen så att inmatningen jämförs utan hänsyn till skiftläge]
- **Varför sprintmålet håller:** [Ändringen är liten och påverkar endast rabattkodsfunktionen. Den kräver ingen omarbetning av övriga delar och påverkar därför inte sprintens leverans.]