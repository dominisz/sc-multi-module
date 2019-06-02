# Wielomodułowy projekt mavenowy

## Opis projektu

Repozytorium zawiera kod źródłowy wielomodułowego projektu mavenowego. W skład projektu wchodza następujące moduły:
- główny katalog zawiera parent pom
- katalog `library-one` zawiera projekt mavenowy z implementacją niezbędnej biblioteki
- katalog `library-two` zawiera projekt mavenowy z implementacją drugiej niezbędnej biblioteki
- katalog `application` zawiera główną aplikację, aplikacja wykorzystuje klasy z dwóch bibliotek

## Budowanie projektu

- wywołanie polecenia `mvn package`/`mvn install` w głównym katalogu powoduje zbudowanie wszystkich podmodułów i utworzenie artefaktów (i ewentualne zainstalowanie w lokalnym repozytorium)
- artefakty można również budować niezależnie od siebie wywołując `mvn package`/`mvn install` w poszczególnych podkatalogach