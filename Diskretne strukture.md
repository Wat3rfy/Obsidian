
**Graf** je množica vozlišč in množica povezav med njimi

$$G = (V, E)$$

$V$ je **množica vozlišč**.
$E$ je **množica povezav**, ki vsebuje dvoelementne podmnožice $V$.

$$E = \{\{ u,v\} \,;\;  u,v \in  V \,,\;u \neq v\}$$

**Enostaven graf** je graf brez zank, vzporednih, in usmerjenih povezav. *Kjer so zanke povezazve same s seboj.*

$$uv := \{ u,v\} := u \sim v$$

**Stopnja** vozlišča je število povezav, ki vsebujejo vozlišče.

$$\deg_{G}u = \left|\{ e \,;\; u \in e\} \right|$$

**Izolirano vozlišče** je nepovezano vozlišče oz. $\deg_{G}u = 0$.

Povezavi sta **incidenčni** če nimata skupnega vozlišča.

$$e,f \in E, e \neq f, e \cap f = \emptyset$$

**Matrika sosednosti** je kvadratna matrika, ki opisuje katera vozlišča grafa so med seboj povezana. 
Za graf $G = (V,E)\,;\; V = \{ v_{1},... v_{n}\}$
je velikosti $n \times n$, kjer je $A_{ij} = 1$, če obstaja povezava med vozliščema $v_{i}, v_{j}$ oz. 0 če ne obstaja.

Matrika je vedno simetrična, na diagonali ima same ničle (pri enostavnih), vspta vrednosti vrstic oz. stolpcev za vozlišče $v_{i}$ je enaka stopnji $v_{i}$.

**Incidenčna matrika** je matrika ki povezuje vozlišča in povezave grafa. 

Za graf $G = (V,E)$ z $n$ vozlišči in $m$ povezazavami je velikosti $n \times m$ kjer je $B_{ij} = 1$, če je vozlišče $v_{i}$ povezano s povezavo $e_{j}$ in $B_{ij} = 0$, če ni.

Vsak stolpec ima natanko 2 enici. Vsota vrednosti vrstic je enaka stopnji vozlišča $v_{i}$.ž

Za predstavitev grafa lahko uporabimo tudi **seznam sosedov**. Vsako vozlišče ima svojo množico sosednjih vozlišč s katerimi je povezano.

$$N_{G}(v) = \{ u \in  V \,;\; u \sim v\}$$
$$ (N_{G}(v_{1}),...,N_{G}(v_{n}))$$
***
>**Izrek o rokovanju** pravi da je vsota stopenj vseh vozlišč enaka dvakratniku števila povezav. 
>*Vsaka povezava pogojuje 2 vozlišči stopnje 1*
>
>$$\sum_{v \in V}^{}\deg(v) = 2 |E|$$
>>[!|dokaz]- Dokaz:
>>Vsaka povezava prispeva 1 k stopnji dveh vozlišč.
>>Če seštevamo stopnje vseh vozlišč, vsako povezavo štejemo dvakrat - enkrat za vsako vozlišče, ki jo povezuje.
>>To pomeni da je vsota stopenj enaka dvakratniku števila povzav.
***
> V vsakem grafu je sodo število vozlišč lihe stopnje.
> >[!|dokaz]- Dokaz:
> > Uporabimo izrek o rokovanju, kjer vsoto stopenj vozlišč razdelimo na vsoto stopenj sodih in vsoto stopenj lihih vozlišč.
> > Vsota lihih števil je soda če je število lihih števil sodo.
> > Vsota sodih števil je soda.
> > $2|E|$ je sodo in vsota sodih stopenj je soda torej mora biti število lihih stopenj sodo.
***
$G$ je **$k$-regularen**, če je stopnja vsakega vozlišča $k$.
$G$ je **regularen**, če je $k$-regularen.

$H$ je **podgraf** če je $V_{H} \subset V_{G}$ in $E_{H} \subset E_{G}$.

