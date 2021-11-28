
## Lab01:

* Step 01:
* mvn compile exec:java -Dexec.mainClass="com.marcobehler.ApplicationLauncher"
* http://localhost:8080

* Step02:
* mvn package
* java -jar target\myfancypdfinvoices-1.0-SNAPSHOT.jar
* http://localhost:8080

## Lab02:

* Step01:
* mvn package
* java -jar target\myfancypdfinvoices-1.0-SNAPSHOT.jar
* POST http://localhost:8080/invoices?user_id=freddieFox&amount=50
* Accept: application/json
* payload:
  {
  "id": "8e5e750b-d0ab-4003-b0ed-2adaf0f51c4f",
  "amount": 50,
  "user_id": "freddieFox",
  "pdf_url": "http://www.africau.edu/images/default/sample.pdf"
  }

* Step02:
* GET http://localhost:8080/invoices
* Accept: application/json

