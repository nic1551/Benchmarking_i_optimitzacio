# Part 1. Escriu les sentències SQL per tal d’obtenir els que se’ns demana. A més a més si creus que la sentència es pot millorar amb la incorporació d’un índex i/o modificació de l’esquema (sense alterar-ne el comportament),etc... Afegeix la sentència DDL i l’output de EXPLAIN mostrant la millora (EXPLAIN sense índex i EXPLAIN amb índex). Si creus que la consulta no es pot millorar mitjançant índexs justifica el perquè. ( 2 punts )

1.	Obtenir el nom i l’adreça dels hotels de 4 estrelles.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/1.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/1.png)

2.	Obtenir el nom dels clients (Nom i cognom) que el seu cognom comenci per vocal (sense tenir en compte els accents).

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/2.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/2.png)

3.	Quina és la reserva_id que té més nits. Indica també la quantitat de nits.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/3.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/3.png)

4.	Quantes reserves va rebre l’hotel ‘Catalonia Ramblas’ de Barcelona durant tot  l’any 2015 (una reserva pertany al 2015 si alguna nit d’aquesta reserva era del 2015).

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/4.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/4.png)

5.	Obtenir el nom i cognoms dels clients que varen néixer el mes de Març.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/5.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/5.png)

6.	Quantitat d’hotels de 4 estrelles de la població de Barcelona.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/6.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/6.png)

7.	De l’any 2015 volem obtenir els seu histograma de reserves. És a dir volem saber el número de reserves de cadascun dels mesos. Una reserva pertany a un mes si la alguna nit d’aquella reserva cau a dins de l’any 2015.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/7.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/7.png)

8.	El nom dels hotels que tenen com a mínim una habitació lliure durant les dates ‘2015-05-01’ i ‘2015-05-17’.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/8.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/8.png)

9.	Obtenir la quantitat de reserves que s’inicien en cadascun dels dies de la setmana. Tenint en compte només l’any 2016.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/9.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/9.png)

10.	Durant 2014 qui va realitzar més reserves? Els homes o les dones? Mostra el sexe i el número de reserves.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/10.png)


Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/10.png)

11.	Quina és la mitjana de dies de reserva per l’hotel «HTOP Royal Star» de Blanes durant l’any 2016? (Una reserva pertany el 2016 si alguna nit cau en aquest any).

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/11.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/11.png)

12.	El nom, categoria, adreça i número d’habitacions de l’hotel amb més habitacions de la BD.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/12.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/12.png)

13.	Rànquing de 5 països amb més reserves durant l’any 2016. Per cada país mostrar el nom del país i el número de reserves.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/13.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/13.png)

14.	Codi client, Nom, Cognom, del client que ha realitzat més reserves de tota la BD.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/14.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/14.png)

15.	Codi client, Nom, Cognom, del client que ha realitzat més reserves durant el mes d’agost de l’any 2016. Les reserves a comptabilitzar són totes aquelles que en algun dia del seu període cau en el mes d’agost.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/15.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/15.png)

16.	Quin és el país que en tenim menys clients?

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/16.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/16.png)

17.	Quina és la mitjana de nits dels clients provinents d’‘HOLANDA’ per l’any 2016?

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/17.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/17.png)

18.	Digues el nom i cognoms dels clients que el seu cognom sigui ‘Bahi’.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/18.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/18.png)

19.	Quins clients (nom, cognoms) segueixen el patró de que el seu cognom comenci per la lletra ‘p’  i seguida d’una vocal.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/19.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/19.png)

20.	Quin és l’hotel de 4 estrelles amb més reserves durant tot el 2015 ( una reserva pertany el 2015 si alguna de les nits hi pertany).

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/20.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/20.png)

21.	Quin és l’hotel amb més reserves (tota la BD).

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/21.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/21.png)

22.	Quin és el país amb més reserves? (tots els anys) O sigui, quin és el país d’on han vingut més turistes.

Sense Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_sin_index/22.png)

Amb Index:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Capturas_con_index/22.png)


# Explicació de Indexs

CLIENTS: Aqui he agafat els 3 camps que feien servir mes en la taul: Camp del nom, camp de cognom i camp de data de naixement.
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Indexes/c1.png)

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Indexes/c2.png)

