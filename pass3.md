# Pass 3

## Veckans begrepp: vad betyder de?

* Javadoc
* Identifierare 
* Modifierare (private/public/static/abstract/etc.)
* Klass
* Metod vs funktion
* Variabel
* Syntax vs Semantik
* Rekursion
* Modularisering
* Wrapper
* Scope
* Arv
* Literal
* Inkapsling

Arbeta utan dator först. Diskutera runt bordet vad ni tror och varför. Håller ni med varandra? 

När ni kommit överens, testa i datorn. Blev det som ni trodde? Om inte, vad kan det bero på?

### Uppgift 1

**Diskutera**

Ni har följande variabler:

        int a1 = 10;
        int a2 = 10;
        Integer a3 = new Integer(10);
        Integer a4 = new Integer(10);

        double b1 = 10.0;
        double b2 = 30*(1/10.0 + 2/10.0) + 1;
        Double b3 = new Double(10.0);

        String s1 = "Hello";
        String s2 = "Hello";
        String s3 = new String("Hello");

Vad blir resultatet av följande jämförelser, `true` eller `false`?

        a1 == a2;
        a1 == a3;
        a3 == a3;
        a3 == a4;
        a1 == b1;
        b1 == b2;
        b1 == b3;
        s1 == s2;
        s2 == s3;

### Uppgift 2

Utgå från samma variabler som förra uppgiften.

Vad blir resultatet av följande jämförelser? `true`, `false` eller orsakar de fel?

Kan ni använda Javas API för att ta reda på svaret?

        a1.equals(a2);
        a3.equals(a3);
        a3.equals(a4);
        b3.equals(b2);
        b3.equals(a3);
        d3.doubleValue == d1;
        s1.equals(s2);
        s2.equals(s3);

Bonusfråga: Vad blir resultatet?
        
        a3.equals(10);

### Uppgift 3

Ni har filen FunBar.java som ser ut som följer.

        package foo;

        public class FunBar {
            private int apa, bepa;
            protected int cepa = 3;
            String name;

            private FunBar(String name) {
                this.name = name;
            }

            public static FunBar constructor(String name) {
                return new FunBar(name);
            }

            public int sum() {
                return apa + bepa + cepa;
            }

            private class SmallFunBar extends FunBar {
                
                public SmallFunBar(String name) {
                    super(name);
                }

           }
        }

I samma mapp finns filen FooTester.java
        
        package foo;

        public class FooTester {
            public static void main(String[] args) {
                //a)
                FunBar bar1 = new FunBar("Bar1");
                bar1.cepa = 5;
                System.out.println(bar1.sum());
                
                //b)
                FunBar bar2 = FunBar.constructor("Bar2");
                bar2.cepa = 5;
                System.out.println(bar2.sum());

                //c)
                bar1.name = bar2.name;

                //d)
                FunBar.SmallFunBar small = new FunBar.SmallFunBar("small");
                small.cepa = 5;
                System.out.println(small.sum());
            }
        }

Vilka kodblock av a, b, c, och d kommer fungera att köra? Hur skulle ni kunna modifiera de som inte fungerar så att de blir körbara?

### Uppgift 4

Sant eller falskt? Motivera ditt svar. 

Hur skulle du förklara svaret för någon som precis börjat lära sig programmering?

a)  Uttrycket nedan kompilerar ok. (Antag att o inte deklarerats tidigare)

        Object o = new Integer(5);

b)  Uttrycket nedan evalueras till sant

            new Integer(11) == new Integer(11)

c)  En statisk medlemsmetod kan referera icke statiska variabler i samma klass men endast efter att en instans av klassen skapats.

d)  När ett objekt skickas som argumet till en metod så kan metoden ändra objektet.

### Begrepp för kommande veckor

* Interface
* Abstrakt klass
* Delegering
* Rekursion
* Exception

## Om ni får tid över

Har ni frågor ni vill ta upp och ha hjälp med?
