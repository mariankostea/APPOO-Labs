## Lab-4 Proiectarea sistemului. Tipuri de arhitecturi

#### Obiectivele
- Proiectarea sistemului. 
- Familiarizarea cu ahitectura pe nivele (Layered architecture)
- Structurarea logica in package-uri. Package by layer vs package by feature.
 
## Sarcina

- Pentru laboratorul 1, fiecare a ales o tema si a construit diagrama de clasa. Insa diagrama de clasa continea doar clasele model(asa numitele clase care contin date, nu contin logica). Acesta se considera data layer din aplicatia voastra. In orice aplicatie, datele sunt pastrate undeva la nivel fizic, nu doar in memorie. O sa consideram ca mai departe utilizam o baza de date, care corespunde relational cu diagrama voastra de clasa. Adica, contine aceleasi tabele ca si clasele voastre, si aceleasi relatie intre tabele.  Pentru acest lab, o sa ne familiarizam cu inca 2 layere, DAO (Data Acces Object) layer si Service layer. 

**DAO:** Este in general pentru logica de date. Contine metode de operatiune cu datele. Spre exemplu ar contine metode ca sa returneze datele conform careva criterii.

**Service:** Contine nemijlocit business logica. Spre exemplu careva logica asupra datelor extrase prin DAO layer.

Baza de date se alege de catre fiecare la dorință. Aceasta poate fi creata cu SQl scripturi , manual, nu e necesar de facut asta din Java. În java, trebuie de implementat aceste 2 layere, fiecare se gandeste, și adaugă câteva metode DAO și Service. În main, imi demonstrați comportamentul DAO și Service. (e.g. Scoateți careva date, le prelucrați cu metode din service, le faceți update înapoi în bază).

