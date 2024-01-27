Assignment: Testiranje
Kurs: Software Quality Introduction
Modul: Testiranje u službi kvaliteta


Testiranje metodom crne kutije (black box)


1. Testiranje operacije sabiranja:

Unos: 1 + 2 + 3 + 4
Očekivani rezultat:  10.0 – test je proša
Unos: +1 + 2 + 3 + 4
Očekivani rezultat:  10.0 – test je proša
Unos: 1 ++ 2
Očekivani rezultat: 3.0 – test nije prošao – dobijeni rezultat je: ERROR


2. Testiranje operacije oduzimanja:

Unos: 10 - 2 - 3 - 1 
Očekivani rezultat: 4.0 – test je prošao
Unos: -10 - 2 - 3 - 1 
Očekivani rezultat: -16.0 – test je prošao
Unos: 2 - - 3
Očekivani rezultat: 5.0 – test nije prošao – dobijeni rezultat je: ERROR


3. Testiranje operacije množenja:

Unos: 10 * 2
Očekivani rezultat: 20.0 – test je prošao
Unos: 10 * 2 * 3 * 1 
Očekivani rezultat: 60.0 – test je prošao
Unos: 10 ** 2
Očekivani rezultat: ERROR – test je prošao


4. Testiranje operacije deljenja:

Unos: 10 / 2
Očekivani rezultat: 5.0 – test je prošao
Unos: 20 /5/ 2
Očekivani rezultat: 2.0 – test je prošao
Unos: 10 // 2
Očekivani rezultat: ERROR – test je prošao


5. Testiranje uzastopnih različitih operacija:

Unos: 2 + 3 * 4 - 5 / 2 * 2
Očekivani rezultat: 9.0 – test je prošao


6. Testiranje operacija sa negativnim brojevima:

Unos:   -2 * 3 + 5
Očekivani rezultat: -1.0 – test je prošao
Unos:   -2 -5
Očekivani rezultat: -7.0 – test je prošao
Unos:   2*-3
Očekivani rezultat: -6.0 – test nije prošao – dobijeni rezultat je: ERROR
Unos:   2+-3
Očekivani rezultat: -1.0 – test nije prošao – dobijeni rezultat je: ERROR
Unos:   -4/2
Očekivani rezultat: -2.0 – test je prošao
Unos:   -4/-2
Očekivani rezultat: 2.0 – test nije prošao – dobijeni rezultat je: ERROR
Unos:   4/-2
Očekivani rezultat: -2.0 – test nije prošao – dobijeni rezultat je: ERROR


7. Testiranje složenijih izraza sa decimalnim brojevima, razlomcima, zagradama, …

Unos:   2 * (3 + 4) – 6 / (2 + 1)
Očekivani rezultat: 12.0  – test nije prošao – dobijeni rezultat je: ERROR
Unos:   1.5 + 2 * 3 / 4
Očekivani rezultat: 3.0 – test je prošao
Unos:  2 + 3* 4 - 5 / 2 
Očekivani rezultat: 11.5 – test je prošao
Unos:  2 * (3 + 4) / 2 
Očekivani rezultat: 7.0 – test nije prošao – dobijeni rezultat je: ERROR
Unos:  −1.5+2.5*3/−4.0−(−1.0/2)
Očekivani rezultat: −2.875 – test nije prošao – dobijeni rezultat je: ERROR
Unos: -4.10/2
Očekivani rezultat: -2.05 – test je prošao
Unos: 1 / 3
Očekivani rezultat: 0.33333334 – test je prošao
Unos: 0.12345 * 10
Očekivani rezultat: 1.2345 – test je prošao
Unos: 8 / 2.5
Očekivani rezultat: 3.2– test je prošao
Unos: 0.5 * 2/3
Očekivani rezultat: 0.33333334 – test je prošao
Unos: 2.333 + 1.2 - 0.333
Očekivani rezultat: 3.2 – test je prošao


8. Testiranje unosa sa nulom:

Unos: 5 * 0 
Očekivani rezultat: 0.0 – test je prošao
Unos: 5 + 0 
Očekivani rezultat: 5.0 – test je prošao
Unos: 5 - 0 
Očekivani rezultat: 5.0 – test je prošao
Unos: 5/0 
Očekivani rezultat: Infinity – test je prošao
Unos: 5 / 0.0000
Očekivani rezultat: Infinity – test je prošao
Unos: 5.000 / 0.0000
Očekivani rezultat: Infinity – test je prošao
Unos: 0/5
Očekivani rezultat: 0.0 – test je prošao
Unos: 0/0 
Očekivani rezultat: NaN – test je prošao
Unos: 5 * 0 / 2
Očekivani rezultat: 0.0 – test je prošao
Unos: 5 * 2/ 0
Očekivani rezultat: Infinity – test je prošao


9. Testiranje velih brojeva:

Unos:  1000000000 + 500000000
Očekivani rezultat: 1.5E9 – test je prošao
Unos:  1000000000000/1.1
Očekivani rezultat: 9.090909E11 – test je prošao
Unos:  1.0E38/2
Očekivani rezultat: 5.0E37 – test je prošao
Unos:  1.0E20*100   
Očekivani rezultat: 1.0E22 – test je prošao


10. Testiranje neispravnog unosa:

