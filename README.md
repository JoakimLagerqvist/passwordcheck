# passwordcheck
schoolwork
Specifikation

- Skapa en class PasswordChecker
    - Attribut
        - password
        - weak_passwords
    - Metoder
        - is_password_length_ok
            - Ser så lösenordet är minst 8 characters långt
            - Returnera True om OK, annars False
        - is_password_weak
            - Titta så att lösenordet inte hittas i listan weak_passwords
            - Returnera True om OK, annars False
        - has_password_at_least_two_numbers
            - Titta så lösenordet har åtminstonde 2 siffror
                - Tips - använd pythons isnumeric() funktion
            - Returnera True om OK, annars False
        - has_password_at_least_two_capital_letters
            - Titta så lösenordet har åtminstonde 2 versaler
                - Tips - använd pythons isupper
            - Returnera True om OK, annars False
        - do_password_validation
            - Kalla på ovan metoder, om lösenordet inte har några fel, printa ut “Password OK”, annars printa ut ett meddelande för respektive kontroll så användaren kan se vad som är fel på lösenordet
            - Funktionen skall också returnera totala antalet fel som uppstått
- Skapa en TestClass som heter TestPasswordChecker (som ärver från TestCase) med tester i en separat fil där du testar de olika metoderna, både om man skickar in ett “bra” lösenord men också om man skickar in ett bristfälligt lösenord, testa respektive metod i din PasswordChecker class.
    - Testet skall köras automatiskt mha main-processen när man kör test-filen
    - Skapa både unit-tester för respektive metod, men också ett integrationtest som testar do_password_validation
    

Tips:

- Tänk på att du i classen kan sätta ett password i __init__ kan sättas = None vilket gör att du kan instantiera classen i setUp() och sen sätta lösenordet på classen manuellt i respektive test med instance.password = ‘asdasdadad’ t.ex.
