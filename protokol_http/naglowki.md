# Nagłówki odpowiedzi:
- **"acces-contol-allow-origin: https://www.sci.edu.pl/"** - zezwala na dostęp do zasobów serwera określonej domenie, w tym przypadku https://www.sci.edu.pl/
- **"content-type: application/json"** - określa typ danych odpowiedzi w tym przypadku json
- **"Access-Control-Allow-Credentials: true"** - Ten nagłówek jest częścią mechanizmu CORS i informuje przeglądarkę, czy zapytania pochodzące z innej domeny mogą zawierać dane uwierzytelniające w tym przypadku true, takie jak:
    * cookies
    * hasła
    * loginy

# Nagłówki rządania
- **Priority** - jest używany do określenia priorytetu zapytania HTTP w kontekście sieci. Może pomóc serwerowi w określeniu, które zapytania są ważniejsze do przetworzenia lub które zasoby powinny być załadowane w pierwszej kolejności.
- **Origin** - wskazuje pochodzenie żądania, czyli protokół, domenę i port strony, z której pochodzi zapytanie. Jest to kluczowe w kontekście CORS, ponieważ serwer używa tego nagłówka do określenia, czy pozwolić na zapytanie z zewnętrznej domeny.
- **Accept** - nformuje serwer, jakie typy danych klient jest w stanie zaakceptować. Jest to kluczowy nagłówek w kontekście API, który pozwala serwerowi wysłać odpowiedź w odpowiednim formacie, takim jak JSON, XML itp.

