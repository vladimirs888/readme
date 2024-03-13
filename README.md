UKUPAN BROJ LINIJA KLASA Start.java i Calculator.java je 19 + 130=149
Fajl: Start.java
Broj linije koda: 19
Ciklomatska složenost: 2
Kognitivna složenost: 1

Start.java -6
	-Varijabla Expression je deklarisana za čuvanje unosa, ali bi bilo bolje da se naziva po konvenciji expression
Start.java -11
	-Petlja while se koristi za kontinuirano čitanje korisničkog unosa dok god je program aktivan
	-Svaka iteracija petlje stvara novu instancu Scanner, što može biti nepotrebno
	-Nema provere ispravnosti unosa. Ako korisnik unese neispravan izraz, program bi mogao naići na grešku pri evaluaciji izraza
Start.java -19
	-U kodu se koristi klasa Calculator, tačnije metoda Run kako bi se izvršilo računanje izraza

Calculator.java
Broj linija koda: 130
Ciklomatska složenost: 5
Kognitivna složenost: 3

Calculator.java - 4-26
	-Kod je organizovan u jednu javnu klasu Calculator i jednu unutrašnju statičku klasu Operations
	-Postoji metoda Run() za pokretanje kalkulatora i nekoliko pomoćnih metoda (evaluateExpression() i Calculate())
	-Postoji statička promenljiva finalResult koja je korišćena za čuvanje rezultata izračunavanja, nije jasno zašto je ova promenljiva statička, a nema komentara koji objašnjavaju njenu namenu.
Calculator.java - 18
	-Unutrašnja statička klasa Operations definiše simbole za osnovne aritmetičke operacije (+, -, *, /). Njena metoda ToString() kombinuje ove simbole u string,
	naziv metode ne prati konvenciju imenovanja prvo slovo u nazivu je veliko, takodje naziv metode bi trebao da bude precizniji
Calculator.java - 24
	-Metoda Run() poziva evaluateExpression() za izračunavanje izraza. Naziv ove metode bi mogao biti precizniji
Calculator.java - 28
	-Ova metoda obrađuje uneti izraz
	-Nedostaje komentar koji bi objasnio funkcionalnost metode, kao i ulazne/izlazne parametre
	-Nedostaje provera unosa, kao što je provera da li je izraz null pre korišćenja charAt()

Calculator.java - 74
	-Ova metoda vrši izračunavanje konačnog rezultata na osnovu liste brojeva i operacija
	-Metoda `Calculate` je suviše kompleksna i sadrži dupliran kod
	-Nedostaje komentar koji bi objasnio funkcionalnost metode, kao i ulazne/izlazne parametre
	-Nedostatak provere unosa i mogući problemi sa tačnošću računanja pri radu sa float vrednostima



	
