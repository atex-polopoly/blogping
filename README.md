================================================================================

INNEHÅLL:

    1. Arbetsprov - Beskrivning
    2. Uppgift - Blog Ping
    3. Installera Blog Ping projektet
    4. Testning
 

================================================================================
1 Arbetsprov - Beskrivning
================================================================================

Målet med provet är att visa hur du normalt tar dig an en javabaserad
programmeringsuppgift. Kriterier vi kommer använda vid bedömning
innehåller:
 - Clean design
 - Reuse (3:rd part products)
 - Maintainability
 - Testability
 - Java knowledge
 - Coding style

Du avgör själv hur "djupt" du måste utföra arbetsprovet för att
ovanstående skall framgå.

================================================================================
2. Uppgift - Blog Ping
================================================================================

Skriv en klient samt server som implementerar REST varianten av det så
kallade blogping protokollet i Java.

Vi vill således se:
 - En klient (kommandorad eller webapp) som anropar en blogping-server
med korrekta argument (och som hanterar eventuella felfall) med hjälp av
REST-apiet
 - En blogping-server som kan ta emot en REST blogping
 - En blogping-server som listar pingade bloggar i en changes.xml som är
tillgänglig via HTTP

Blogping REST-api samt formatet för changes.xml finns dokumenterat på:

 http://www.weblogs.com/api.html (par: Setting up a REST Client)


================================================================================
3. Installera Blog Ping projektet
================================================================================

Var god följ stegen nedan:

1. Ladda ner och installera Maven. Maven kan du ladda ner från http://maven.apache.org/download.cgi
2. Kör kommandot: "mvn install" i roten av distributionsmappen.  
3. Kör kommandot: "mvn jetty:run" "blogping". Detta kommer att starta en Jetty Server på port 8080.
4. Gå mot adressen: http://localhost:8080/hello. Servern bör svara med en text som lyder: "Hello Atex!".
5. Nu är din miljö och Blog Ping projekt korrekt installerat.

================================================================================
4. Testning
================================================================================

Vi uppmana dig att skriva unit/integration tester.

Följ namngivningskonvention:
* unit-test: src/test/java/**/*Test.java
* integration-test: src/test/java/**/*IT.java

Det finns några enkla test att utgå ifrån. Du kör integration-tester med "mvn verify", notera då att
mvn drar igång jetty åt dig. Om din implementation är korrekt borde com.atex.blogping.BlogpingIT går igenom.

 
 
