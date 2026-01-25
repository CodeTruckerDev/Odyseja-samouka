# Odyseja-samouka

Z góry uprzedzam, to będzie raczej długa opowieść, bez skrótów typu TL;DR

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

I w tym właśnie momencie uznałem, że napiszę taką aplikację sam.

Zrobiłem więc ranking języków programowania, wybrałem Pythona i rozpocząłem naukę z tutoriali dostępnych na platformie YouTube. Jednak po pewnym niedługim czasie zauważyłem, że tutoriale te 
oczywiście pokazują użycie komend ale nie uczą praktyki. Opracowałem więc własny sposób nauki. Zarejestrowałem się na forum Pythonowym i korzystając z pytań, które zgłaszali studenci
zgłębiałem wiedzę dotyczącą tego języka. Googlałem tematy, przeprowadzałem testy na swoim komputerze, po czym dawałem odpowiedź. Nigdy nie dawałem gotowca, dawałem podpowiedzi wraz z 
odnośnikami do źródeł. Tak więc pytający byli zadowoleni, i ja także.

Wracając do problemu z synem, zaprojektowałem aplikację oraz sposób jej działania, po czym napisałem kod - oczywiście nie od razu zadziałało jak chciałem - jednak koniec konców powstała aplikacja
dzięki której stałem się wrogiem publicznym mojego syna. Aplikacja była stosunkowo prosta - na starcie komputera do pliku tekstowego była dopisywana aktualna data, po czym trzy ostatnie wpisy
były porównywane. Jeśli zapisy były różne, młodzieniec mógł korzystać z komputera przez godzinę, po upływie której komputer samoczynnie się wyłączał. Jeżeli natomiast zapisy dat były takie same
komputer wyłączał się po jednej minucie. W ten sposób syn mógł grać dwa razy po jednej godzinie, a pozostała minuta została stworzona aby całkowicie nie zablokować komputera - żeby w 
razie potrzeby móc aplikację zatrzymać. Oto przed Wami - Guardian 1.0.
