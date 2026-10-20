# Wijzigingen per scherm

Datum: 20 oktober 2026
Uitgangspunt: de aangeleverde MindMirror_DP4_Prototype.zip van 1 oktober 2026.

De vormgeving, CSS, kleuren, lettertypen en bestaande 21 scherm-ID’s zijn behouden. Er zijn geen nieuwe hoofdschermen toegevoegd. Alleen de kernflow en bijbehorende statusweergave zijn aangepast.

| Scherm | Wat is aangepast | Waarom |
| --- | --- | --- |
| AI-inzicht (`insight`) | Uitstelgedrag niet meer als eerste verklaring tonen. Appgebruik en onbekende bedoeling worden gescheiden. Vraag Was dit een geplande pauze? met Ja, Nee, Weet ik niet en Overslaan. Bij Ja volgt de vraag of de pauze uitliep. Directe knop Dit klopt niet en directe toegang tot pauzeren. Eigen opgeslagen context blijft zichtbaar bij terugkeer. | DP4: uitleg en correctie waren bij alle drie gedeeltelijk duidelijk. Een geplande pauze mag niet zelfstandig als uitstelgedrag worden gelabeld. |
| Waarom dit inzicht (`explain`) | Studietijd preciezer aan donderdag gekoppeld; de AI-redenering verwijst niet meer naar een veronderstelde intentie. De vervolgknop gaat naar de contextvraag. | Tijd en duur verklaren geen bedoeling. |
| Controleer AI (`failure`) | Geplande pauze en Liever niet invullen toegevoegd. De oorspronkelijke andere contextkeuzes blijven aanwezig. De te stellige uitspraak is vervangen door een waarneming. Opslaan blijft uitgeschakeld tot een optie gekozen is; bij een verwerkingsfout volgt een foutmelding. | Direct en vrijwillig kunnen tegenspreken zonder een reden te moeten verantwoorden. |
| Correctie (`corrected`) | Bevestiging toont de werkelijk gekozen context. De oude versie toonde altijd Informatie voor school. De keuze voor een geplande pauze is expliciet herkenbaar. Alleen na een zelf gemelde uitloop volgt toegang tot een vrijwillig voorstel. Terug naar inzicht, inzicht verwijderen en pauzeren zijn bereikbaar. | Zichtbaar herstel en bevestiging die overeenkomt met de gekozen correctie. |
| Voorstel (`suggestion`) | De niet door de gebruiker bevestigde uitspraak over gemiddeld 18 minuten uitloop is verwijderd. De reminder is gekoppeld aan de eigen melding dat de pauze uitliep. Nee bedankt en Later hebben een duidelijke bevestiging. Terug naar Home en direct pauzeren toegevoegd. | Ondersteuning blijft vrijwillig; geen suggestie op basis van een onbekende bedoeling. |
| Jouw gegevens (`privacysetup`) | Locatiekeuze verwijderd. Alle andere gegevenskeuzes en de doorgaan-knop behouden. | Locatie is niet nodig voor de gekozen kernflow. |
| Privacy en controle (`privacy`) | Locatiekeuze verwijderd. Bestaande overige schakelaars en routes behouden. | Sluit aan op dataminimalisatie in de DP6-documenten. |
| AI pauzeren (`pause`) | Pauzeduur wordt bijgehouden binnen de demo. Hervatten en terug naar Home toegevoegd. Pauze onderdrukt nieuwe contextvragen en toegang tot reminder-voorstellen; bestaande context blijft beschikbaar. | De pauzeknop heeft nu een zichtbaar gevolg in de kernflow. Dit simuleert geen echte gegevensverwerking. |
| Home (`home`) | Toont de gekozen context, pauzestatus of verwijderstatus. Bij pauze is hervatten bereikbaar. De knop naar het verwijderde inzicht verdwijnt na Inzicht verwijderen. | Een handeling blijft herkenbaar na terugkeer naar Home. |
| AI-activiteit (`aihistory`) | De vooraf ingevulde correctie naar Informatie voor school is verwijderd. Een correctieregel verschijnt pas na eigen invoer en toont de gekozen context. | Geen onuitgevoerde correctie als uitgevoerd tonen. |
| Over de AI (`about`) | Verduidelijkt dat de AI zelf geen apps blokkeert of probleemgedrag labelt. | Sluit aan op de morele grens uit DP6. |

## Wat verder gelijk is gebleven

De volledige CSS is ongewijzigd. De volgende tien schermen zijn inhoudelijk en qua HTML exact gelijk gebleven: welkom, inzichtenoverzicht, doelen, nieuw doel, profiel, account, wachtwoord, meldingen, mijn gegevens en gegevens verwijderen. Bestaande account-, export- en meldingsfuncties blijven dezelfde demo-interacties.

De gegevensschakelaars en terugpijlen hebben daarnaast toegankelijke labels gekregen. De zichtbare vormgeving is daarvoor niet aangepast.

## Technisch gecontroleerd

- Geen JavaScript-syntaxisfouten of dubbele HTML-ID’s.
- Alle navigatiebestemmingen bestaan; alle navigatieroutes zijn lokaal via de eventlogica doorlopen.
- Alle zeven correctieopties tonen hun eigen bevestiging en context bij heropenen.
- Geplande pauze met en zonder uitloop; onbekende context en overslaan.
- Voorstel weigeren, inzicht verwijderen, pauzeren en hervatten.
- Alle vier pauzeduren, privacyknoppen en bestaande menuroutes.

Deze controle is uitgevoerd met een lokale DOM- en eventtest, niet met proefpersonen. Een visuele browsercontrole was door een beveiligingscontrole van de app niet beschikbaar. Er worden daarom geen nieuwe gebruikerstestresultaten of bewezen welzijnseffecten geclaimd.

## Nog doen voor DP6

Leg dezelfde schermen uit de oorspronkelijke en verbeterde versie naast elkaar vast, met datum en bijbehorende DP4-feedback. Test daarna de aangepaste flow met echte deelnemers en werk de resultaten bij in de Research Journey. De wijziging is nu uitgevoerd in deze HTML-versie; de vervolgtest is nog niet uitgevoerd.
