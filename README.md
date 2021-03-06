# eindopdracht_advanced_css_2
Herkansing eindopdracht advanced css
// commentaar achter de //strepen

Beste Joost,

Je hebt de eindopdracht niet goed genoeg gedaan. Je moet de eindopdracht 
herkansen.

Hier een aantal verbeterpunten:

In sub-opdracht 1 heb je momenteel in je CSS een class 'cardmain' en een class 
'cardfooter'. In deze classes heb je veel overlappende CSS. Dit zou je kunnen 
oplossen door je 'article' element op lijn 9 in je 'index.html', een class te 
geven van 'card'. Vervolgens kun je de 'card' class slecteren in je SCSS file en 
met het BEM && Sass principe al je styling groeperen. like so:

    .card {

        {some generic styles here}

        &main {

            {some 'cardmain' styles here}

        }

        &footer {

            {some 'cardfooter' styles here}

        }

    }
// akkoord, aangepast


// ik heb twee verschillende oplossingen gemaakt. Welke vind jij de beste, hoe zou jij het doen?
// ik vind de shift-up_container een beetje een getruukte oplossing

//
// ----------------------------------------------------------------------------
//

In sub-opdracht 2 heb je bovenaan in je CSS file voor je body een margin-top 
aangegeven. Echter veroorzaakt deze een grijze balk op je pagina. Deze balkt 
lijkt niet nodig.

//akkoord

Je kunt je 'main' element verwijderen en de styling die je daar hebt gezet in je 
'grid-container' stoppen.

// ja, kan. Als ik dan het browser-window versmal tot ik maar 1 kolom foto's over heb,
// staat die kolom niet meer in het midden maar links.
// Ik gebruikte de main met display flex en justify-content: center om dat op te lossen

Je moet dan alleen je 'max-width' aanpassen naar 100% 
(i.v.m. nog meer grijze balken!!).

// ja, dat kan, maar het leidt tot ander gedrag als je het browser-window heel breed maakt.
// Dan gaat 'ie de kolommen verdelen over het venster en anders blijven ze bij elkaar staan.


Dit is een quick-fix voor je Grid css:

.cardbutton {

  opacity: 0;

  border-radius: 5px;

  height: 2em;

  font-weight: bold;

  box-shadow: 2px 2px 2px gray;

}

.cardbackground:hover .card__button {

  opacity: 1;

  position: absolute;

  width: 100px;

  height: 30px;

  top: 0;

  left: 0;

  bottom: 0;

  right: 0;

  margin: auto;

}

// okee, helder, de transitie gaat met de opacity

Dit is nog geen Sass en kan beter.
// Akkoord, aangepast

Deze zelfde vorm van transitie kun je 
gebruiken om je 'img' minder zichtbaar te maken en je background kleur te 
veranderen.


// 
// Ik heb het niet 100% goed werkend gekregen.
   Als de button in beeld komt, rekt zijn container op. Is niet fraai.
   Een vaste width en heigth werken niet goed.
   Als je laat weten om welke property het gaat, werk ik er nog aan.

// Kan ik de button op een nettere manier centreren, zowel verticaal als horizontaal?
//   dus zonder harde waarden voor top en left?
*/

//
// ----------------------------------------------------------------------------
//

In sub-opdracht 3 is er horizontale scrolling mogelijk en de grijze balken zijn 
terug!!

// Klopt. Ik had de opdracht niet goed begrepen. Ik snap dat me laat herkansen, dat kon beter.

Je hebt ook nog niet correct het Sass principe toegepast. Daarnaast is je SCSS 
file nog wat rommelig. Probeer je classes goed te groeperen en je comments te 
verwijderen.

// akkoord, aangepast

Probeer ook om alleen je 'index.html' en je 'readme.txt' in de root van je 
directory te houden en plaats de rest in sub-folders. Al je CSS in een folder 
styles/css al je foto's in een folder foto's/images/pictures/assets enzovoorts.

// okee, overal aangepast

// een vraag
Ik heb buttons gemaakt maar dat hoeft eigenlijk niet, denk ik.
Omdat er geen form-action aan vast hoeft te zitten, een <a> doet al het werk.
Het zou dus ook met een <div> kunnen, denk ik. Ben je het daarmee eens?
//
// ----------------------------------------------------------------------------
//


Requirements

Algemene requirements

[ ] Sass principe is gebruikt in elke sub-opdracht

[x] BEM principe is gebruikt in elke sub-opdracht

[ ] Geen horizontale scrolling

Level 1:

[x] Testimonial design is compleet:

[x] footer testimonial - paars/blauw: #686de0

[x] Achtergrond pagina - grijs: #c3cfe2

[x] Achtergrondkleur tekst - wit: #fff

[x] Random portretfoto gebruikt

Level 2:

[ ] Portfolio grid is compleet:

[x] Achtergrond pagina grijs: #c3cfe2

[ ] Er verschijnt een button on hover. De foto verdwijnt smoothly.

[x] Grid is mobile responsive voor 3 schermen: Desktop: 3 kolommen, Tablet:  2 
kolommen, Mobiel:  1 kolom   

Level 3:

[ ] Social media buttons zijn compleet:

[ ] Social media buttons zijn aanwezig

[ ] Social media buttons hebben ongeveer dezelfde animatie zoals in het 
voorbeeld

[ ] Social media iconen zijn toegevoegd met ::before (bonus)

Sterke punten

Je gebruikt goede namen voor je classes

Je testimonial is goed gedaan

Verbeterpunten

Je hebt niet aan de minimale requirements voldaan

Je hebt een onduidelijke file structuur

Er zit (veel) herhaling in je CSS

Met vriendelijke groet,

Namens het Winc docenten-team,

Ben Linnenbank docent(-assistent)

Sluiten
