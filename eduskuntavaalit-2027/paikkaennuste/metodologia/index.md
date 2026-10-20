---
title: "Miten paikkaennuste toimii"
layout: splash
---
<div class="ev2027" markdown="1">

# Miten paikkaennuste toimii

Databyron paikkaennuste muuntaa valtakunnalliset kannatusmittaukset arvioksi siitä, miten eduskunnan paikat jakautuisivat, jos vaalit pidettäisiin nyt. Ennuste on niin sanottu nowcast eikä forecast: se kuvaa tilannetta mittausten aikaan, mutta ei ennusta, miten kannatus muuttuu ennen huhtikuun 2027 eduskuntavaaleja tai minkälaiset kannatukset ovat silloin.

Ennuste lasketaan kolmessa vaiheessa.

## 1. Mittaukset

Ennuste perustuu kahteen säännöllisesti julkaistavaan valtakunnalliseen kannatusmittaukseen: Verianin (Helsingin Sanomat) ja Taloustutkimuksen (Yle) tuoreimpiin mittauksiin. Ennuste päivitetään kerran kuussa Verianin mittauksen julkaisun jälkeen. Näin ajoitettuna kahden tuoreimman mittauksen keruuajat ovat tyypillisesti enemmän päällekkäin kuin Taloustutkimuksen jälkeen ajoitettuna. Ennustekuvioiden alalaidassa kerrotaan aina, mitkä mittaukset paikkalaskennassa ovat mukana.

Ensiksi mittaukset yhdistetään antamalla kummallekin yhtä suuri paino. Mittausten otoskoot määräävät, kuinka paljon satunnaista otantavirhettä kannatuslukuihin liittyy: mitä suurempi otos, sitä pienempi otantavaihtelusta johtuva virhe.

## 2. Kannatuksen muuntaminen koko maan tasolta vaalipiiritasolle

Koska suomalaisessa vaalijärjestelmässä eduskunnan paikat jaetaan vaalipiireittäin, koko maan kannatus täytyy ensin muuntaa arvioiksi puolueiden kannatuksesta kussakin vaalipiirissä. Lähtötasona tälle ovat vuoden 2023 eduskuntavaalien vaalipiirikohtaiset tulokset kunkin puolueen osalta.

Puolueen kannatus kussakin vaalipiirissä muuttuu samassa suhteessa kuin sen kannatus koko maassa. Esimerkki: puolue keräsi edellisissä vaaleissa koko maassa 20 prosentin kannatuksen, ja mittauksissa sen kannatus on nyt 22 prosenttia. Kerroin, jolla vuoden 2023 piirikannatus puolueen osalta kerrotaan on tällöin 22 / 20 = 1,1. Jos puolue sai edellisissä vaaleissa Keski-Suomen vaalipiirissä 25 prosenttia, arvio sen nykyisestä kannatuksesta siellä on 25 × 1,1 = 27,5 prosenttia. Oulun vaalipiirissä 15 prosentin tulos muuttuu vastaavasti 16,5 prosentiksi. Jos puolueen kannatus koko maassa laskee, kerroin on pienempi kuin yksi ja arviot kannatuksesta laskevat kaikissa vaalipiireissä.

## 3. Vaalien simuloiminen piiritasolla ja summaus kansalliseksi ennusteeksi

Kun kannatukset on muutettu piirikohtaisiksi kunkin puolueen osalta, voidaan aloittaa vaalin simuloiminen kussakin piirissä. Tässä vaiheessa jokaisen puolueen kannatukseen vaalipiireissä lisätään hieman satunnaista vaihtelua. Se kuvaa sitä, ettei historiallisesti tarkasteltuna yksikään vaalipiiri ole seurannut koko maan kehitystä täsmälleen: syynä voivat olla esimerkiksi poikkeuksellisen onnistunut ehdokasasettelu piirissä tai paikallisesti pinnalla olevat poliittiset kysymykset. Kannatusvaihtelun suuruus piirissä perustuu Databyron arvioon.

Saadut puoluekohtaiset piirikannatukset muunnetaan eduskuntapaikoiksi kussakin vaalipiirissä d'Hondtin menetelmällä, kuten oikeissa vaaleissa, ja vaalipiirien paikat lasketaan yhteen kansalliselle tasolle.

Yksi tällainen vaalin simuloiminen ei kuitenkaan lopulta kerro, kuinka varma tulos on. Puolueen kansallisesti mitattu tulos voi esimerkiksi olla hieman pielessä tai puolue voi olla odotettua vahvempi odotettua useammassa piirissä. Siksi vaalit simuloidaan 10 000 kertaa hieman puolueiden mitattua kansallista kannatusta ja piirikohtaisia arvioita varioiden mitattujen kannatusten keskiarvon ympäriltä.

