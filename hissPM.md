# THE HISS

Kevin Tornéus 2024-12-13

## Inledning


Vi fick i uppgift att med hjälp av digitala hjälpmedel analysera hur en typisk hiss fungerar för att sedan försöka återskapa en egen.

## Bakgrund

Jag och min grupp hade ett gemensamt mål i början att göra våran version av en hiss i spelmotorn Unity eftersom att vi påstod att med hjälp av denna spelmotor så skulle arbetet underlättas, speciellt med att lägga till grafik. 

Vi behövde först dock skapa en hiss i valfritt programmeringsspråk först innan vi skulle gå i unity för att få en uppfattning på hur vi skulle kunna skriva koden senare i spelmotorn, och få en generell uppfattning på hur en hiss kod är upplagd.

Efter lite fram och tillbaka så bestämde vi oss för att börja skriva våran kod i språken C# eftersom att det var det språket som Unity använde sig av och att vi enklare kunde klistra in våran kod direkt i Unity. Till slut så hade vi en färdig hiss i C# som kunde läsa in förtryckta "hissknappar" och åka samt stanna vid dem.

För detta moment så använde vi och delade ett github repo och/eller passade runt en dator så alla kunde hjälpas åt att koda scriptet, eftersom c# liknar bland annat java som vi hade kodat i förut samt att jag själv har använt unity förut var det enkelt att komma in i. Denna version av hissen fungerade genom att två arrayer vid namnet "upQueue" och "downQueue" hade olika värden inuti sig som representerade de olika knapptrycken utanför hissen. När programmet sedan startades så avlästes sedan dessa och programmet skrev i terminalen vart och när den stannade på våningarna.

Slutligen när det var klart så övergick vi till att använda programmet Unity för att implementera grafik i en 2D scen. Vi började med att skapa en simpel kvadrat sprite och försöka klistra in våran förra C# kod in ett script i unity som var en component till våran sprite.

Att skriva om denna kod var lite svårt, delvis eftersom att vi alla förväntade oss att det fortfarande skulle fungerera om vi bara klistrade in våran kod i unity. Det visade sig att unity använder sin egen version av en massa grejer och det blev upp till oss alla att försöka rätta till det för att passa in i unitys c#.

När vi slutligen lyckades korrekt skriva om koden för att vara kompatibel med unity så lades ui knappar till och funktioner kopplades sedan till dessa, dessa knappar aktiverade sedan den färdiga hisskoden. Med knappar tillagda var vår hiss kvar och jag använde den resterande tiden till att lägga till larmknapp och byta ut hissspriten mot en hiss som Oscar ritade.

Bild på nuvarande projektet i Unity editor:

![NTI Gymnasiet Umeå Logo](https://cdn.discordapp.com/attachments/1241135025555247214/1318908241966665768/image.png?ex=67640885&is=6762b705&hm=f8c618df1b7df7bbf82fbe605587e9837d9c83cdffd16463a1e6ff3c479591d0&)

## Positiva erfarenheter

Våran slutprodukt blev jag i alla fall nöjd med och till en viss nivå vägen dit också. Om vi bortser ifrån hur trögt framstegen togs i början så hade vi alla i våran grupp ändå rätt så lika insats i detta projekt. Såklart så hade jag lite förkunskap när det kom till just c# och unity men det kändes aldrig som om jag tog över helt riktigt. Alla hjälpes åt och gjorde sitt bästa med detta projekt vilket är något som jag respekterar. 

## Negativa erfarenheter

Här beskriver du det som du anser har gått mindre bra med ditt projekt och analyserar hur du kan undvika detta i framtida projekt.

Som sagt så hade jag ansett att början av detta projekt var lite osäkert eftersom att vi inte visste riktigt hur vi skulle börja koda en hiss och i vilket språk. Vi förlorade motivation på grund av detta och i kombination av att vi då på den tiden brukade variera vem som kodade mellan varje lektion hade alla en lite annorlunda syn på hur hissen borde fungera. detta ledde till att koden skrevs om flera gånger innan vi kom någon vart.

Detta hade kunnats undvikas i framtiden genom att tydlig planera innan och se till att alla i ens grupp är med på samma sak och att vi alla har en tydlig plan sedan innan om hur allting borde fungera.

## Sammanfattning

Här redovisar du dina slutsatser, erfarenheter och lärdomar. Reflektera över din produkt och dess/dina utvecklingsmöjligheter.
Vad kan vidareutvecklas och finns det utrymme att bygga vidare på projektet.

Sammanfattningsvis så var jag nöjd med de flesta anspekter av detta projekt, jag lärde mig även mycket ifrån detta projekt till exempel att övergå från c# till att klistra in det i unity kräver ompassning av kod och syntax.

Våran slutprodukt, medan jag som sagt blev nöjd med den så är den inte perfekt, till exempel så var ett problem att programmet kraschade när knappen längst ned trycktes. Ingen lyckades komma fram till varför detta uppstod och till slut kom jag på den temporära lösningen att automatiskt ändra hissens intärna nuvarande våning med ett medan den visuellt var kvar på våning noll. Detta gjorde det desvärre så att hissen sedan fort hoppar emellan våningarna vilket inte ser verkligt ut alls. Utöver det så fungerar hissen som den ska.




