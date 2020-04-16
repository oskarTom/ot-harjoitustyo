![Julia Set](https://github.com/oskarTom/ot-harjoitustyo/blob/master/images/Julia%202.png)

# Julian joukot
Ohjelma kuvaa valitulle kompleksiluvulle vastaavan Julian joukon. Kompleksiluku valitaan painamalla jotakin pistettä Mandelbrotin joukosta tai sen lähettyviltä.

Projekti on toteutettu hakemistoon Fraktaalit.

## Dokumentaatio
[Vaatimusmäärittely](https://github.com/oskarTom/ot-harjoitustyo/blob/master/Dokumentointi/Vaatimusmaarittely.md)

[Työaikakirjanpito](https://github.com/oskarTom/ot-harjoitustyo/blob/master/Dokumentointi/tuntikirjanpito.md)

[Arkkitehtuurikuvaus](https://github.com/oskarTom/ot-harjoitustyo/blob/master/Dokumentointi/arkkitehtuuri.md)

## Releaset
[v1.1](https://github.com/oskarTom/ot-harjoitustyo/releases/tag/v1.1)

[v1.0](https://github.com/oskarTom/ot-harjoitustyo/releases/tag/v1.0)

## Komentorivitoiminnot
### Testit
Testien suorittaminen toteutetaan komennolla

    mvn test
Testikattavuusraportin luominen tapahtuu komennolla

    mvn test jacoco:report
Kattavuusraporttia voi tarkastella avaamalla tiedosto *target/site/jacoco/index.html* selaimessa
### Jar
Jarin generointi onnistuu komennolla

    mvn package
    
Jar luodaan kansioon *target/* ja sen voi suorittaa komennolla

    java -jar target/Fraktaalit-1.0-SNAPSHOT.jar
### Checkstyle
Ckeckstyle tarkistus suoritetaan komennolla

    mvn jxr:jxr checkstyle:checkstyle
Tulokset näkyvät tiedostossa *target/site/checkstyle.html*