Unos: 2+d+3
Očekivani rezultat:  ERROR – test je proša
Unos:  2*3+a
Očekivani rezultat:  ERROR – test je prošao
Unos:  5 -
Očekivani rezultat:  5.0 – test je prošao
Unos:  5 +
Očekivani rezultat:  5.0 – test je prošao
Unos:   2 +       3+       2
Očekivani rezultat: 7.0 – test je prošao
Unos:   2 *      3*      2
Očekivani rezultat: 12.0 – test je prošao




11. Testiranje operacija sa beskonačnim vrednostima:

Unos:   2 + Infinity
Očekivani rezultat: Infinity – test je prošao
Unos:   2 - Infinity
Očekivani rezultat: -Infinity – test je prošao
Unos:   2 * Infinity
Očekivani rezultat: Infinity – test je prošao
Unos:   2 / Infinity
Očekivani rezultat: 0.0 – test je prošao
Unos:   2.10 / Infinity
Očekivani rezultat: 0.0 – test je prošao
Unos:   2.10/2/ Infinity
Očekivani rezultat: 0.0 – test je prošao
Unos:   Infinity * Infinity
Očekivani rezultat: Infinity – test je prošao
Unos:   Infinity +Infinity
Očekivani rezultat: Infinity – test je prošao
Unos:   Infinity /0
Očekivani rezultat: Infinity – test je prošao
Unos:   Infinity - Infinity
Očekivani rezultat: NaN – test je prošao
Unos:   Infinity / Infinity
Očekivani rezultat: NaN – test je prošao
Unos:   0 * Infinity
Očekivani rezultat: NaN – test je prošao


12. Testiranje zatvaranja programa:

Unos: exit
Očekivani rezultat: izlaz iz programa – test je prošao





Zaključak testiranja metodom crne kutije (black box):


Testiranje metodom crne kutije otkriva nekoliko ključnih problema u implementaciji kalkulatora:


•Nedostatak podrške za zagrade (testovi iz 7. grupe):
Kalkulator nepravilno obrađuje izraze sa zagradama, što rezultira pojavu greške i nemogućnošću obrade složenih izraza.

•Problemi sa uzastopnim operatorima (testovi iz 1., 2. i 6. grupe):
Korišćenje uzastopnih operatora generiše grešku.

•Predlozi za poboljšanja:
Implementirati podršku za zagrade kako bi se omogućila ispravna obrada složenih izraza.
Razmotriti rešenje problema sa uzastopnim operatorima kako bi se osigurala tačnost rezultata.


Jedinično testiranje


public void testAddition()
//assertEquals(3.0f, parseFloat(Calculator.Run("1++2")));
assertEquals(ERROR, Calculator.Run("1++2"));
Greška nastaje prilikom pokušaja konverzije niza karaktera koji ne predstavlja validan broj u tip float. Konkretno, u ovom slučaju, pokušava se parsiranje niza "ERROR". Zaključak da program ne podržava upotrebu uzastopnih operatora (++).


public void testSubtraction()
//assertEquals(5.0f, parseFloat(Calculator.Run("2--3")));
assertEquals(ERROR, Calculator.Run("2--3"));
Greška nastaje prilikom pokušaja konverzije niza karaktera koji ne predstavlja validan broj u tip float. Konkretno, u ovom slučaju, pokušava se parsiranje niza "ERROR". Zaključak da program ne podržava upotrebu uzastopnih operatora (--).


public void testMultiplication()
//assertEquals(-20.0f, parseFloat(Calculator.Run("10*-2")));
assertEquals(ERROR, Calculator.Run("10*-2"));
Program ne podržava upotrebu uzastopnih operatora (*-).


public void testDivision()
//assertEquals(-5.0f, parseFloat(Calculator.Run("10/-2")));
assertEquals(ERROR, Calculator.Run("10/-2"));
Program ne podržava upotrebu uzastopnih operatora (/-).


public void testComplexExpressionsWithDecimals()
//assertEquals(12.0f, parseFloat(Calculator.Run("2*(3+4)-6/(2+1)")));
assertEquals(ERROR, Calculator.Run("2*(3+4)-6/(2+1)"));
Program ne podržava upotrebu zagrada ().


Zaključak:
	
Testovi pokazuju da kalkulator ispravno obavlja osnovne matematičke operacije i pravilno rukuje različitim tipovima ulaznih vrednosti. Međutim, postoji prostor za unapređenje, posebno u vezi sa podrškom za složene izraze i uzastopne operatore.

Prilikom testiranja različitih aritmetičkih operacija unutar testova za sabiranje, oduzimanje, množenje, deljenje i kompleksnih izraza s decimalnim brojevima, primećene su greške u programu. Greške proizilaze iz nepodržavanja uzastopnih operatora (npr. "++", "--", "*-", "/-"), kao i neadekvatne obrade zagrada u složenim izrazima.

Da bi se program unapredio, potrebno je implementirati logiku koja će pravilno tretirati uzastopne operatore i zagrade. Ovo uključuje definisanje jasnih pravila za postupanje s takvim slučajevima, poput ignorisanja uzastopnih operatora, zamene uzastopnih operatora jednim i pravilne obrade zagrada u složenim izrazima.

Ova poboljšanja će omogućiti da program adekvatno i precizno obrađuje različite matematičke izraze, čime će se eliminisati trenutne greške i poboljšati ukupna funkcionalnost kalkulatora.

