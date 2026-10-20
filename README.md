# MindMirror verbeterde versie

Herzien op 20 oktober 2026. De bestaande vormgeving en schermstructuur zijn behouden. De kernflow is aangepast op basis van de bestaande DP4-feedback en de DP6-ontwerpkeuzes.

## Openen
1. Pak de zip volledig uit.
2. Open de map `MindMirror_DP4_Prototype`.
3. Dubbelklik op `index.html` om het prototype in je browser te openen. Je kunt ook Live Server in Visual Studio Code gebruiken.

Er zijn geen externe libraries of installatie nodig. Open het HTML-bestand na het uitpakken, niet vanuit de zip-preview.

## Verbeterde kernflow
Aan de slag → gegevenskeuzes → Home → Bekijk inzicht → contextvraag of uitleg → correctie → bevestiging → eventueel vrijwillige suggestie → privacy en AI pauzeren.

Voorbeeld 1: kies bij het inzicht **Ja, een geplande pauze** en vervolgens **Nee, ik bleef binnen mijn pauze**. De bevestiging toont Geplande pauze; er volgt geen reminder.

Voorbeeld 2: kies **Ja, mijn pauze liep uit**. Alleen dan verschijnt de knop om een vrijwillige suggestie te bekijken. **Nee bedankt** stelt geen reminder in.

Voorbeeld 3: kies **Dit klopt niet**, selecteer een eigen context en sla op. De bevestiging en de AI-activiteit tonen de werkelijk gekozen context. Je kunt ook **Liever niet invullen** kiezen.

AI pauzeren is rechtstreeks bereikbaar vanuit de kernflow. Via **Terug naar Home** zie je de pauzestatus; **AI hervatten** brengt je naar het pauzescherm waar je kunt hervatten.

## Wat dit prototype doet
Dit is een interactieve demo met voorbeeldgegevens, zonder werkende AI, server of koppeling met echte gebruiksgegevens. Correctie en pauzestatus worden in het geheugen van de geopende pagina bijgehouden. Een uur, dag of week wordt binnen die sessie als eindtijd gebruikt; Tot ik het weer aanzet blijft actief binnen die sessie. De pagina opnieuw laden begint een nieuwe demo en wist deze keuzes.

Reminders, export, accountinstellingen en gegevensbeheer blijven simulaties zoals in de oorspronkelijke versie. Er worden geen echte meldingen verstuurd, accounts aangepast of gebruiksgegevens verzameld. Locatie is uit beide gegevensschermen verwijderd.

## Controle en vervolg
De JavaScript-syntaxis, schermverwijzingen en kliklogica zijn lokaal gecontroleerd, inclusief alle correctieopties, pauzeduren, weigeren, heropenen en navigatieroutes. De CSS en tien overige schermen zijn identiek aan het origineel. Een volledige visuele browsercontrole was in deze werkomgeving geblokkeerd; deze controles zijn geen gebruikerstest.

Voor DP6 kun je nu de originele en deze aangepaste versie naast elkaar vastleggen. Laat daarna deelnemers zonder hulp corrigeren, weigeren en pauzeren en noteer wat lukt. Er zijn bij deze wijziging geen nieuwe gebruikerstestresultaten toegevoegd.

Zie `VERBETERINGEN.md` voor de exacte wijzigingen per scherm.
