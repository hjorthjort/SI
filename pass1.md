# Pass 1

## Uppgift 1
### Vad blir outputen när man kör följande loopar?

#### a)
     for(int i = 1; i <= 5; i++) {
         System.out.println(i*i);
     }

#### b)

     for(int i = 1; i <= 10; i++) {
         if(i%2 == 0) {
             System.out.println(i);
         }
      }

#### c)
     for(int i = 1; i <= 3; i++) {
         for(int j = 1; j <= 3; j++) {
             System.out.println(i*j);
         }
     }

#### d)
     for(int i = 1; i <= 3; i++) {
         for(int j = 1; j <= 3; j++) {
             if((i*j)%2 == 0) {
                 System.out.println(i*j);
             }
         }
     }

#### e)
     for(int i = 1; i <= 3; i++) {
         for(int j = 3; true; j += 10) {
             System.out.println(i*j);
             break;
         }
     }

#### f)
     for(int i = 3; i >= 1; i--) {
         for(int j = 5; j >= 1; j = j - 2) {
             System.out.println(i+j);
         }
     }

#### g)
    for(int i = 1; i <= 5; i++) {
         if(i%2 == 0) {
             for(int j = 1; j <= 3; j++) {
                 System.out.println(i*j);
             }
         }
     }


## Uppgift 2
Förklara för varandra:

1. Hur skapar man en klass?
2. Hur skapar man en metod?
1. Om du vill manipulera en sträng (klassen String), t.ex. skriva ut den baklänges – var skulle vara ett bra ställe att börja leta metoder som gör det?

## Uppgift 3
Fibonaccis talföljd är följande: 1 1 2 3 5 8 13 ...

Den brukar definieras såhär:

    fib(1) = 1
    fib(2) = 1
    fib(n) = fib(n-1) + fib(n-2) , n > 2

Skriv ett program som skriver ut de 10 första Fibonacci-talen. Använd for- och/eller while-loopar.

## Uppgift 4
Om du vill skicka med argument, till exempel tal eller strängar, till main-metoden, hur gör du då? Kan ni hitta svaret på Google?

Skriv ett program som bara upprepar vad du skriver.

Till exempel:

    $ javac Repeat.java
    $ java Repeat "Hej på dig!"
    $ Hej på dig!


## Uppgift 5
Skriv en metod som givet ett heltal `n` skriver ut de `n` första fibonacci-talen.

Exempel:

    $ javac Fib.java
    $ java Fib 10
    $ 1 1 2 3 5 8 13 21 34 55

Tips: kan ni göra om Uppgift 3 till en egen metod och använda den för att göra den här uppgiften?

## Uppgift 6
Skriv ett program som skriver ut följande rutnät

        + + + + +
        + + + + +
        + + + + +
        + + + + +

## Uppgift 7
Skriv ett program som skriver ut triangeln nedan:

    00000
      0000
        000
          00
            0

## Uppgift 8
Primtalstvillingar kallas två primtal som bara har ett annat tal mellan sig. Exempel på primtalstvillingar är `5, 7`, `11, 13`, `41, 43` osv.

Skriv ett program som använder loopar för att hitta de största primtalstvillingarna under ett visst tal. Såhär ska det fungera:

      $ javac Twins.java
      $ java Twins 70
      $ (59, 61)
