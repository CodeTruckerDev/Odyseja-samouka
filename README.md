# Odyseja-samouka

Z góry uprzedzam, to będzie długa opowieść, bez skrótów typu TL;DR

## PROLOG

Urodziłem się w roku 1980, a w moich latach młodzieńczych imponowała mi postać pewnego znanego ówcześnie człowieka. Był nim Kevin Mitnick. 
I to, co postrzegałem za niesamowite w tejże postaci był fakt, że wszystkiego się nauczył i co opanował, dokonał tego samodzielnie. 
W ten właśnie sposób narodził się pomysł, że skoro on nauczył się czegoś sam, to i ja dam radę samodzielnie nauczyć się pisania programów komputerowych.

Jako szkołę średnią wybrałem technikum elektroniczne ze specjalnością "Systemy komputerowe", jednak niestety nie znalazłem tam informacji, dzięki którym mógłbym
rozpocząć naukę programowania. Jedyna tematyka zajęć dodatkowych, która wywarła na mnie wielkie wrażenie dotyczyła systemu operacyjnego UNIX. 
Wtedy poznałem pierwsze komendy tego systemu, co było zalążkiem miłości do systemów operacyjnych opartych na jądrze Linuxa. 

Nie znając totalnie nikogo, kto mógłby mi pomóc - sam na własną rękę postanowiłem że zawalczę z tematem programowania. I tak na warsztat wziąłem język Turbo Pascal. 
Mozolnie wklepywałem pierwsze komendy, jednak gdy nastąpił pierwszy poważniejszy problem (o ile dobrze kojarzę była to pętla for) nie mogąc zrozumieć tematu uznałem, 
że to chyba jednak nie jest dla mnie. I temat programowania poszedł w kąt. 

Jednak po kilku miesiącach zapragnąłem spróbować ponownie. I skoro Turbo Pascal sprawiał mi trudności, stwierdziłem że użyję czegoś innego. Gdy jednak doszedłem do tego samego
momentu blokady, znając już wcześniejszy sposób ponownie uznałem że programowanie nie jest dla mnie. Ileż ja się namęczyłem z ++i oraz i++ (z minusami także). 

I tak co kilka miesięcy podejmowałem próby z kolejnymi językami programowania, jednak brak konkretnie wskazanej specjalizacji czy kierunku owocował w kolejnych momentach, 
gdzie porzucałem temat nauki programowania. A po pewnym czasie stwierdziłem, że już chyba całkowicie nie mam co się z tym męczyć. I odpuściłem niemal na zawsze.

W takiej nudnej codziennej monotonności dotrwałem do roku 2016, gdzie pojawiła się żona, dwoje dzieci i cała masa problemów życia codziennego. Starsze dziecko - syn - miał wtedy 11 lat
i jak wiele dzieciaków z tamtego czasu, miał poważny problem z ilościa czasu jaki spędzał przy komputerze grając. Problem był istotny, bo syn miał komputer u siebie w pokoju i bywało,
że wstawał w nocy i grał. Zakładanie hasła na komputer niestety nie było opcją, gdyż moja lepsza połowa nie chciała mieć z komputerami nic do czynienia. A ja będąc w pracy czy gdziekolwiek
indziej nie byłbym w stanie odblokować komputera. Zacząłem więc poszukiwania aplikacji do nadzoru ile dziecko może spędzić przy komputerze. A wtedy w roku 2016 nie było jeszcze zbyt wielu 
możliwości. Wszelkie polskojęzyczne aplikacje nie spełniały mojego założenia, a pozostałe które znalazłem były płatne w dolarach, co dla mnie wtedy było problemowe.

Zrobiłem więc ranking języków programowania, wybrałem Pythona i rozpocząłem naukę z tutoriali dostępnych na platformie YouTube. Jednak po pewnym niedługim czasie zauważyłem, że tutoriale te 
oczywiście pokazują użycie komend ale nie uczą praktyki. Opracowałem więc własny sposób nauki. Zarejestrowałem się na oficjalnym forum Pythonowym i korzystając z pytań, które zgłaszali studenci
zgłębiałem wiedzę dotyczącą tego języka. Googlałem tematy, przeprowadzałem testy na swoim komputerze, po czym dawałem odpowiedź. Nigdy nie dawałem gotowca, dawałem podpowiedzi naprowadzające na
odpowiedź wraz z odnośnikami do źródeł. Tak więc pytający byli zadowoleni, i ja także.

I w tym właśnie momencie uznałem, że napiszę taką aplikację sam. To jest początek prawdziwej opowieści.

## ROZDZIAŁ 1 - GUARDIAN

