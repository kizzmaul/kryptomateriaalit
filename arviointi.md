# Kryptonvaluutan tai poletin nimi

- Kaikkiin kysymyksiin on vastattava. Jos ei ole tietoa, niin kirjoittaa ettei ole tietoa. Tämä siksi, että tyhjä kenttä voi implikoida sitä ettei ole koskaan sanonut ettei tiedä vastausta johonkin. Näin ei voi välttää vastuuta kysymyksistä.
- Johdantoon ja tekniseen osuuteen EI SAA laittaa mitään hypoteettista, vaan ainoastaan asioita jotka ovat jo olemassa ja toiminnassa. Hypoteettiset asiat voi laittaa sitten tulevaisuuden suunnitelmiin.
- Valehteluun nollatoleranssi.
- Ei linkkejä mihinkään ostopaikkoihin, tämän on tarkoitus olla vain infopläjäys.
- Ei hintaspekulointia.
- Mielellään lähde jokaiseen vastaukseen. Jos yksi lähde (esim. valkopaperi) vastaa useampaan kysymykseen, eritellään sivu JA kappale/virke.
- Jokaiseen kysymykseen vastataan erikseen.
- Asiat ei aina ole mustavalkoisia, mutta aivan kaikki pitää perustella.
- Kaikki vastaukset Suomen kielellä.

## Johdanto
- Mikä on tämän krypton ydinsanoma, mitä ongelmaa se yrittää ratkaista?
- Mitä uniikkia juuri tässä kryptovaluutassa on, mitä muut ratkaisut ei tarjoa?
    - parametrin tuunaaminen ei ole uniikki ominaisuus. esim. kilpailijalla jokaisesta siirrosta menee kehittäjille 3% versus tässä vain 0.5%
    - "Voi käyttää meidän palvelun ostamiseen" on relevanttia vain silloin kun kyseistä palvelua ei voi ostaa muulla tavalla kuin kyseisellä kryptolla. Muutenhan juuri tämä krypto ja sen maksuvälineominaisuus ei olisi uniikkia.
- Millainen kohderyhmä kryptolla on?
- Ketkä tätä kryptoa kehittää (jos tiedossa)?
- Miten kehitystä on rahoitettu, jos ollenkaan, ja onko rahoitus 100% turvattu pidemmäksi aikaa?
- Onko ulkopuolisten mahdollista jatkaa kehitystä, jos alkuperäiset kehittäjät eivät ole enää kiinnostuneita?
- Millaisia riskejä tämä krypto sisältää? Millaisia kilpailijoita tällä kryptolla on?
    - esimerkiksi "on mahdollista tulkita, että krypto on arvopaperi"
- Millainen yhteisö on krypton takana?
    - ei mitään linkkejä mihinkään TG-kanaville tmv, vaan ihan normaalia selkokieltä suoraan vastaajalta. 
- Millaisilla mekanismeilla varmistetaan, että kerätty rahoitus menee vain ja ainoastaan itse kehityksen rahoittamiseen eikä jonkun takataskuun?

## Tekninen osuus
Yhteiset kysymykset
- Mistä voi nähdä lähdekoodin?
- Onko kehitystyö avointa siten, että kuka tahansa voi osallistua siihen esimerkiksi githubin kautta?
- Jos kehittäjät ja kaikki heidän omistamat tietokoneet/palvelimet katoaisivat nyt, niin täyttäisikö krypto edelleen arvolupauksensa? 
    - Esimerkiksi Uniswap täyttää, sillä heidän älysopimus on käytettävissä Ethereumin lohkoketjusta käsin vaikka nettisivu olisi poissa. Likviditeettialtaat olisivat edelleen olemassa ja käytettävissä.
- Onko kryptolla mitään keskitettyä kipupistettä, joka olisi hajautetun eetoksen vastainen? Kts. seuraavat esimerkit
    - Iota: keskitetysti hallittu koordinaattorisolmu, jota ilman se ei toimi
    - BSC: ainoastaan Binancen valitsemat entiteetit voi ylläpitää validaattoreita.
    - Storj: keskitetyt relay solmut. 
