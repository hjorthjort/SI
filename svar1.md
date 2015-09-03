# Svar till första passet

## Uppgift 1
Sätt int looparna i ett program och testa!

Skapa en javafil via terminalen:

    $ touch TestLoops.java

Klistra in följande
    public class TestLoops {
      public static void main(String[] args) {
        [klistra in loopen här]
      }
    }

Kör detta i terminalen

    $ javac TestLoops.java
    $ java TestLoops

så skrivs resultatet ut.

Ni kan förstås också köra programmet från Eclipse, IntelliJ eller någon annan [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment) om ni vill det.

## Uppgift 2

Du skapar en (publik) klass med syntaxen

    public class ClassName {
      [grejerna inuti klassen]
    }

För att till exempel skapa en metod som tar emot två heltal och returnerar ett heltal

    public int aMathyMethod(int firstNumber, int secondNumber) {
      [uträkningar och grejer]
      return [det som ska skickas tillbaka, i detta fallet ett heltal]
    }

## Uppgift 3

Till exempel:

    public class Fibonacci {
      public static void main(String[] args) {
        int lastOne = 1;  
        int lastTwo = 1;
        for (int i = 0; i<10; i++) {
          System.out.print(lastOne + " ");
          int newNum = lastOne + lastTwo;
          lastOne = lastTwo;
          lastTwo = newNum;
        }
      }
    }

## Uppgift 4

Det är detta man använder "String[] args" i main-metoden till!

När du i terminalen skriver

    $ java MittProgram Tre olika argument "Ett långt argument"

Så skapas [arrayen](http://docs.oracle.com/javase/tutorial/java/nutsandbolts/arrays.html) args, som innehåller `["Tre", "olika", "argument", "Ett långt argument"]`

För att skriva ut det du skickar in skriver du helt enkelt

    public static void main(String[] args) {
      System.out.println(args[0]);
    }

Det är därför du alltid måste ha med `String[] args` i din main-metod.


## Uppgift 5

Till exempel:

    public class Fibonacci {
      public static void main(String[] args) {
        int argument = Integer.parseInt(args[0]);
        fib(argument);
      }

      private static void fib(int number) {
        int lastOne = 1;  
        int lastTwo = 1;
        for (int i = 0; i < number; i++) { //Notera skillnaden från ovan
          System.out.print(lastOne + " ");
          int newNum = lastOne + lastTwo;
          lastOne = lastTwo;
          lastTwo = newNum;
        }
      }
    }

Detta är inte det elegantaste sättet att göra det på. Man kan också göra såhär:

      public class Fibonacci {
        public static void main(String[] args) {
          int argument = Integer.parseInt(args[0]);
          for (int i = 1; i <= argument; i++)
              System.out.println(fib(i) + " ");
        }

        private static int fib(int number) {
          int lastOne = 1;  
          int lastTwo = 1;
          for (int i = 1; i < number; i++) { //Notera skillnaden från ovan
            int newNum = lastOne + lastTwo;
            lastOne = lastTwo;
            lastTwo = newNum;
          }
          return lastOne;
        }
      }

När programmet ser ut såhär kan man också använda fib-metoden till andra saker, vilket ofta är en stor fördel.

Däremot är programmet inte särskilt effektivt. Varför? Hur skulle man kunna göra det effektivare? Tips: Kan man spara resultatet från tidigare uträkningar på något smart sätt?

Bonus: Vilket är det största Fibonacci-talet du kan räkna ut med metoden utan att något går fel? Hur stort är det ungefär?

## Uppgift 6

Till exempel:

    public class Square {
      public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
          for (int j = 0; j < 5; j++)
            System.out.print("+ ");
          System.out.println();
        }
      }
    }

## Uppgift 7

Till exempel:

    public class Triangle {
      public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
          for (int k = 0; k < i; k++)
            System.out.print("  ");
          for (int j = 0; j < 5 - i; j++)
            System.out.print('0');
          System.out.println();
        }
      }
    }

## Uppgift 8

Tankenöt: Här får du inget facit!

Tips på ett sätt att lösa uppgiften:
* Skriv metod som kollar om ett tal är ett primtal.
* Skriv en metod som använder metoden ovan för att kolla om två tal är primtalstvillingar.
* Skriv en metod som letar primtalstvillingar upp till ett visst tal, och skriver ut resultaten.
* Starta metoden ovan från main-metoden.

Återigen, detta är inte det allra effektivaste sättet, eftersom samma sak kanske räknas ut flera gånger. Hur skulle man kunna göra det effektivare? Här räcker det att formulera steg på samma sätt som ovan för hur man skulle kunna gå tillväga.