Wracając do problemu z synem, zaprojektowałem aplikację oraz sposób jej działania, po czym napisałem kod - oczywiście nie od razu zadziałało jak chciałem - jednak koniec konców aplikacja powstała. 
I była ona stosunkowo prosta - na starcie komputera do pliku tekstowego była dopisywana aktualna data, po czym trzy ostatnie wpisy były porównywane. Jeśli zapisy były różne, młodzieniec mógł 
korzystać z komputera przez godzinę, po upływie której komputer samoczynnie się wyłączał. Jeżeli natomiast zapisy dat były takie same komputer wyłączał się po jednej minucie. W ten sposób syn mógł 
grać dwa razy po jednej godzinie, a pozostała minuta została stworzona aby całkowicie nie zablokować komputera - żeby w razie potrzeby móc aplikację zatrzymać. Obecny kod został przerobiony do 
pliku exe i trafił do autostartu Windowsa. Jako że skrypt był napisany jako narzędzie konsolowe przy starcie systemu na ułamek sekundy pojawiało się okienko CMD, co niestety rodziło zagrożenie. 
Wystarczyłoby wiedzieć gdzie dokładnie na monitorze wyświetla się X zamykający okno CMD i cała aplikacja przestałaby działać zanim by jeszcze zdążyła się uruchomić. Tu na pomoc przyszło oczywiście 
Google a rozwiązaniem okazał się skrypt VBS ukrywający okno aplikacji. 

Guardian 1.0 [link]

W ten oto sposób stałem się wrogiem publicznym numer jeden mojego syna, który nie ustępował w wysiłkach jak obejść moją aplikację. Sam próbował, próbowali jego koledzy, starsi bracia jego kolegów
oraz koledzy starszych braci. Nikt nie potrafił się z Guardianem uporać. Byłem zadowolony nie zdając sobie sprawy, jak szybko odkryję najsłabsze ogniwo mojej aplikacji. 
Po kilku tygodniach 'życia' aplikacji zaobserwowałem zestaw zachowań u młodzieńca. Otóż znikał na pół godziny w swoim pokoju, po czym wychodził na dwór na kilkanaście minut, i wracał do pokoju.
I tak wiele razy. Oczywiście zastanowiło mnie to zachowanie, więc w wolnej chwili uruchomiłem jego komputer i gdy sprawdziłem plik z zapisanymi datami doznałem szoku. Syn zhakował moją aplikację.
Po każdym uruchomieniu komputera zmieniał rok, co dawało mu nieograniczony ilościowo dostęp do komputera. Gdy zacząłem go wypytawć jak tego dokonał, powiedział że podsłuchał jak któregoś razu
chwaliłem się znajomemu zasadą działania mojego programiku. Więc tym najsłabszym ogniwem aplikacji okazałem się być ja sam. 
To było istotne doświadczenie, w wyniku którego postanowiłem podjąć się wyzwania jakim było usprawnienie aplikacji. Zacząłem więc obserwować mojego syna i bardzo szybko doszedłem do wniosku, że 
dla niego komputer bez dostępu do internetu to tylko sterta złomu, bo jego rozrywka opierała się na grach on-line. Zebrawszy wywiad przysiadłem ponownie do klawiatury i wykorzystując pozyskaną
wiedzę stworzyłem Guardiana w wersji 2.0. Zasada działania nowszej wersji była podbna do wersji 1.0 jednak z pewnym usprawnieniem. Aplikacja będąc w autostarcie Windowsa sprawdzała, czy jest już
aktywne połączenie z internetem. Jeśli połączenia nie było, czekała 5 sekund po czym sprawdzała ponownie aż do skutku. Gdyby internetu nie było komputer zostałby wyłączony przez samego użytkownika.
W momencie gdy połączenie z internetem było aktywne, aplikacja pobierała aktualną datę z internetu, po czym zapisywała do pliku tekstowego i reszta działała już po staremu. I powstało dzieło idealne.
Nie pomagały już wszelkiego rodzaju różne próby jej przełamania. I Guardian 2.0 działał przez kilka miesięcy, po których młody haker naoglądał się filmików pokazujących jak podkręcać wydajność 
procesora i karty graficznej zworkami na płycie głównej. W ten oto sposób spaliła się i karta graficzna i zasilacz. A później przez pewien czas nie mieliśmy możliwości zdobycia nowego komputera
dla overlockera, a gdy już się udało go zdobyć, niedługo po tym rozpoczęła się pandemia covid19 i było lepiej żeby młody siedział w domu i grał bez ograniczeń. W ten oto sposób moja aplikacja
umarła śmiercią naturalną, gdyż nie było już dla niej zastosowania.

Guardian 2.0 [link]

## ROZDZIAŁ 2 - EKSPLOZJA KREATYWNOŚCI

Równolegle z wydarzeniami kiedy tworzyłem Guardiana zacząłem się uczyć kolejnych rzeczy. Każdy projekt który zaczynałem skupiał się na pewnych cechach aplikacji. Co istotne, każdy rozpoczęty 
projekt postanowiłem doprowadziać do końca za wszelką cenę, żeby ta nauka była wymierna. Testowałem wszelkie tematy, w których widziałem jakiekolwiek zastosowanie. Co oczywiście jako samouka
poprowadziło drogą pomijającą pewne zagadnienia. Ale ciągle odczuwając że się uczę miałem myśli, że kiedyś gdy będę potrzebował to nauczę się wszystkiego. Ale nawet zwykłe zagadnienia 
potrafiłem ubrać w ciekawe i zabawne skrypty. Przykładem jest poniższy kod.

Three [link]



