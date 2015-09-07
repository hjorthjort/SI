# Pass 2

**I det här passet ska vi skapa ett spel som du kan spela i terminalen/kommandopromten, genom att bygga upp det bit för bit med hjälp av klasser och objekt. Använd `System.out.print` och `System.out.println` för att skriva ut spelets händelser.

Innan du börjar, skapa en klass Main med en main-metod för att du ska kunna testa dina nya klasser och kolla så att de fungerar som de ska.**

*Jag ber om ursäkt på förhand för all svengelska. Det är svårt att skriva om spel på svenska. Fråga om något känns otydligt*

## Uppgift 1

**Diskutera i grupp**

Hur tacklar du en uppgift som du inte vet hur du ska lösa och där det inte är tydligt var du ska börja?

Var tycker du om att börja leta information? Vad gör du om du inte hittar något bra svar på första googlingen?


## Uppgift 2

1. Gå till Javas API och titta på klassen java.util.Random. Bekanta dig med dess metoder.
2. Skriv nu en klass som modellerar en tärning. Du ska kunna:
    * ... skapa en ny tärning med godtyckligt antal sidor.
    * ... rulla tärningen och få veta vad den visade.

Kör din main-metod, skapa några olika tärningar och testa att rulla dem. Funkar allt som det ska?

## Uppgift 3

Skapa en klass `Monster`. Ett monster har en instansvariabel, `damage`, som sätts när monstret skapas till en siffra mellan 1 och 30.

Skapa också en klass `HealingPotion` som har en instansvariabel `healingPower` som fungerar på samma sätt, men har ett värde mellan 1 och 5.

Testa dina klasser i din main metod så att de funkar som de ska.

## Uppgift 4

Skapa en klass `Player`. En spelare ska ha ett namn och ett visst antal `healthPoints`, förslagsvis 100. 

Utöver detta ska en player ha två metoder, en för att slåss mot ett monster, och en för att helas av en healing potion. Den första metoden ska ta ett monster som argument, och den andra en healing potion.

När spelarens metod för att möta ett monster anropas så förlorar spelaren samma antal health points som monstret gör skada. Om spelaren dör ska ett lämpligt meddelande med spelarens namn skrivas ut, och programmet avslutsas.

Om spelarens metod för att helas anropas ska spelarens health points öka lika mycket som potionens healing power.

**Hur avslutar man ett program i Java? Googla!** 

Testa din Player-klass i main metoden.

## Uppgift 5

Lägg till att programmet ska vila i två sekunder mellan det att spelaren stöter på ett monster eller en healing potion, och att spelarens health points uppdateras. Lägg också in ett meddelande i båda metoderna som berättar vad som händer: att spelaren stött på ett monster eller en healing potion innan fördröjningen, och hur mycket skada eller extraliv som spelaren får efter.

## Uppgift 6

Skapa en klass `Room`. Denna ska innehålla en healing potion som är samma hela tiden. Klassen ska också ha en metod `enterPlayer` som tar emot en `Player` som argument.

När en spelare kommer in i rummet skapas ett nytt Monster, och en tärning rullas (förslagvis en 6-sidig tärning). Om tärningen visar en låg siffra (välj själv hur lågt som passar) ska spelaren slåss mot monstret. Rulla sedan tärningen igen. Om den visar en hög siffra ska spelaren helas av healing potionen. 

Testa så att klassen fungerar som den ska.

## Uppgift 7

Nu är det dags att bli kreativ! Sätt ihop ett spel av dina klasser. 

Skapa en klass `Map` som innehåller en samling rum. Dessa kan ligga på led efter varandra, så att det bara finns en väg framåt, eller i ett rutnät, så att det går att gå upp, ner, fram och bak. 

**Vad är ett lämpligt sätt att hålla reda på rummen i kartan? Vilka typer av objekt i Java kan du använda?**

I första varianten räcker det att du kan gå runt, stöta på monster och healing potions, utan att det finns ett mål. Välj själv hur du vill navigera runt. Ett sätt är att du matar in en bokstav och trycker Enter. Titta på klassen Scanner för att se hur du kan mata in text till ett program.

Lek med de klasser du har skapat, anpassa dem och se om du kan sätta ihop ett roligt spel.
