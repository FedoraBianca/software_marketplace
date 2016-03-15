# software_marketplace

Portal web cu site de tip "marketplace" (piata) pentru software (in cele ce
 urmeaza un obiect software va fi numit generic "program"). El va contine
 cel putin urmatoarele:
 - o baza de date pe un server MySQL, PostgreSQL, MSSQL sau Oracle, cu
 programele cerute spre realizare, utilizatorii inregistrati, etc.;
   pentru fiecare program se vor retine cel putin: numele, cumparatorul,
 realizatorii, specificatiile, tipul de licenta (BSD, GPL, CDDL, etc.),
 pretul licitat;
   utilizatorii pot fi de mai multe categorii: administrator, cumparator,
 analist (realizeaza specificarea cerintelor), proiectant (realizeaza
 design-ul software), programator (realizeaza codul), tester (testeaza
 programul si raporteaza bug-uri, efectueaza recenzii); pentru fiecare
 utilizator se va retine cel putin: numele contului si parola, numele real,
 CNP, adresa, e-mail, pagina web (doar in cazul analistilor, proiectantilor,
 programatorilor, testerilor), programe cumparate/realizate pana acum,
 suma totala cheltuita/castigata pana in prezent, rating (cu exceptia
 administratorului);
 - o interfata web care ofera cel putin urmatoarele:
  * motor de cautare pentru programe, cu categorii si search (cu filtrare pe
   categorii/subcategorii); sa se poata cauta dupa mai multe criterii:
   limbaj de programare, cuvinte-cheie, pret/dificultate, rating, etc.;
  * creare cont (cu furnizarea unor date proprii)/logare in cont;
  * pentru alte facilitati - a se vedea mai jos;
 - dupa logare utilizatorul isi poate accesa contul si in functie de
   categorie poate efectua in plus anumite operatii:
  * un administrator poate face toate operatiile de administrare;
  * un cumparator poate solicita programe folosind niste formulare (care vor
     cere suficiente informatii pentru a permite actualizarea tuturor
     aspectelor legate de program in baza de date);
    programele sunt supuse licitatiei (bid) in care se va decide cine va
     realiza specificarea cerintelor, proiectul software, dezvoltarea
     (codarea), testarea, in functie de preferintele cumparatorului;
  * un analist creaza documentul cu specificarea exacta a cerintelor, pe
     baza descrierilor facute de cumparator; documentul descrie CE trebuie
     sa faca programul;
    un proiectant creaza proiectul software, pe baza specificatiilor
     analistului; el descrie CUM este construit si functioneaza programul;
    un programator creaza codul propriuzis pe baza specificatiilor
     proiectantului;
    testerul testeaza si/sau analizeaza programul gata dezvoltat furnizand
     rapoarte cu bug-uri programatorului si/sau recenzia programului
     cumparatorului;
    fiecare completeaza un formular si atasaza fisierele necesare;
  * un analist/proiectatant/programator/tester poate sa liciteze pentru un
     anumit program, cerand un anumit pret;
    din moment ce cumparatorul a acceptat pretul cerut, programul intra
     in faza de specificare/proiectare/dezvoltare/testare/analiza si nu
     poate fi modificat la capitolul cerinte, iar cumparatorul va efectua
     plata pentru program site-ului, urmand ca banii sa ajunga la
     realizatori cand programul este gata si operational;
    cumparatorul nu are voie sa liciteze sub conturi de analist/proiectatant
     /programator/tester la propriile programe; de asemenea cei care vor
     avea clone vor fi BAN-ati (inclusiv BAN la IP daca este nevoie);
    in functie de anumiti factori se calculeaza un rating pentru fiecare
     program care poate sa mareasca sau sa scada ratingul cumparatorului si
     realizatorilor; alternativa: la finalul realizarii unui program
     cumparatorul are posibilitatea sa evalueze realizatorii implicati iar
     realizatorii pe cumparator, iar aceste evaluari vor afecta rating-ul
     fiecaruia;
  * orice utilizator inregistrat (indiferent de categorie) poate efectua
     urmatoarele:
    ** actualizare informatii personale din cont;
    ** eliminarea propriului cont; aceast lucru este posibil doar daca nu
        are proiecte in derulare;
    ** browse printre licitatii/programe/utilizatori;
    ** search (folosind motorul de cautare - a se vedea mai sus) pentru
        licitatii/programe/analisti/proiectanti/programatori/testeri, cu
        filtrare dupa categorii/subcategorii, specificatii, etc.; sa se
        poata cauta dupa mai multe criterii;
    ** view activitatea curenta (ce proiecte are in derulare, liciteaza);
    ** posibilitate de comanda prin e-mail;
    ** e-mail pentru asistenta;
    ** forum de discutii;
    ** talk (intr-o fereastra text) cu unul/mai multi dintre utilizatorii
        curent logati (ei vor fi afisati organizat pentru a fi selectati
        usor).
Eventual, portalul va permite si vanzarea prin licitatie a unor programe
 complet realizate.
