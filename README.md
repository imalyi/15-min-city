# 15_minutescity

Celem projektu "Miasto 15-minutowe" jest stworzenie aplikacji internetowej, która pomoże mieszkańcom konkretnego miasta lub obszaru w łatwym i wygodnym dostępie do podstawowych usług, miejsc pracy, edukacji, rozrywki oraz innych istotnych punktów w ich codziennym życiu. Głównym celem jest zapewnienie, aby większość tych punktów była dostępna pieszo w ciągu 15 minut.

Aplikacja będzie składać się z trzech głównych komponentów: panelu administratora, panelu użytkownika i backendu do przechowywania danych, zbierania nowych informacji o miejscach publicznych oraz wyszukiwania najbliższych punktów.

Panel administratora(https://github.com/imalyi/google_maps_parser_api) będzie służyć do tworzenia zadań dotyczących zbierania danych z Google Maps Places API. Ze względu na koszty dostępu do danych, niemożliwe jest natychmiastowe zebranie wszystkich informacji o wszystkich miejscach publicznych w kraju. Administrator będzie miał możliwość wprowadzania koordynatów miejsca, promienia oraz kategorii miejsc, które mają zostać zebrane. Lista dostępnych kategorii jest dostępna pod linkiem https://developers.google.com/maps/documentation/places/web-service/supported_types

Interfejs użytkownika w formie strony internetowej pozwoli użytkownikowi wprowadzić swój adres domowy. Po wprowadzeniu adresu, użytkownik zobaczy, czy miejsca publiczne w kategoriach takich jak sklepy, placówki edukacyjne, banki, przychodnie, itp., są dostępne w ciągu 15 minut pieszo. Dodatkowo, użytkownicy będą mieli możliwość zapisania się do newslettera informującego o nowych miejscach w ich okolicy oraz przeglądania opinii o miejscach w ich okolicy z ostatnich 3 miesięcy.

Po zebraniu danych, aplikacja wykorzysta informacje z OpenStreetMaps i OpenStreetAddress, aby obliczyć najkrótsze trasy z każdego budynku do każdego miejsca publicznego w promieniu 3 km. Dane te będą przechowywane w bazie danych, takiej jak PostGIS lub Neo4j, i wykorzystywane do generowania odpowiedzi na zapytania użytkowników.


Zespół:
1. Ihor Malyi (lider)
2. Artsem Stankevich



![Diagram](https://github.com/imalyi/15_minutescity/blob/main/Untitled-2023-11-08-1551(3).png?raw=true)
