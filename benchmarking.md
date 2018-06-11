Part 3 – Benchmarking (2 punts)

### Nota. Els següents captures estan fet en un Ubuntu Server.

Mitjançant la eina Sysbench prepara un joc de proves mitjançant les sentències SQL anteriors o d’altres que creguis que puguin anar bé per realitzar les proves.

Instal·lació:

![Instal·lació](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/sysbench.png).

Crearem un base de datos de prova:

![Prova](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/create_db.png).

Omplim de dates creades per el BBDD:

![test1](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/gg.png).

Si fem un COUNT mostra que ha tardat 0,16s.

![count](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/test1.png).

Ara fem una altre prova de escritura:

![test2](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/updgrade1.png).

I els resultats:

![res](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/test2.png).

Finalment netejem la taula de prova:

![cleanup](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/cleanup.png).

Documenta la instal·lació de l'eina, la creació dels scripts de prova i l’execució de les proves. 

Treu tots els índexs de la Part 1 i desactiva la CACHE i realitza el benchmark.

◦ Afegeix els índexs de la part 1


◦ Activa la CACHE (també fes que les consultes passin per aquesta CACHE)
Realitza una comparativa mostrant els resultats obtinguts dels tres benchmarks. En el tercer cas indica quin ha estat el valor de CacheHitRatio.
