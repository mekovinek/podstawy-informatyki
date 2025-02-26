#  sieci fizyczne:
Sieć fizyczna to fizyczne ułorzenie kabli, urządzeń, i połączeń.Przykłady:
### Topologia magistrali (Bus)
jest to topologia w której wszystkie urządzenia w sieci są 
podłączone do jednego, wspólnego przewodu 
komunikacyjnego (tzw. magistrali). Dane przesyłane są w 
obu kierunkach, a każde urządzenie monitoruje przesył i 
odbiera dane przeznaczone dla siebie.
- Wady:
    - awaraia głównej magistrali powodóje awarię całego systemu.
    - im większa ilość urządzeń tym większe przeciąrzenie magistrali.
- Zalety:
    - łatwa i tania, w montarzu i obsłódze.
    - łatwa rozbudowa, poprzez pddanie nowego urzadzenia.
- Stosowana:
    - w starszych sieciach LAN o ograniczonej ilości urządzeń.
    - w celach edukacyjnych i testowych
### Topologia pierścienia(Ring)
jest to topologia w której urządzenia są połączone w zamkniętą 
pętlę. Dane przesyłane są w jednym kierunku (lub w obu w 
przypadku pierścieni dwukierunkowych), a każde 
urządzenie działa jako wzmacniacz sygnału.
- Wady:
    - awaria jednego urządzenia powoduje przerwanie działania całej sieci.
    - trudna naprawa i diagnostyka.
- Zalety:
    - brak kolizji danych przez uporządkowany ruch.
    - stabilna wydajność przy durzej liczbie urządzeń.
- Stosowana:
    - w sieciach korporacyjnych.
    - w starszych systemach telekomunikacyjnych.
### Topologia gwiazdy (Star)
jest to topologia w której wszystkie urządzenia w sieci są połączone z jednym  
centralnym punktem, którym najczęściej jest switch lub 
router. Każde urządzenie komunikuje się z innymi za 
pośrednictwem tego punktu.
- Wady:  
    - awaria centralnego węzła powodóje awarię całej sieci.
    - wysokie koszty wdrorzenie za względu na durzą ilośc okablowania.  
- Zalety:  
    - łatwe diagnozowanie problemów.
    - awaria jednego urządzenia nie wpływa na całą sieć.
    - łatwa rozbudowa, dodanie nowego urządzenia wymaga podłączenia go do centralnego węzła.  
- Stosowana:  
    - w nowoczesnych sieciach LAN w biurach i szkołach.
    - sieci domowe z ruterem jako centralą.
# sieci logiczne:
Sieci logiczne opisóją sposób wymiany danych między urządzeniami, nie zalerznie od fizycznej struktury.przykłady:
### punkt-punkt (point-to-point)
W tej topologii dane przesyłane są tylko między dwoma określonymi urządzeniami.
- Wady:
    - Brak skalowalności (każde nowe połączenie wymaga dodatkowego przewodu lub kanału).
    - Awaria jednego połączenia całkowicie przerywa komunikację.
- Zalety:
    - Brak kolizji danych (tylko dwa urządzenia komunikują się bezpośrednio).
    - Bardzo prosta implementacja.
    - Wysoka przepustowość
- Stosowana:
    - w połączeniach między dwoma routerami lub serwerami.
    - w sieciach VPN
    - w łączeniach urządzeń peryferyjnych(np. drukarka)
### rozgłaszania (broadcast)
W tej topologii host wysyła dane do wszystkich urządzeń podłączonych do danego centrum, a odbiorca je filtruje. Ten kto pierwszy wysyła dane zostaje pierwszy obsłurzony
- Wady:
    - Duża liczba kolizji
    - Niska wydajność w większych sieciach
    - Brak kontroli nad tym, kto odbiera dane.
- Zalety:
    - Prosta implementacja
    - Każde urządzenie w sieci może odbierać dane bez potrzeby trasowania.
    - Szybka komunikacja w małych sieciach.
- Stosowana:
    - w sieciach Ethernet
    - Sieci LAN (z hubem)
### przekazywania tokenu (token passing)
W tej topologii dane rozprowadzane są kolejno do urządzeń przez sieć. Urządzenie, które posiada token może korzystać z medium. Kiedy dane urządzenie nie potrzebuje dostępu do medium, to przekazuje ono token kolejnemu. 
- Wady:
    - Wolniejsze przesyłanie danych w porównaniu do nowoczesnych metod
    - Jeśli token zostanie utracony, sieć może wymagać restartu.
    - Skomplikowana implementacja i utrzymanie.
- Zalety:
    - Brak kolizji danych
    - Lepsza wydajność w dużych sieciach
    - Lepsza kontrola nad przepustowością sieci