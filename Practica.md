Part 1. Escriu les sentències SQL per tal d’obtenir els que se’ns demana. A més a més si creus que la sentència es pot millorar amb la incorporació d’un índex i/o modificació de l’esquema (sense alterar-ne el comportament),etc... Afegeix la sentència DDL i l’output de EXPLAIN mostrant la millora (EXPLAIN sense índex i EXPLAIN amb índex). Si creus que la consulta no es pot millorar mitjançant índexs justifica el perquè. ( 2 punts )

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
i1
i2

HOTELS: Aqui només he agafat el poblacio_id per ser més ràpid aleshores de buscar els poblacions diferents.
i1
i2

HABITACIONS:No fa falta perque un hotel no té moltes habitacions. Si tenia més de 300 habitacions podem començar a pensar sobre indexes

RESERVES: Aqui he agafat els camps hab_id, data_inici, data_fi i client_id, perquè son les mes buscades.


PAISOS: Com que el Base de Datos té poc països no fa falta crear un index.

POBLACIONS: Passa el mateix que països, com que hi ha pocs de moment no fa falta. Si ampliarem i posem poblacions de tot el món si necesitarem un index.
