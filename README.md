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
poprowadziło drogą pomijającą pewne zagadnienia. Ale ciągle odczuwając że się uczę miałem myśli, że kiedyś gdy będę potrzebował to samodzielnie nauczę się wszystkiego. 

Ale nawet zwykłe zagadnienia 
potrafiłem ubrać w ciekawe i zabawne skrypty. Przykładem jest poniższy kod.

Three [link]

Moja świętej pamięci mama była księgową, a ja sporo jej w tym pomagałem. Wszędzie tam, gdzie trzeba było się podpisać widniał jej podpis a do mnie należało sprawne działanie komputera i oprogramowania
wraz z jego obsługą. Wiele razy widziałem sytuacje, gdzie z wartości z paragonu bądź faktury mama wyliczała wartość podatku VAT. Zawsze ręcznie. I tu ujrzałem możliwość pomocy. Napisałem jej
malutkie narzędzie do wyliczania wartości podatku z podanej przez użytkownika wartości brutto dokumentu finansowego. I mama była zadowolona. Niestety pokonał ją covid, a narzędzie trafiło do szuflady,
jako już nikomu nie potrzebne.

Obliczacz-VAT [link]

Kontynuując naukę poprzez forum, które stało się moim swoistym cyfrowym domem, zbierałem punkty reputacji, które wtedy miały dla mnie znaczenie, bo utwierdzały mnie w przekonaniu, że robię dobrą robotę.
W tak zwanym międzyczasie rozwijając skile podstawowej biblioteki Pythona zostałem poproszony o napisanie, a właściwie o propozycję napisania aplikacji do sprawdzania numeru PESEL. Kod miał być częścią
większego systemu. A ja tak sobie wziąłem do serca to zlecenie, że wykorzystując biblioteki tkinter napisałem samodzielny tester numeru PESEL.

PESEL-tester [link]

Innym razem ujrzałem możliwość pomocy mojej teściowej, która będąc zapaloną graczką gier Lotto co kilka dni wieczorem sprawdzała wylosowane numery korzystając z telegazety w telewizorze. Do tej pory gra
stałymi numerami. I wtedy pomyślałem nad narzędziem, które samo pobrałoby numery losowania ze strony lotto i sprawdzenie, czy stałe, nazwane przeze mnie złotymi liczbami strzały były trafione w danym
losowaniu. Całość została ubrana w proste okienko stworzone oczywiście w tkinter, który w tamtym momencie był celem. Określiłem swój cel na tworzenie aplikacji okienkowych.

Multi-Multi-złote-liczby [link]

Ucząc się zaczynałem miewać pomysły, jakoby zawodowe programowanie mogłby być moim celem. I na potrzeby zaprezentowania siebie stworzyłem swoją wizytówkę. I tak jak w poprzednich przypadkach padło na
tkinter. Aplikacja korzysta z tajemnych mocy, aby znaleźć odpowiedniego kandydata. I pomimo, że aplikacja powstała w wersji finalnej jako plik wykonywalny exe, nigdy jej nikomu nie pokazałem.
Toczyłem wewnętrzną walkę o wiarę we własne siły oraz projekty i niestety brak wiary w siebie wygrał, zresztą jak zazwyczaj. Tak czy inaczej poniżej można zobaczyć, jak wyglądała moja wizytówka.

Super-secret-searcher [link]

Gdy tworzyłem Guardiana, miałem pomysły żeby była mmożliwość odblokowaa Windowsa własnym hasłem, czyli żeby system przez kilka minut po osiągnięciu maksymalnego czasu korzystania z komputera wyświetlał okienko 
z możłiwością wpisania hasła, które pozwalałoby na dalsze korzystanie z komputera. Finalnie nie zastosowałem tego rodzaju rozwiązań, jednak ten sposób zabezpieczania aplikacji stał się trzonem
mojego procesu nauki oraz rozważań teoretycznych i praktycznych. Zastanawiałem się nad ukrytymi i nieoczywistymi rozwiązaniami, które wymagają od użytkownika interakcji ażeby w pewien sposób rozwiązać 
zagadkę i wpisać prawidłowe hasło. I przy tym projekcie realizowałem także naukę importów zewnętrznych modułów. Stworzyłem więc aplikację, w której w górnej części okienka (ofc tkinter) wyświetlał się napis
"You won't find my magic code" i należo zwrócić uwagę na słowo 'magic', które było trzeba wpisać w specyficzny sposób. Zachęcam do sprawdzenia. Miłej zabawy :)

