# Opis projektu #

W projekcie tym tak jak poprzednio znajduje się minimalny kod wyjściowy.
- plik crawler.php -> zapisuje content strony w bazie danych w tabeli "SitesViewed" oraz linki w tabeli "SitesAwaiting"
- plik create_db.php -> tworzy bazę oraz tabele
- plik rest.php!! (nowość) -> póki co zwraca wszystkie wiersze z tabeli SitesViewed w formacie JSON, ale powinien zwracać tylko te które zawierają w kolumnie "content" wyrażenie przekazane za pomocą parametru "search" w URL'u (metodą GET)

### User story: ###

Co to jest user story?! [Link](https://en.wikipedia.org/wiki/User_story)

- Użytkownik wchodzi na stronę wyglądającą jak strona wyników wyszukiwania google.com
- Użytkownik ma możliwość wpisywania tekstów w pole search'a
- Użytkownik po naciśnięciu przyciusku enter otrzymuje wyniki wyszukiwania na tej samej stronie widząc:
	- wyniki wyszukiwania dla wpisanej frazy
	- znalezione teksty wyników nie muszą być pogrubione
	- wyniki powinny mieć długość do 3 linii (jak w google) - reszta obcinana
	- powinien być widoczny url strony na której dany tekst został znaleziony
- Użytkownik ma możliwość zmiany tekstu w polu search
- Po zmianie i naciśnięciu enter odświeża się lista wyników wyszukiwania

### Techniczne rozwiązanie: ###

- Należy stworzyć stronę wyników wyszukiwania google
- Należy rozbudować plik rest.php aby zwracał wyniki tylko dla przekazanej frazy
- Należy użyć AJAX lub [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)
- Można wykorzystywać po stronie JS biblioteki jakie się tylko chce
- Do tego zadania dla osób które nie używały dużo JS'a zalecany jest zwykły najprostszy [jQuery](https://jquery.com/)


### Punktacja: ###

- 200pkt za skończenie zadania ze zrealizowanymi funkcjonalnościami
- nie ma punktów za pull request
- każdy pracuje na swoim repozytorium
- można uzyskać uścisk dłoni od prowadzącego ćwiczenia za zgłoszenie pull requesta do błędów stylistycznych/językowych/ortograficznych

### Negocjacje: ###

- Jeżeli któryś punkt wydaje się być za skomplikowany można poprosić prowadzącego o doimplementowanie
- Zrobienie MySQL SELECT ... LIKE ... nie należy do rzeczy "za skomplikowanych"