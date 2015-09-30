Pass 4
======

Begrepp: nya
-------

Diskutera fem minuter i grupp: vilka nya begrepp har dykt upp den här veckan? Vilka kan ni förklara? Finns det några som ni inte vet vad de betyder.

Använd gärna föreläsningsslides!

Begrepp: repetition
-------------------

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

Chalmersstudenten
-----------------

Dela in er i grupper. Helst minst 3 grupper om möjligt, men se till att var aåtminstone 2 i varje grupp.

### Uppgift 1

Skriv en klass som representerar en Chalmersstudent. 

1. Vilka klass- och instansvariabler behövs? Lägg dessa högst upp i klassen. Lägg till setters och getters till de som kan komma att ändras.
1. Tänk ut vilka beteenden studenten ska kunna ha (minst 5) och skriv metoder för dessa. Här kan ni låtsas att det finns andra klasser, som University, Teacher, Exam, och annat ni kan komma på. Gör det gärna Chalmersspecifikt, med saker som man bara kan göra här!
1. Skapa flera olika konstruktorer för olika ändamål. Vad måste finnas varje gång? Vad kan man göra till default? 
1. När ni är nöjda, skicka klassen vidare till en annan grupp.

### Uppgift 2

1. Sätt er in i klassen ni fått. Förstår ni vad den gör? Är några namn på variabler eller metoder otydliga? Ändra i så fall dessa.
1. Skapa en testklass och skriv i dess main-metod flera tester (minst 3) som testar att klassen ni fått gör vad man kan förvänta sig. Vill ni skriva ut testresultat eller använda `assert` för att kolla att allt funkar?
1. Skicka vidare klassen till en ny grupp.

### Uppgift 3

1. Skriv javadoc för klassen för Chalmersstudenten. Använd till exempel taggarna `@param`, `@return` och `@throws`. Googla vad dessa gör.
1. Skriv en beskrivande javadoc-kommentar för hela klassen. Vad är dess syfte och vad modellerar den?
1. Skicka klassen vidare till nästa grupp.

*Viktigt att tänka på när ni skriver kommentarer: Förklara inte hur koden jobbar, säg bara vad den gör. Den som läser kommentaren ska inte behöva veta hur metoderna ser ut inuti, utan det ska räcka att läsa kommentarer för att förstå vad metoden gör.*

Utmaningar
----------

### Uppgift 4

1. Specificera ett interface för er klass att implementera. Detta interface ska vilken student på vilken högskola som helst kunna implementera. Vilka metoder plockar ni ut? Ni kan skriva nya metoder i er klass, eller byta namn på dem.
1. Skapa en klass WorkingStudent som ärver från er tidigare klass, men som dessutom ska ha metoder och variabler för att representera följande
    * Nuvarande lön
    * Nuvarande arbetsplats
    * Arbetslivserfarenhet mätt i år
1. Skicka vidare

### Uppgift 5

Skapa till klass, för en KTH-student, på samma sätt som ni skapade en för Chalmersstudenten.

Innan ni börjar, fundera över följande:
* Kan ni på något sätt minimera den kod som behövs?
* Hur kan ni göra för att ha en WorkingStudent på KTH också?
* Är strukturen ni fått, med klasser och interface, den bästa? Eller finns det smartare sätt att använda arv, interface och abstrakta klasser för att få de klasser och beteenden ni vill ha?

Bonus
-----

### Uppgift 6

Åh nej! Java-kompilatorn har gått sönder! Den kan inte längre göra loopar eller hantera några andra literaler än `1`!

Hur ska du kunna utföra beräkningar?

Skriv en metod som adderar två tal som den får in. Du får inte addera eller subtrahera med mer än 1 i en beräkning, och du kan inte använda loopar. Hur gör du?

### Uppgift 7

Skriv en metod som beräknar det n:te Fibonacci-talet med hjälp av rekursion. Testkör den med 100, 1000, 10 000, 100 000 och 2 000 000 000.

Vad händer med uträkningshastigheten? 

Hur skulle du kunna får metoden att jobba snabbare? Kan du lägga in något i klassen eller objektet som kan öka ditt performance?