Magic [link]

Wspomniałem wcześniej o powstałej miłości do Linuxów. Od wielu lat używam ich w codziennej pracy na komputerze. Przetestowałem kilka dystrybucji i chyba idąc standardową ścieżka dla zapaleńców, najpierw
korzystałem z Ubuntu. Dosyć krótko, bo denerwowała mnie ilość niepotrzebnego oprogramowania dostarczanego wraz z systemem operacyjnym. Ale nie tylko to sprawiło, że zacząłem szukać wyzwań. Wraz z samą obsługą
narodziła się pasja do korzystania z terminala. Zacząłem się więc uczyć pisania skryptów bash, a później podstawowych narzędzi systemów operacyjnych z rodziny *nix. W ten oto sposób obsługa komputera
bez odrywania rąk z klawiatury zaczęła mnie interesować bardziej. Zmieniłem standardowe dla Pythona IDLE na rzecz VIMa. Z Ubuntu przeskoczyłem na Manjaro, a później na Archa ze środowiskiem i3. I w nim 
spędzałem cały czas jaki miałem za zabawę związaną z komputerem. Zabawę, ponieważ nauka tego wszystkiego zastępowała mi klasyczną rozrywkę jaką są gry. Nie potrzebowałem gier. Całkowicie wystarczało mi
rozwiązywanie 'zadań' logicznych związanych z obs\lugą systemu operacyjnego.

Po zapoznaniu się z większością systemu, jednak w stopniu tylko pdstawowym, gdyż jest tego zbyt wiele a ja mając ograniczone zasoby czasu musiałem decydować ile i czego się uczyć - zwróciłem uwagę na kolorowanie
składni tekstu wyświetlanego w terminalowym okienku. Tak narodził się pomysł nawiązujący do poprzedniej aplikacji na napisanie skryptu w Pythonie. To był taki mój 'protoplasta' AI. Głównym założeniem aplikacji
było wykorzystanie losowości w utworzeniu znaków hasła, a następnie pokolorowaniu tych znaków jednym z określoną listą kolorów. Aplikacja ta miała w swoim założeniu wykorzystywać interakcję użytkownika i jego
zdolność do obserwacji i rozwiązywania zagadek. W mojej apce wyświetlał się napis sugerujący że słowa te 'wypowiada' sztuczna inteligencja, a były to słowa "You can't STOP me". Istotnym elementem jest słowo STOP.
A dkładniej kolor znaku drogowego, oznaczającego stop - czyli koloru czerwonego. I w wygenerowanym losowo i losowo pokolorowanym ciągu znaków, hasłem były tylko znaki w kolorze czerwonym. I jak w poprzednim przypadku
zachęcam do samodzielnego wypróbowania. Windows 11 posiada już wbudowaną obsługę kolorów ANSII wykorzystaną w tym projekcie, więc nie trzeba już zaglądać do Linuxowego terminala, który mimo wszystko odstrasza
większość użytkowników. Projekt nazwałem roboczo "Project X" i tak już zostało. Ale projekt ten stał się zalążkiem tego, co stworzyłem 8 lat później.

Project-X [link]

Ciągle się ucząc nowych rzeczy, odwiedziłem pewną stronę której temat przewodni w tamtym czasie spowodował, że się zatrzymałem i zacząłem się zastanawiać nad moim procesem nauki. Była tam informacja o rozpoczynającym 
się niebawem konkursie programistycznym. Oczywiście z nagrodami. Na podjęcie ewentualnej decyzji miałem nie więcej niż dwie godziny. I stwierdziłem, że chcę zobaczyć, jak taki konkurs wygląda od środka. Zgłosiłem się 
więc z projektem, który w tamtym czasie wydawał mi się istotnym. Otóż mój syn, ten sam na którym przetestowałem Guardiana, miał problemy z ortografią. Nic specjalnego, sytuacja jak w wileu domach. A ja wtedy wymyśliłem,
że pomimo że na rynku były aplikacje do nauki ortografii - że napiszę własną, opierającą się na moich pomysłach. Głównymi założeniami konkursu oprócz oczywiście rozwoju projektu było prowadzenie bloga, który tygodniowo
miał być zasilany dwoma wpisami - jednym dotyczącym aktualnie rozwiązywanego tematu aplikacji, oraz drugim, który mógł dotyczyć czegokolwiek. Całość oparłem oczywiście na znanym już mi tkinter. 