HOTELS: Aqui només he agafat el poblacio_id per ser més ràpid aleshores de buscar els poblacions diferents.
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Indexes/h1.png)
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Indexes/h2.png)

HABITACIONS:No fa falta perque un hotel no té moltes habitacions. Si tenia més de 300 habitacions podem començar a pensar sobre indexes

RESERVES: Aqui he agafat els camps hab_id, data_inici, data_fi i client_id, perquè son les mes buscades.
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Indexes/r1.png)
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Indexes/r2.png)

PAISOS: Com que el Base de Datos té poc països no fa falta crear un index.

POBLACIONS: Passa el mateix que països, com que hi ha pocs de moment no fa falta. Si ampliarem i posem poblacions de tot el món si necesitarem un index.


# Part 2 – Query Cache (5 punts)
Escull 5 sentències SQL de la Part 1 (intenta que els temps d’execució siguin significatius)
•	Quins temps d'execució t'han sortit per cada consulta?

El 9 = 0.00.000.102

El 13 = 0.00.000.079

El 17 = 0.00.000.090

El 21 = 0.00.000.088

El 7 = 0.00.00.108

•	Activa la Query Cache (ON)

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/1.png)

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/2.png)

◦	Reexecuta les consultes anteriors 2 vegades seguides. Ha millorat el temps d'execució?


el 9.1 :

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/9.1.png)

el 9.2 : 

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/9.2.png)

el 13.1 :

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/13.1.png)

el 13.2 : 

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/13.2.png)

el 17.1 :

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/17.1.png)

el 17.2 : 

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/17.2.png)

el 21.1 : 

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/21.1.png)

el 21.2 :

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/21.2.png)

el 7.1: 

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/7.1.png)

el 7.2 : 

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/7.2.png)

◦	Quina modificació hem de fer perquè la consulta no passi per Cache? (reescriu una consulta amb els canvis)

La comanda es SELECT SQL_NO_CACHE.

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/no_cache.png)


Aqui: (https://dev.mysql.com/doc/refman/5.5/en/query-cache-in-select.html)

•Activa la Query Cache (ON DEMAND)

La comanda es SELECT SQL_CACHE

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/sql_cache.png)

Podem fer referència al enllaç anterior de dev.mysql.com

◦	Posa un exemple d'execució sota demanda.

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/sql_cache.png)

◦	Quina modificació hem de fer perquè la consulta passi per Cache?(reescriu la consulta amb els canvis)


![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/sql_cache.png)


•	Un cop acabats els punts anteriors mostra quin ha estat el teu CacheHitRatio? Com has obtingut els valors de cache_hits i cache_misses?



•	Demostra quines sentències DML (INSERT, UPDATE, DELETE) provoquen que es buidi la cache de les taules implicades amb aquestes sentències.

Guia: (https://stackoverflow.com/questions/5231678/clear-mysql-query-cache-without-restarting-server)

FLUSH:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/FLUSH_QUERY_CACHE.png)

RESET:
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/CacheQuery/reset_query_cache.png)
# Part 3 – Benchmarking (2 punts)
Mitjançant la eina Sysbench prepara un joc de proves mitjançant les sentències SQL anteriors o d’altres que creguis que puguin anar bé per realitzar les proves.

Documenta la instal·lació de l'eina, la creació dels scripts de prova i l’execució de les proves.
Instalació:
Primer descarguem els REMIS.
![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Benchmarking/Install1.png).

Despres descarguem la segona paquet que conté els EPELREMOS.

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Benchmarking/Install2.png).

Finalment amb el YUM INSTALL WGET:.

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Benchmarking/sysbenche.png).

###	Test 1
Treu tots els índexs de la Part 1 i desactiva la CACHE i realitza el benchmark.

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Benchmarking/remove_index.png).

![alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Benchmarking/deactivate_cache_query.png).

ª[alt index](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Benchmarking/test1_1.png).

###	Test 2
◦	Afegeix els índexs de  la part 1
###	Test 3
◦	Activa la CACHE (també fes que les consultes passin per aquesta CACHE)
###	Realitza una comparativa mostrant els resultats obtinguts dels tres benchmarks. 	En el tercer cas indica quin ha estat el valor de CacheHitRatio.






