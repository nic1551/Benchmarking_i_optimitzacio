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

Test sense index ni cache:

![nada](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/test_nada.png).


◦ Afegeix els índexs de la part 1
Index hotels:

![indexH](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/index_h.png).

Index Clients:

![indexc](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/index_C.png).

Index Reserves:

![indexc](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/res.png).

Benchmark amb index:

![indexo](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/no_Cache.png).

◦ Activa la CACHE (també fes que les consultes passin per aquesta CACHE)

Activa cache:

![1](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/setting_cache.png).

![2](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/doblecheck.png).


Realitza una comparativa mostrant els resultats obtinguts dels tres benchmarks. En el tercer cas indica quin ha estat el valor de CacheHitRatio.

Amb cache i index(s):

![todo](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/cahce.png).

Cache hits:

![hit](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/qhits.png).

Cache Inserts

![insert](https://github.com/nic1551/Benchmarking_i_optimitzacio/blob/master/Extrabench/qinserts.png).


Qcache_hits / (Qcache_hits + Qcache_inserts)

Simplefiquem: 

579 / (579 + 756848)

Encara mes: 

579 / 757427