Vaalipiirien paikkamäärinä käytetään vuoden 2023 paikkamääriä, kunnes vuoden 2027 viralliset paikkamäärät on vahvistettu. Ahvenanmaan yksi paikka ei ole mukana laskelmassa, joten puolueiden paikat summautuvat 199:ään. Pienpuolueiden ja muiden ryhmien kannatus on mukana laskettaessa vaalipiirien kannatusosuuksia, mutta niille ei jaeta paikkoja, sillä suomalaisissa mielipidemittauksissa pienpuolueita käsitellään erittelemättömänä blokkina. Mikäli mittaajat alkavat näyttämään puoluekohtaisia kannatusosuuksia myös eduskunnan ulkopuolisille puolueille, Databyro pystyy estimoimaan niiden odotettua paikkamäärää muiden puolueiden tapaan.

Vaalipiirikohtaisia arvioita ei julkaista ennusteina.

## Näin luet ennustetta

- **Ennuste** on puolueen paikkamäärien keskiarvo 10 000 simulaatiossa. Keskiarvot on pyöristetty suurimman jäännöksen menetelmällä niin, että ne summautuvat 199:ään.
- **Vaaleampi palkki** puolueiden kuviossa niiden ennusteen taustalla on puolueen paikkamäärä vuoden 2023 vaaleissa.
- **80 %:n todennäköisyysväli** kertoo, mille välille puolueen paikkamäärä osui kahdeksassa simulaatiossa kymmenestä. Väli on simulaatioiden 10. ja 90. persentiilin välinen alue.
- **Hallituspohjien** paikkamäärä lasketaan jokaisessa simulaatiossa erikseen puolueiden yhteenlaskettuna paikkamääränä. Hallitusten paikkamääriä arvioivassa kuviossa näkyvä luku on näiden summien keskiarvo, ja se voi pyöristyksen vuoksi poiketa yhdellä paikalla puolueiden pyöristettyjen ennusteiden summasta.
- **Punainen viiva** hallituspohjien kuvassa on enemmistön raja: enemmistöön tarvitaan 101 paikkaa 200:sta, käytännössä toimivan enemmistöhallituksen kasaamiseen on historiallisesti vaadittu runsaampi enemmistö.

## Mitä ennuste ei ota huomioon

Todennäköisyysvälit kuvaavat mittausten otantavirhettä ja vaalipiirien satunnaista vaihtelua. Ne eivät sisällä seuraavia epävarmuuden lähteitä, joten todellinen epävarmuus on välejä suurempi:

- **Mittausten järjestelmällinen virhe.** Jos kannatusmittaukset yli- tai aliarvioivat jonkin puolueen kannatusta, ennuste perii saman virheen.
- **Kannatuksen muutokset ennen vaaleja.** Ennuste kuvaa tilannetta mittausten aikaan.

## Usein kysyttyä

**Miksi puolueiden paikat summautuvat 199:ään eivätkä 200:aan?**  
Ahvenanmaan vaalipiiri valitsee yhden kansanedustajan, eikä sen tulosta voi arvioida valtakunnallisista mittauksista. Se on jätetty laskelman ulkopuolelle, Ahvenanmaan edustaja istuu perinteisesti RKP:n eduskuntaryhmässä.

**Arvioin, että pienpuolueen ehdokkaiden henkilökohtainen kannatus on suurempi kuin mittaukset antavat olettaa. Huomioiko ennuste sen?**  
Ei suoraan. Ennuste perustuu valtakunnallisiin puoluekannatusmittauksiin. Vaalipiirikohtainen satunnaisvaihtelu jättää tilaa yksittäisten ehdokkaiden ja paikallisten tekijöiden vaikutukselle, mutta ennuste ei tunnista, kenen ehdokkaat menestyvät tavallista paremmin. Ennusteen heikoin kohta ovat siksi puolueet, joiden paikat riippuvat muutamasta vahvasta ehdokkaasta.

**Huomioiko ennuste vaaliliitot?**  
Ei automaattisesti. Vaaliliitot voivat ratkaista yksittäisiä paikkoja erityisesti pienille puolueille, mutta niiden vaikutusta ei voi arvioida valtakunnallisista mittauksista. Kun (eduskuntapuolueiden) vaaliliittoja julkaistaan, Databyro pyrkii kuitenkin estimoimaan vaaliliiton vaikutusta kyseisessä tai kyseisissä piireissä.

## Tarkkuus

Databyron paikkaennusteen osumatarkkuus aiemmissa eduskuntavaaleissa on koottu [Tarkkuus-sivulle]({{ '/tarkkuus/' | relative_url }}).

## Muutosloki
- 

</div>