$H$ je **vpet podgraf** če velja da je $V_{H} = V_{G}$

$H$ je **induciran podgraf** če velja da ob izbiri podmnožice volišč, ta ohranjajo vse medsebojne povezave originalnega grafa.

$$V_{H}\subset  V_{G}$$
$$E_{H} = \{ uv \,;\;u,v \in V_{H} \land uv \in  E_{G}\}$$

**Komplement grafa** G je $\overline{G}$ in velja

$$\overline{G} = (V, \overline{E})$$
$$\overline{E} = \{ uv \,;\; uv \notin E\}$$

**Polni graf** $[K_{n}]$ je graf v katerem so vsa vozlišča povezana med sabo.

$$V = [n] \;\;\;\;\;E = \{ i\sim j \,;\; i \neq j \land i,j \in V\}$$ 
$$|E(K_{n})| = \frac{n(n-1)}{2} $$

**Pot** $[P_{n}]$ je graf v katerem so povezana samo zaporedna vozlišča.

$$V = [n] \;\;\;\;\;E = \{ i \sim (i+1) \,;\; i \in \{ 0,...,n\}\}$$

$$|E(P_{n})| =n-1 $$

**Cikel** $[C_{n}]$ je graf kjer so povezana samo zaporedna vozlišča ter prvo in zadnje.

$$V = [n] \;\;\;\;\;E = \{ i \sim j \,;\; i-j = 1 \lor j-i = 1\}$$

**Hiperkocka** $[Q_{n}]$ je graf, ki predstavlja $n$-dimenzionalno kocko.

$$V = \{ (\varepsilon_{1} ... \varepsilon_{n}) \,;\; \varepsilon_{i} \in \{ 0,1\}\} $$ 
$$E = \{ (\varepsilon_{1} ... \varepsilon_{n}) \sim (\delta_{1}...\delta_{n}) \,;\; \text{razlikujeta v samo enem mestu}\}$$

Vozlišča so binarni listi, dolžine $n$, povezave pa so tvorjene med tistimi vozlišči, ki se razlikujejo v natanko eni števki. Ob večanju $n$ se nova števka postavi na konev lista.

**Polni dvodelni graf** $[K_{m,n}]$ je graf, kjer je množica vozlišč razdeljena na 2 disjunktni podmnožici, kjer so vozlišča povezana le iz ene množice v drugo, povezave med vozlišči v isti podmnožici pa ne obstajata.

$$V = [m] \times \{ 0\} \cup [n] \times \{ 1\}$$
$$E = \{ (i,j) \sim (i',j') \;;\; j \neq j' \}$$

**Posplošeni petersonov graf** $[P_{n,k}]$ je graf tvorjen iz $C_{n}$ in $G_{n}$ z množico vozlišč, ki se porazdeli v $C_{n}$ in $G_{n}$, tako da so v $C$ in $G$ indeksi od $1$ do $n$, kjer je $C_{n}$ cikel indeksov, vsako $i$ vozl. iz $C$ je povezano z vsakim $i$ vozl. iz $G$, povezave v $G_{n}$ pa so tvorjene med vozlišči, katera razlika je enaka $k$ po modulu.

$$V(P_{n,k}) = \{ u_{1},...,u_{n},v_{1},...,v_{n}\}$$
$$A = \{ u_{i} \sim u_{i+1} \land u_{1} \sim u_{n}\}$$
$$B = \{ u_{i} \sim v_{i}\}$$
$$C = \{ v_{i} \sim v_{\,i+k \;(\text{mod } n)}\}$$
$$E(P_{n,k}) = A \cup B \cup C$$

Petersonov graf je $P_{5,2.}$

**Komponenta grafa** je tak podgraf za katerega velja da za vse  pare vozlišč $G$ velja, da če sta v množici podgrafa potem obstaja pot med njima.

$$u,v \in V \Rightarrow \exists P(u,v)$$

**Povezan graf** je graf z eno komponento.
Če graf ni povezan ga sestavlja več komponent.