- Onko jonkun muun kuin yksityisen avaimen omistajan mahdollista rajoittaa krypton lähetystä/vastaanottamista?

Näistä valitaan vain toinen.
- Kyseessä on poletti (esim. ERC20)
    - Missä verkossa poletti sijaitsee? Jos poletti sijaitsee useassa eri verkossa, niin onko sille jotain erityistä syytä? Jos syy on se, että toisessa verkossa on halvemmat transaktiokustannukset, ja se on oleellista että on halvat transaktiokustannukset, niin mikä virka on sillä versiolla poletista, joka on kalliimmassa verkossa?
    - Millä mekanismilla polettia jaetaan, onko niitä esimerkiksi mahdollista ansaita jotenkin (esimerkiksi ylläpitämällä hajautettua tiedostonjakosolmua) vai onko niitä aivan pakko ostaa? Jos on pakko ostaa, niin kuka on ensisijainen myyjä? Kuka oli ensimmäinen likviditeetin tarjoaja, ja mihin tarkalleen ottaen tällaisesta toiminnasta saadut varat menee?
    - Kuinka voin varmistaa, että älysopimuksen osoitteessa todella sijaitsee aikaisemmin mainitusta lähdekoodista käännetty sovellus?
        - tämä voi olla triviaalia ainakin Ethereumin tapauksessa, jolloin kehittäjä voi lähettää lähdekoodin sivulle ja sivu voi sitten tarkistaa, että tosiaan tämä versio tästä sovelluksesta pyörii tässä osoitteessa
    - Jotkut kehittäjät tekevät siten, että julkaisevat poletin ja myöhemmin tekevät uuden poletin johon voi sitten vaihtaa aikaisemmasta (esimerkiksi siksi, ettei aikaisempi poletti sisältänyt kaikkia ominaisuuksia). Tämä ei välttämättä ole pahantahtoista, mutta vaatii ehdottomasti selvitystä. Onko tämä poletti sellainen, joka päivitetään myöhemmin uuteen? Jos on, niin onko mahdollista, että vaihto on pakko suorittaa tietyn aikamääreen sisällä? Millä mekanismilla vaihto tulisi tapahtumaan? Miksi nykyinen poletti tehtiin, jos se kuitenkin joudutaan myöhemmin vaihtamaan?
- Kyseessä on itsenäinen lohkoketju/suunnattu verkko (DAG)
    - Mitä konsensusmekanismia on käytetty?
    - Onko kryptoa mahdollista saada ilman, että joutuu ensin antamaan rahaa toiselle?
        - esimerkiksi louhimalla
    - Kuvaile krypton hajautuneisuutta muutamalla lauseella seuraavissa konteksteissa:
        - solmujen ylläpitäjät
        - louhijat/validaattorit
        - muut entiteetit
    - Tukeeko älysopimuksia? Jos tukee, niin onko ne Turing-täydellisiä?
    - Jos DAG-pohjainen, niin onko verkon toiminta riippumaton jostain keskitetysti jaetusta solmulistasta? 
        - Esimerkiksi Ripple antaa solmulistan validaattoreille. Suunnatut verkot tuppaavat menemään epätasaiseksi ja suorituskyky heikentyy, jos yhdistää epäoptimaalisiin solmuihin.
    - Onko verkon ylläpitämiseen osallistuminen jollain tavalla teknisesti rajoitettua?
        - Esimerkiksi Bitcoinissa on 1 megatavun lohkot, jolloin heikompikin rauta voi osallistua solmun ylläpitoon ja näin lisätä hajautuneisuutta. Tämä on tärkeä ominaisuus kryptovaluutassa.


## Tulevaisuuden suunnitelma
- Mihin suuntaan tätä kryptoa aiotaan kehittää tulevaisuudessa?
- Millä aikataululla?