I po pewnym czasie doszedłem do tak zwanej ściany, nie mogąc wymyślić rozwiązania. Kontaktowałem się z prowadzącym konkurs z informacją że rezygnuję. Zresztą patrząc z perspektywy czasu rezygnacja była moją obroną przed 
porażka. Robiłem tak wiele razy już kiedyś, i zrobię w przyszłości - o czym napiszę poniżej. W każdym bądź razie organizator konkursu próbował wspierać mnie w moim przedsięwzięciu sugerując żebym się nie poddawał.
I przez pewien czas odpuściłem. Nie prowadziłem bloga i siłą rzeczy nie spełniając głównego założenia konkursu nie dostałem się do części finalnej. I tak nie liczyłem na nagrody. Jednak słowa Pana Macieja (bo tak ma na
imię ów twórca tamtego konkursu) spowodowały, że nie ugiąłem się i nie położyłem całkowicie projektu. 

Korzystając z forum, na którym wtedy byłem już troszkę znany poprzez punkty reputacji, skontaktowełem się ze stowarzyszeniem Pythonowym - PLPUG. Owe stowarzyszenie wspierało różne projekty związane z rozwojem dzieci, i 
mój "Mistrz ortografii" idealnie tam pasował. Umówiłem się na rozmowę na żywo na jednym ze spotkań PyWaw organizowanym w Warszaawie. Pojechałem pełny niepewności, czy pasuję do tego środowiska. W końcu byli tam zawodowcy.
Albo kandydaci na zawodowców (studenci). I zostałem pochwalony za pomysł. Uzyskałem też pewną pomoc, która stała się także wyznacznikiem moich przyszłych projektów. Nikt mi wtedy nie mówił co i jak mam pisać, ale 
dowiedziałem się że w takich przypadkach najlepiej jest zrobić kilka kroków wstecz, i zacząć pisać kod w sposób inny do tego co już zostało napisane. I to rzeczywiście zadziałało. I finalnie, pomimo że nie spełniałem już 
obowiązku pisania bloga, mój projekt został zakończony sukcesem. I tak zapewne gdybym się dostał do finału nic bym nie wygrał. Ale wygrałem za to troszkę wiary w siebie.

I tak niemal zakończyła się historia z tym projektem. Ale nie do końca. Ponieważ udało mi się z tejże aplikacji kilka razy korzystać. Otóż, gdy do mojego syna przyjeżdżali znajomi, zawsze padało pytanie z prośbą o hasło
do Wifi. I ja wtedy mówiłem: dobrze, nie ma problemu. Ale najpierw zerknijcie, mam tu taką aplikację. Jeśli osiągniecie stu procentową skuteczność po dwudziestu słowach - podam wam hasło. I dzieciaki walcząc o hasło
uczyły się przy okazji. Finalnie aplikacja była krótko przeze mnie używana, ale co było moim niesamowitym sukcesem sprzedałem (za niewielkie pieniądze) tę aplikację jednej osobie dla jego dzieci :)

Mistrz-ortografii [link]

Wszystkie powyższe aplikacje z tego zordziału były dziełem roku 2017. I mając kontakt z Panem Maciejem co kilka tygodni wymienialiśmy informacje, za pomocą których trafiłem także jako wpis na jego bloga. 

Jednak nastąpiło coś, czego się nie spodziewałem. W wyniku jednej z takich rozmów Pan Maciej przekonywał mnie, że osoba taka jak ja, bez wykształcenia i bez znajomości podstaw nie ma szans zostać programistą. I jako, że 
Pan Maciej był dle mnie swoistym autorytetem i ekspertem uwierzyłem w jego słowa podkręcane zresztą przez mój brak wiary w siebie. I ponownie uznałem, że programowanie, pomimo że sprawia mi niesamowitą frajdę - że nie 
powinienm się nim zajmować. Że są od tego wykształceni specjaliści

## ROZDZAIŁ 3 - POWRÓT (i nowe nadzieje)
