
### Podmnožice v evklidskem prostoru



*Nekje se vse elementerne funkcije*


##### Zadosten in potreben pogoj

Pogoj je **zadosten**, če lahko posledica obstaja brez pogoja. Torej ob A vemo B, a ni nujno da A velja da velja tudi B. To da velja A nam da vedeti da velja B, a B velja neodvisno od A.

Pogoj je **potreben**, če velja da posledica ne obstaja če pogoj ne obstaja. Ob $\neg$B vemo da $\neg$ A, ob B pa ne vemo ali A velja ali ne, samo vemo da mora B veljati da velja A, torej lahko A tudi ne velja.

### Množice v merskih prostorih


Množica je **navzgor** omejena če velja, da obstaja število tako, da je večje od vsakega elementa v množici.

$$\exists \overline{a}\;\forall a : \overline{a}>a $$

Množica je **omejena** če je omejena navzgor in navzdol hkrati.

**Okolica** točke $a$ je vsak odprti interval $(a-\varepsilon, a +\varepsilon)$.

Točka je **notranja** če velja da obstaja njena okolica, ki vsebuje samo elemente iz množica. 
Točka je **robna** če velja, da za vsako njeno okolico velja da vsebuje vsaj en element iz množice in en element izven množice. 
Točka je **zunanja** če obstaja okolica, ki vsebuje samo elemente izven množice.

Množica je **odprta**, natanko tedaj ko za vsak $a$ obstaja taka okolica $a$, ki je popolnoma vsebovana v množici.
*Vse njene točke so notranje* 


Naj bo $X$ podmnožica $\mathbb{R}$. Množica $A \subset X$ je **odprta v $X$** če obstaja odprta množica $B \subset \mathbb{R}$ tako da velja $A = B \cap X$ ^ad8952

Množica je **zaprta** če je komplement odprte. 
*Vsebuje vse svoje robne točke.*

Množica je **kompaktna** če je zaprta in omejena hkrati. ^2de28b
Oziroma če lahko iz vsakega zaporedja točk vsaj 1 stekališče v množici.

Množica je **končna**, če ima končno število elementov.




Element $a$ je **stekališče množice** $A$ če velja da vsaka njena okolica vsebuje neskončno točk množice $A$.


$$n! := 1 \cdot 2 \cdot ... \cdot n$$
$$0! = 1$$
$$\binom{\,n\,}{\,k\,} := \frac{n!}{k!(n-k)!} $$
$$(a+b)^{n} = \sum_{0}^{n}\binom{\,n\,}{\,k\,}a^{k}b^{n-k}$$


Realno **zaporedje** je preslikava iz $\mathbb{N} \longrightarrow \mathbb{R}$. $(a_{n})_{n}$ kjer je $a_{n} = a(n)$. Lahko jih seštevamo, odštevamo, množimo in delimo.

Zapoerdje je **rekurzivno** s podanim prvim členom in formulo, s katero opisujemo naslednji element iz prejšnjega.

**Aritemtično zaporedje** je zaporedje s konstantno razliko med členi.

$$a_{n} = a_{n-1} + d = a_{1}+d(n-1)$$
$$S_{n} = \frac{n}{2} \cdot  (a_{1}+a_{n})$$

**Geometrično zaporedje** je zaporedje s konstantim koeficientom med členi.

$$a_{n} = a_{n-1} \cdot k = a_{1} \cdot k^{n-1}$$
$$S_{n} = \sum_{1}^{n} = a_{1} + a_{1}k + ... + a_{1}k^{n-1}$$
$$S_{n}k = k\sum_{1}^{n} = a_{1}k + a_{1}k^2 + ... + a_{1}k^{n}$$
$$...$$
$$S_{n} = a_{1}\frac{1-k^{n+1}}{1-k}$$
$$\sum_{1}^{\infty} = \frac{a_{1}}{k-1} ;\; |k |<1$$

Zaporedje je **omejeno navzgor**, če je množica $a_{n}$ omejena navzgor.

Množica ima **supremum** če za vsako manjšo zgornjo mejo obstaja element večji od nje.

$$\sup A \Leftrightarrow \forall \varepsilon > 0 \;\exists a \in A \ni: a > \sup A - \varepsilon$$

Če ni omejeno je **neomejeno**.

**Naraščajoče zaporedje**: $a_{n+1} > a_{n}$ ; nenaraščajoče $\geq$

Zaporedje je **monotono** če je nepadajoče ali nenaraščajoče oz. strogo monotono če je naraščajoče ali padajoče $\forall n$.

Točka $t$ je **limita zaporedja** če za vsako njeno okolico velja da vsebuje vse elemente od nekega indeksa naprej.

$$\lim_{n \to \infty}a_{n}$$


>Konvergentno zaporedje v $\mathbb{R}$ ima natanko eno limito.  
>*Elementi ne morejo skakati iz okolico v okolico ker drugače niso vsi elementi v okolici ene od limit*

>Vsako konvergentno zaporedje v $\mathbb{R}$ je omejeno.
>*Recimo da ni omejeno potem obstaja *

> Za konvergentni zaporedji velja da je vsota njunih limit enaka limiti vsote zaporedij. Enako za razliko, produkt in koeficient.
>*Lahko si izberemo tak $\varepsilon$ da je $|(a_n +b_n) - (A+B)| \leq \frac{\varepsilon}{2} + \frac{\varepsilon}{2} = e$*

>Če je zaporedje montono ima limito enako $\sup a_{n}$ če pada pa $\inf a_{n}$

> Če je zaporedje monotono in omejeno, je konvergentno


Bernoullijeva neenakost

$$\forall n \in \mathbb{N}, \;\forall \alpha \leq 1 : (1-\alpha)^{n} \geq 1 -\alpha n$$


Zaporedje $a_{n} := (1+ \frac{1}{n})^{n}$ je konvergentno.

**Podzaporedje** zaporedja $a_{n}$ je zaporedje $a_{n'}$, kjer je $n' : \mathbb{N} \rightarrow \mathbb{N}$ neka funkcija.

> Če je $L$ limita $a_{n}$ je $L$ limita vsakega podzaporedja.

Točka je **stekališče** zaporedja če v vsaki njeni okolici obstaja neskončno členov zaporedja *(oz. če je stekališče množice členov zaporedja, kot podmnožica metričnega prostora.)*

> Točka je stekališče zaporedja natanko tedaj ko je točka limita nekega njegovega podzaporedja
> *V levo smer imp. po definiciji limite, v desno smer imp. po dnf stekališča*

> Če obstaja limta zaporedja je to edino stekališče zaporedja.
> *Po prejšnjem izreku da je limita zaporedja limita vsakega podzaporedja, stekališče zaporedja pa je limita podzaporedja*

> Vsako omejeno zaporedje v realnih številih ima kakšno stekališče v realnih številih.

> Če ima zaporedje natanko eno stekališče je to limita zaporedja.

Pravimo da ima zaporedje **stekališče v $\infty$** če za vsak interval $(M, \infty)$ velja da vsebuje neskončno elementov.

Pravimo da ima zaporedje **limito v $\infty$** če vsak interval $(M, \infty)$ vsebuje neskončno elementov od nekega indeksa naprej.

**Limes superior** $\lim \sup$ je vrednost proti kateri gre supremum zaporedja.
**Limes inferior** $\lim \inf$ je vrednost proti kateri gre infimum zaporedja.
> Če je zaporedje navzgor oz. navzdol neomejeno sta ti vrednosti $\infty$ oz. $-\infty$.

> Lim sup in lim inf vedno obstajata.

> $\lim \sup$ oz. $\lim \inf$ je največje oz. najmanjše stekališče zaporedja $a_{n}$

**Zaporedjeje** **Cauchyjevo** če za vsako še tako majhno število, za vse pare členov velja da je njuna razlika manjša, za vse pare od nekega indeksa dalje. 



> Konvergentno zaporedje je natannko tedaj ko je Cauchyjevo


**Vrsta konvergira** če je konvergentno zaporedje delnih vsot. Taki limiti pravimo **vsota vrste**.

$$\lim_{n \to \infty}s_{n} = \sum_{1}^{\infty}a_{k}$$






**Geometrijska vrsta** je vrsta oblike

$$\sum_{1}^{\infty}k^j$$
$$S_{n} = \sum_{1}^{n} = 1 + k + ... + k^{n}$$
$$S_{n}k = k\sum_{1}^{n} = a_{1}k + a_{1}k^2 + ... + a_{1}k^{n+1}$$
$$...$$
$$S_{n} = \frac{1-k^{n+1}}{1-k}$$
$$\sum_{1}^{\infty} = \frac{1}{k-1} ;\; |k |<1$$

> Geomterijska vrsta je konvergentna če je $k \in (-1,1)$ konvergira pa k $\frac{1}{k-1}$.

**Hamonična vrsta** je vrsta oblike

$$\sum_{1}^{\infty} \frac{1}{j}$$

vemo da zaporedje $\frac{1}{n}$ konvergira k nič, a ta vrsta divergira.

> Vrsta je konvergentna natanko tedaj, ko je Cauchyjeva.
>$$\left| \sum_{n+1}^{m} a_{j}\right| < \varepsilon$$

>Če vrsta konvergira, zaporedje konvergira k 0.
>*$a_{n} = s_{n+1}-s_{n} \rightarrow s-s = 0$*







Vrsta je **absolutno konvergentna** če je 

$$\sum_{1}^{\infty}|a_{n}| < \infty$$

> Če je vrsta absolutno konvergentna je konvergentna.
> *Cauchyjev pogoj ... $|s_{m}-s_{n}| = |\sum_{n+1}^{m}a_{j}| \leq \sum_{n+1 }^{m}|a_{j}|<\varepsilon$*

**Primerjalni kriterij** je pravilo ki pravi da če imamo dve vrsti z nenegativnimi členi in ena konvergira, potem konvergira vsaka vrsta manjša od nje. Vrsta, ki omejuje manjše vrste se imenuje **majoranta**.

> Če neka vrsta divergira potem divergira vsak vrsta večja od nje.

**Kvocientni / d'Alembertov kriterij** je pravilo, ki pravi da če je limita kvocienta sosednjih členov manjša od 1 potem vrsta absolutno konvergira, če je večja od 1 divergira, če pa je 1 pa ne vemo.
Izhaja iz geometrijske vrste kjer vemo da če je kvocient manjši od 1 potem vrsta konvergira.

$$D_{n} = \left|\frac{a_{n+1}}{a_{n}} \right|$$

$$D \leq k < 1$$

**Korenski / Cauchyjev kriterij** je pravilo, ki pravi da če je limita n-tega korena n-tega člena manjša od 1 potem vrsta konvergira, če je večja od 1 divergira, če je 1 pa ne vemo.

$$C_{n} = \sqrt[n]{|a_{n}|}$$

Spet izhaja iz geomtrijske vrste kjer je geometrijska vrsta majoranta. 

$$\sqrt[n]{|a_{n}|} \leq k < 1 \Rightarrow |a_{n}| \leq k^{n} < 1$$

Vrsta je **alternirajoča** če za vse $n$ velja da je predznak prejšnjega člena drugačen trenutnemu.

**Leibnizov konvergenčni kriterij** trdi da če zaporedje konvergira k nič z desne potem konvergira vrsta $$\sum_{1 }^{\infty} (-1)^{j}a_{j}$$

> Ob tem velja da je $|s - s_{n}| \leq a_{n+1}$

Vrsta je **brezpogojno konvergentna**, če za vsako permutacijo indeksov konvergira.

Vrsta je **pogojno konvergentna** če je konvergentna, a ne brezpogojno.

**Funkcije** so predpis, ki slikajo iz ene množice v drugo. 

Funkcija mora biti definirana za celotno svoje defincijsko območje.

**Praslika množice $B$** pod funkcijo $f$, označena z$f^{-1}(B)$, je množica vseh elementov $x$ v domeni $f$ za katere velja  $f(x) \in  B$

$$f^{−1}(B)=\{x \in X ;\; f(x) \in B\}$$

**Praslika posameznega elementa**: Če imamo posamezen element $y$ in množico $B = \{ y \}$, potem je praslika $f^{-1}(\{ y \})$ množica vseh $x$, za katere velja $f(x) = y$. Če je $f$ injektivna, bo ta množica vsebovala največ en element, in če $f$ ima inverzno funkcijo, bo $f^{-1}(\{ y \}) = \{ f^{-1}(y) \}$.

**Zožitev funkcije** je funkcija ki slika iz podmnožice definicijskega območja.

**Kompozitum** je slikanje preko ene funckije nato pa slikanje pridobljene vrednosti čez še eno funkcijo.

Funkcija je **injektivna** če vsakemu elementu v zalogi vrednosti pripada en element v definicijskem območju.

$$f(x) = f(y) \Rightarrow x = y$$

Funkcija je **surjektivna** ko velja da imajo vse vrednosti iz zaloge vrednosti svojo prasliko.

$$Z_{f} = B$$

Funkcija je **bijektivna** natanko tedaj ko za vsak element v $B$ obstaja natanko en element v $A$, ki se preslika vanj.

Če je funkcija bijektivna lahko definiramo njen **inverz** kot funkcijo ki slika iz $B$ v $A$ : $f(x) \mapsto x$.
Velja da je $f^{-1} \circ f = \text{id}_{A}$ in $f \circ f^{-1} = \text{id}_{B}$

Funkcije lahko seštevamo, odštevamo, množimo, delimo med sabo.

Premiki oz. translacije

$$(\tau_{a}f)(x) :=f(x-a)$$
$$(\tau^{a}f)(x) :=f(x)+a$$
$$(\delta_{t}f)(x) :=f\left(\frac{x}{t}\right)$$
$$(\delta^{t}f)(x) :=t \cdot f(x)$$

Zrcaljenje

$$(\delta^{-1}f)(x) \text{ ali } (\delta_{-1}f)(x)$$

Funkcija ima **limito v točki $a$**, ko se $x$ približuje $x_{a}$, če velja, da za vsako okolico $a$, velja da obstaja okolica $x_{a}$ taka da če je $x$ v okolici $x_{a}$ a ne enak $x_{a}$ potem vemo da je $f(x)$ v okolici $a$;

$$\forall \varepsilon > 0 \; \exists \delta>0 \forall x \in D_{f} : 0<|x-x_{a}|<\delta \Rightarrow |f(x)-f(a)|<\varepsilon$$

Leva limita:

$$\forall \varepsilon \; \exists \delta \;\forall x \in D_{f} : 0<x_{a}-x <\delta \Rightarrow |f(x)-f(a)| < \varepsilon $$

$$\lim_{x \to a^{-}}f(x)$$

Desna limita

$$\forall \varepsilon \; \exists \delta \;\forall x \in D_{f} : 0<x- x_{a} <\delta \Rightarrow |f(x)-f(a)| < \varepsilon $$

$$\lim_{x \to a^{+}}f(x)$$


> Funkcija ima limito v točki tudi kadar je desna limita v točki $a$ enaka levi limiti $a$.

Če obstajata leva in desna limita a nista enaki potem ima funkcija tam **skok**.

Funkcija je **zvezna v točki $a$** če velja da za vsako okolico $a$ obstaja okolica $x_{a}$ tako da za vsak $x$ velja da če vemo da je v okolici $x_{a}$ vemo da je $f(x)$ v okolici $a$.

$$\forall \varepsilon > 0 \; \exists \delta>0 \forall x \in D_{f} : |x-x_{a}|<\delta \Rightarrow |f(x)-f(a)|<\varepsilon$$

Recimo da obstaja funkcija, ki je zvezna povsod razen v $a \in D_{f}$. Če v tej točki obstaja limita lahko definiramo funkcijo odsekovno tako da ob $x=a$ rečemo da je $f(a) = \lim_{x \to a}f(x)$, čemur pravimo **zvezna raširitev funkcije**.

Funkcija je **odsekoma zvezna** če velja da je zvezna povsod na $D_{f}$ razen na končno mnogih točkah v katerih ima skok.

> Če je limita $h$ in $g$ v točki $a$ enaka $L$ in velja da je $h \leq f \leq g$ potem je limita $f$ v točki $a$ enaka $L$.

> Funckija naj bo definirana povsod razen v $a$. Za vsako zaporedje $x_{n}$, ki konvergira k $a$ , $f(x_{n})$ konvergira k $L$, natanko tedaj ko je limita funkcije $f$ ko gre $x$ k $a$ enaka $L$.
>
>$$ L = \lim_{x \to a}f(x) \Leftrightarrow (\forall x_{n} : x_{n} \rightarrow a \Rightarrow f(x_{n}) \rightarrow L)$$

> Funkcija je zvezna v $a$ natanko tedaj, ko je v $a$ zvezna po zaporedjih.

>Vsaka vsota. razlika, produkt, kvocient zvzenih funkcij je spet zvezna funkcija.

> Vsi polinomi in racionalne funkcije so zvezne na scojih definicijskih območjih.
> *Iz prejšnje trditve kjer hkrati vemo da je identiteta in konstante zvezne funkcije.*

>Če sta $f$ in $g$ obe zvezni potem je $g \circ f$ zvezna funkcija.

Vsaka **elementarna funkcija** je zvezna na svojem definicijskem območju.

[[#^ad8952|Odprta množica v množici]]

> Naj bo $W \subset D \subset \mathbb{R}$. Velja da je $W$ odprta v $D$ natanko tedaj, ko velja da za vsak element v $W$ obstaja taka okolica da je presek okolice in množice $D$ prava podmnožica $W$.

>Velja tudi da, ko je $D$ odprta in $W \subset D$, je $W$ odprta v $D$ natanko tedaj ko je $W$ odprta v $\mathbb{R}$

>$f$ je zvezna natanko tedaj če za vsako odprto množico $V$ velja da je $f^{-1}(V)$ spet odprta množica v $D$. 


[[#^2de28b|Kompaktna množica]]

Tipičen predstavnik kompaktne množice je **zaprt interval**.

> Naj bo $D$ kompaktna in $f: D \rightarrow \mathbb{R}$ zvezna. Takrat velja da je $f$ omejena in doseže minimum in maksimum.

> Naj bo $f$ definirana na zaprtem intervalu $[a,b]$ zvezna in $f(a)f(b) < 0$. Tedaj velja da obstaja tako število $\xi$ na $(a,b)$ tako da velja $f(\xi ) = 0$

> Če je funkcija definirana na zaprtem intervalu zvezna, na njem doseže minimum, maksimum in vse vrednosti vmes.

Če za zvezno funkcijo velja, da izbran delta deluje za vse vrednosti $x$ ob izbranem $\varepsilon$ potem pravimo da je funkcija enakomerno zvezna.

$$\forall \varepsilon >0 \; \exists \delta > 0\;\forall x' \in D \;  \ni: \forall x \in D\; \;|x-x'|<\delta \Rightarrow |f(x)-f(x')|< \varepsilon$$

> Če je množica kompaktna velja da je funkcija zvezna natanko tedaj, ko je enakomerno zvezna.

Odvod funckije v točki $a$ je koeficient tangente na funkcijo. Pove kako se spreminja vrednost funkcije pri še tako majhnih razlikah v $x$.

$$f'(x) = \lim_{h \to 0}\frac{f(x+h) - f(x)}{h}$$

je odvod če ta limita obstaja. V tem primeru pravimo da je funkcija odvedljiva v $x$.

$\frac{f(x+h) - f(x)}{h}$ se imenuje diferenčni koeficient.

Odvod lahko zapišemo tudi kot 

$$f'(x_{0}) = \frac{df}{dx}(x_{0})$$



>[!|]- Pravila za odvajanje elementranih funkcij
   $$\frac{d}{dx} c = 0, $$
   $$\frac{d}{dx} x^n = n x^{n-1}, \quad n \in \mathbb{R}$$
   $$\frac{d}{dx} e^x = e^x$$  
   $$\frac{d}{dx} a^x = a^x \ln a, \quad a > 0$$
   $$\frac{d}{dx} \ln x = \frac{1}{x}$$  
   $$\frac{d}{dx} \log_a x = \frac{1}{x \ln a}, \quad a > 0, a \neq 1$$
   $$\frac{d}{dx} \sin x = \cos x$$  
   $$\frac{d}{dx} \cos x = -\sin x$$  
   $$\frac{d}{dx} \tan x = \sec^2 x, \quad x \neq \frac{\pi}{2} + k\pi$$  
   $$\frac{d}{dx} \cot x = -\csc^2 x, \quad x \neq k\pi$$  
   $$\frac{d}{dx} \sec x = \sec x \tan x, \quad x \neq \frac{\pi}{2} + k\pi$$  
   $$\frac{d}{dx} \csc x = -\csc x \cot x, \quad x \neq k\pi$$  
   $$\frac{d}{dx} \arcsin x = \frac{1}{\sqrt{1 - x^2}}, \quad |x| < 1$$  
   $$\frac{d}{dx} \arccos x = \frac{-1}{\sqrt{1 - x^2}}, \quad |x| < 1$$  
   $$\frac{d}{dx} \arctan x = \frac{1}{1 + x^2}$$  
   $$\frac{d}{dx} \text{arccot } x = \frac{-1}{1 + x^2}$$  
   $$\frac{d}{dx} \sinh x = \cosh x$$  
   $$\frac{d}{dx} \cosh x = \sinh x$$  


> Če je $f$ odvedljiva v točki $x$ je tam tudi zvezna.

> Če sta $f$ in $g$ odvedljivi potem je vsota, razlika, produkt, kvocientm kompozitum teh funkcij odvedljiva.

$$(fg)' = f'g+fg'$$

$$\left(\frac{f}{g}\right)' = \frac{f'g-fg'}{g^{2}}$$

$$(f \circ g)' = f'(g(x))g'(x)$$

Če je $f$ odvedljiva na intervalu $I$ in $f'(a) \neq 0$ za nek $a$ na intervalu potem je funkcija $f^{-1}$ diferanciabilna v $b = f(a)$.

$$(f^{-1}(b))' = \frac{1}{f'(a)}$$
$$(f^{-1}(b))' = \frac{1}{f'(f^{-1}(b))}$$

Naj bo $f$ deifnirana v točki $a$. Diferencial v točki je definiran kot 

$$df = f'(a)dx$$

oz. kot linearna funkcija

$$df(h) = Kh$$

kjer je $K$ poljubna konstanta. Ta konstanta naj bi zaradi naše zahteve da je

$$\lim_{h \to 0} \frac{|f(a+h)-f(a)-df(h)h|}{|h|} = 0$$

bila enaka $f'(a)$.

> Funkcija je odvedljiva v točki $a$ natanko tedaj ko je diferenciabilna v $a$

**Langrangev izrek** pravi da je če imamo funkcijo definirano na zaprtem intervalu in odvedljivo na istem ampak odprtem intervalu potem obstaja število $\xi \in (a,b)$ tako da velja $f(b)-f(a) = f'(\xi)(b-a)$

**Rollejev izrek** pravi da če imamo enako definirano funkcijo kot prej in vemo da je $f(a) = f(b)$ potem obstaja tako število $\xi \in (a,b)$ tako da velja $f'(\xi)= 0$ 

Funkcija je **Lipshitzova** če velja da obstaja konstanta $L$ nemanjša od 0 tako da za vse $x_{1}, x_{2}$ velja 

$$|f(x_1)-f(x_{2})| \leq L \cdot |x_{1}-x_{2}|$$

L deluje kot meja strmosti, ki je funkcija ne preseže.

> Če je funkcija zvezno odvedljiva na $[a,b]$, je Lipshitzova.

> Funkcija je na intervalu padajoča/naraščajoča če velja da je na istem intervalu odvod funkcije negativna/pozitivna.

Funkcija ke **konveksna** če velja

$$\forall x,a,b \in (a,b): f(x)\leq f(a) + \frac{f(b)-f(a)}{b-a}(x-a)
$$
$$ $$
$$\forall x,y \in I : f\left(\frac{x+y}{2}\right)\leq \frac{f(x)+f(y)}{2}$$

Funkcija ke **konkavna** če velja

$$\forall x,a,b \in (a,b): f(x)\geq f(a) + \frac{f(b)-f(a)}{b-a}(x-a)
$$
$$ $$
$$\forall x,y \in I : f\left(\frac{x+y}{2}\right)\geq \frac{f(x)+f(y)}{2}$$

> Konveksa funkcija je nujno zvezna

> Če je konveksna funkcija odvedljiva potem odvod funkcije narašča

















# Analiza 2


**Okolica** točke $a$ je vsak odprti interval $(a-\varepsilon, a +\varepsilon)$.


Točka je **notranja** če velja da obstaja njena okolica, ki vsebuje samo elemente iz množica. 
Točka je **robna** če velja, da za vsako njeno okolico velja da vsebuje vsaj en element iz množice in en element izven množice. 
Točka je **zunanja** če obstaja okolica, ki vsebuje samo elemente izven množice.


Množica je **odprta**, natanko tedaj ko za vsak $a$ obstaja taka okolica $a$, ki je popolnoma vsebovana v množici.
*Vse njene točke so notranje* 
Naj bo $X$ podmnožica $\mathbb{R}$. Množica $A \subset X$ je **odprta v $X$** če obstaja odprta množica $B \subset \mathbb{R}$ tako da velja $A = B \cap X$


Množica je **zaprta** če je komplement odprte. 
*Vsebuje vse svoje robne točke.*
***
> Množica $A$ je zaprta, natanko tedaj ko za vsako zaporedje v $A$ velja, če je $s$ stekališče potem je $s$ element $A$.
> $$ A \text{ je zaprta } \Leftrightarrow  \forall a_{n}\in A : s \text{ je stekališče } \Rightarrow s \in A$$
> >[!|dokaz]- Dokaz:
> >$\Rightarrow$
> >
> >**Predpostavimo, da je $A$ zaprta množica.**
> >
> >To pomeni, da je njen komplement $A^c$ odprt. 
> >
> >Vzemimo poljubno zaporedje $\{a_n\}$ v $A$, ki konvergira k $s$. Če bi bilo $s \in A^c$, bi obstajala okolica $x$, ki je v celoti vsebovana v $A^c$. 
> >
> >Ker $\{a_n\}$ konvergira k $s$, bi moralo biti neskončno členov zaporedja v tej okolici, kar pa je nemogoče, ker so vsi člani zaporedja v $A$. Zato mora biti $s \in A$.  
> >
> >$\Leftarrow$
> >
> >**Predpostavimo, da za vsako zaporedje $\{a_n\}$ v $A$, ki konvergira k $s$, velja $s \in A$.**
> >
> >Dokazati želimo, da je $A$ zaprta, torej da je $A^c$ odprta. Vzemimo poljuben $x \in A^c$. 
> >
> >Če bi vsaka okolica $x$ vsebovala elemente iz $A$, bi lahko konstruirali zaporedje v $A$, ki konvergira k $x$. Po predpostavki bi moralo biti $x \in A$, kar je v protislovju z $x \in A^c$. 
> >
> >Kar pomeni da ne velja da vsaka okolica $x$ vsebuje elemente iz $A$.
> >
> >Zato mora obstajati okolica $x$, ki je v celoti vsebovana v $A^c$, kar pomeni, da je $A^c$ odprta in posledično $A$ zaprta.

^4ca9f3

Množica je **kompaktna** če je zaprta in omejena hkrati.
***
> Množica $A$ je kompaktna natanko tedaj ko za vsako zaporedje v $A$ velja da ima stekališče v $A$.
> $$A \text{ je kompaktna } \Leftrightarrow \text{ vsako } a_{n} \in A \text{ ima stekališče v } A$$
> 
> >[!|dokaz]- Dokaz:
> >
> > $\Rightarrow$
> > 
> > **Predpostavimo da je $A$ kompaktna**
> > 
> > Vzamemo poljubno zaporedja $a_n$. 
> > 
> > Kompaktna množica je zaprta in omejena. 
> > 
> > Če je zaporedje omejeno v $\mathbb{R}^{n}$ ima vsaj eno stekališče. 
> > 
> > Ker je $A$ zaprta mora le to ležati v $A$. 
> > 
> > Torej ima zaporedje $a_n$ stekališče v $A$.
> > 
> > $\Leftarrow$
> > 
> > **Predpostavimo da ima vsako zaporedje v $A$ stekališče v $A$**
> > 
> > **Zaprtost:** Vzamemo poljubno zaporedje $a_{n}$, ki konvergira k $a$. Ker ima vsako zaporedje v $A$ stekališče v $A$ mora biti $a$ stekališče $a_{n}$, torej je $a \in A$, kar pomeni da je množica zaprta. 
> > 
> > *Izhaja iz izreka o zaprtih množicah in stekališčih.*
> > 
> > **Omejenost:** Recimo da $A$ ni omejena. Potem obstaja zaporedje za katerega velja da je $a_{n} \rightarrow \infty$. Takšno zaporedje nima stekališča v $A$, kar je prostislovje s predpostavko, torej mora biti $A$ omejena.
***
**Evklidski prostor **

$$\mathbb{R}^{k} = \{ x = (x_1,...,x_{k}) \;;\; x_i \in \mathbb{R} \}$$

je vektorski prostor, kjer definiramo seštevanje po komponentah, množenje s sklarjem po komponentah in dolžino oz. normo.

**Norma** oz .dolžina je oddaljenost $x$ od $O(\mathbb{R}^n)$
$$\Vert x \Vert = \sqrt[]{x_{1}^{2}+...+x_{k}^{2}}$$

Razdalja med dvema točkama pa je

$$\Vert x -y\Vert = \sqrt[]{(x_{1}-y_{1})^{2}+ ...+ (x_{k}-y_{k})^2}$$

Definirana je tudi **trikotniška neenakost**

$$\Vert x+y \Vert \leq \Vert x \Vert + \Vert y \Vert$$

$$\left| \Vert x \Vert - \Vert y \Vert \right| \leq \Vert x+y \Vert$$

**Odprta krogla** s središčem v $a$ in radijem $r$ v $\mathbb{R}^{k}$ je $K(a, r) = \{ x \in \mathbb{R}^{k} \;;\; \Vert x-a \Vert < r\}$

**Epsilonska okolica** točke $x$ je odprta krogla $K(x, \varepsilon)$, $\varepsilon > 0$

Množica je **omejena**, če obstaja $M > 0$, da je $A \subset K(0, M)$ oz. $\Vert x \Vert < \Vert M \Vert$

Množica je **končna**, če ima končno število elementov oz. obstaja bijektivna preslikava $A \rightarrow \{ 1,2,...,n\}$

Množica je **odprta** če za vsak $x \in A$ obstaja okolica $x$, ki je popolnoma vsebovana v $A$.

Množica je **zaprta**, če je njen komplement odprta množica.
*Množica je zaprta ko vsebuje vse svoje robne točke.*

Točka je **notranja** če obstaja njena okolica, ki je popolnoma vsebovana v množici.

Točka je **stekališče** **množice** $A$ če vsaka njena okolica seka $A\backslash \{x\}$.

$$K(x, \varepsilon) \cap (A\backslash \{ x\}) \neq \emptyset$$

*Točka je stekališče množice $A$ če za vsako njeno okolico velja da vsebuje neskončno členov množice*

Točka $a$ je **izolirana točka**, če ni stekališče.

**Zaporedje v $\mathbb{R}^{k}$** je preslikava

$$\mathbb{N} \rightarrow \mathbb{R}^{k}$$
$$n \mapsto (x_{1}^{n},...,x_{k}^{n})$$

**Limita** $a_n$ je $a$, če $\forall \varepsilon>0 \;\; \exists n_{0} \,\ni: n>n_{0} :  \Vert a-a_{n} \Vert < \varepsilon$
***
> Če zaporedje konvergira k $L$, potem vsako podzaporedje konvergira k $L$
> >[!|dokaz]- Dokaz:
> > tba
***
Zaporedje ima **limito v neskočnosti**, če velja da so za vsak $M > 0$ vsi členi zaporedja od nekega indeksa naprej zunaj $K(0, M)$.

**Stekališče** $s$ zaporedja $a_{n}$ je če vsaka njegova okolica vsebuje neskončno elementov.
*Je stekališče, če obstaja podzaporedje, ki konvergira k $s$.*
***
> Vsako konvergetno zaporedje je omejeno in ima natanko 1 stekališče, ki je njegova limita.
> 
> >[!|dokaz]- Dokaz:
> >
> >1.$\;$ Vsako konvergentno zaporedje je omejeno:
> >
> > **Vzamemo konvergentno zaporedje $a_{n}$**
> > 
> > Pomeni da za vsak $\varepsilon$ obstaja $n_{0}$, da so vsi členi od tam naprej v neki okolici limite $L$.
> > 
> > Če razdelimo zaporedje na del od $n_{0}$ naprej in nazaj, vemo da je eno omejeno v okolici $L$, drugo pa je končno, končno zaporedje pa je **omejeno**.
> > 
> > 2.$\;$ Zaporedje ima limito $L$ $\Leftrightarrow$ $L$ je edino stekališče zaporedja
> > 
> > $\Rightarrow$
> > 
> > **Predpostavimo da ima limito $L$**
> > 
>> Predpostavimo da obstaja drugo stekališče. 
>> 
>> Potem obstaja podzaporedje, ki konvergira k tej limiti.
>> 
>> Ker $a_n$ konvergira k $L$ mora tudi vsako podzaporedje konvergirati k $L$. (ref.)
>> 
>> 
>> To je protislovje, ker lahko vzmamemo dovolj majhen epsilon da sta množici disjunktni, element zaporedja pa ne more biti hkrati v dveh disjunktnih množicah. Torej je limita edino stekališče.
>> 
> > $\Leftarrow$ 
> > 
> > **Predpostavimo da je $L$ edino stekališče zaporedja.**
> > 
> > Ker vemo, da je v vsaki $\varepsilon$ okolici $L$ neksončno členov, potem mora biti zunaj okolice končno členov. Torej mora obstajati končno število elementov za katere velja da niso v okolici. 
> > 
> > Naj bo $N$ indeks zadnjega elementa izven okolice. To pomeni da za vse člene $n>N$ velja da so v $\varepsilon$ okolici $L$ oz. $|L - a_{n}| < \varepsilon$ kar je definicija limite.
***

> Vsako omejeno zaporedje ima stekališče
> 
> $$ a_{n} \text{ je omejeno } \Leftrightarrow a_{n}\text{ ima stekališče}$$
> 
> >[!|dokaz]+ Dokaz Bolzano-Weierstrassovega izreka:
> >
> >Naj bo $(a_n)$ omejeno zaporedje realnih števil. To pomeni, da obstajata takšni realni števili $m$ in $M$, da za vsak člen zaporedja velja:
> >$$ m \leq a_n \leq M \quad \text{za vse } n \in \mathbb{N}.$$
> > Začnemo z intervalom $I_0 = [m, M]$, ki vsebuje vse člene zaporedja $(a_n)$.
> > Interval $I_0$ razdelimo na dva sklenjena podintervala: $[m, \frac{m+M}{2}]$ in $[\frac{m+M}{2}, M]$.
> >Vsaj eden od teh dveh podintervalov vsebuje neskončno členov zaporedja $(a_n)$. Izberemo ta podinterval in ga označimo z $I_1$.
> > Postopek ponavljamo: vsak interval $I_k$ razdelimo na dva sklenjena podintervala in izberemo tistega, ki vsebuje neskončno členov zaporedja. Tako dobimo zaporedje intervalov $I_0 \supseteq I_1 \supseteq I_2 \supseteq \dots$, kjer je dolžina intervala $I_k$ enaka $\frac{M - m}{2^k}$.
> >
> > V vsakem intervalu $I_k$ izberemo en člen zaporedja $(a_n)$, ki pripada temu intervalu. Ker vsak $I_k$ vsebuje neskončno členov, lahko vedno izberemo nov člen, ki še ni bil izbran v prejšnjih korakih.
> >Tako dobimo podzaporedje $(a_{n_k})$, kjer je $a_{n_k} \in I_k$ za vsak $k$.
> >
> >
> >Ker so intervali $I_k$ vedno manjši (njihova dolžina konvergira k 0) in se vedno bolj "zožajo" okoli neke točke, obstaja točka $L$, ki je presečišče vseh intervalov $I_k$.
> >Podzaporedje $(a_{n_k})$ konvergira k $L$, saj so vsi členi $a_{n_k}$ vsebovani v intervalih $I_k$, ki se zožujejo okoli $L$.
> >
> >
> >Točka $L$ je stekališče zaporedja $(a_n)$, saj obstaja podzaporedje $(a_{n_k})$, ki konvergira k $L$.

***

> Stekališče zaporedja je limita konvergentnega podzaporedja
> >[!|dokaz]- Dokaz:
> >Naj bo $L$ točka, za katero velja, da v vsaki $\epsilon$-okolici točke $L$ leži neskončno členov zaporedja $(a_n)$. Potem lahko konstruiramo podzaporedje $(a_{n_k})$, ki konvergira k $L$, na naslednji način:
> >
> >Izberemo $\epsilon = 1$. V okolici $L$ z radijem $1$ obstaja neskončno členov zaporedja $(a_n)$. Izberemo poljuben člen iz te okolice in ga označimo z $a_{n_1}$.
> >
> > Nato izberemo $\epsilon = \frac{1}{2}$. V okolici $L$ z radijem $\frac{1}{2}$ obstaja neskončno členov zaporedja $(a_n)$. Izberemo člen $a_{n_2}$, kjer je $n_2 > n_1$, da zagotovimo, da gre za podzaporedje.
> >
> >Postopek ponavljamo za $\epsilon = \frac{1}{k}$ za vsak $k \in \mathbb{N}$. V vsakem koraku izberemo člen $a_{n_k}$, kjer je $n_k > n_{k-1}$, tako da $|a_{n_k} - L| < \frac{1}{k}$.
> >
> >Tako konstruirano podzaporedje $(a_{n_k})$ konvergira k $L$, saj za vsak $\epsilon > 0$ obstaja takšen $K$, da za vse $k \geq K$ velja:
> >$$|a_{n_k} - L| < \frac{1}{k} \leq \epsilon.$$
***

> Če so $K_{1},...,K_{k}$ kompaktne je kompaktna $K_{1} \times...\times K_{k}$ kompaktna v $\mathbb{R}^{k}$.
> >[!|dokaz]+ Dokaz:
> >
> >Vsaka množica $K_{i}$ ($i = 1, 2, \dots, k$) je kompaktna v $\mathbb{R}$. Toje  ekvivalentno temu, da je vsaka $K_{i}$ zaprta in omejena.
> >
> >Kartezični produkt $K = K_{1} \times K_{2} \times \dots \times K_{k}$ je definiran kot:
> > **Zaprto:** Kartezični produkt zaprtih množic je zaprt. Ker je vsaka $K_i$ zaprta, je tudi $K$ zaprta.
> > **Omejeno:** Kartezični produkt omejenih množic je omejen. Ker je vsaka $K_i$ omejena, obstaja neka konstanta $M_i > 0$, da velja $|x_i| \leq M_i$ za vsak $x_i \in K_i$. Potem je vsak vektor $(x_1, x_2, \dots, x_k) \in K$ omejen z:
> >  $$ \|(x_1, x_2, \dots, x_k)\| \leq \sqrt{M_1^2 + M_2^2 + \dots + M_k^2}.$$
> >  Zato je $K$ omejena.
   
### Funkcije več spremenljivk


Funkcije več spremenljivk so funkcije, odvisne od dveh ali več spremenljivk. Slikajo iz $\mathbb{R}^{k}$ v $\mathbb{R}$, kjer je $k \geq 2$.

Graf funkcije $f$ je množica 

$$\Gamma = \{ (x, f(x)) \;;\; x \in D \}$$
$$\Gamma  \subset \mathbb{R}^{k} \times \mathbb{R} = \mathbb{R}^{k+1}$$

**Defincijsko območje** je množica vrednosti neodvisnih spr., za katere je $f$ definirana.

**Kodomena** je množica v katero funkcija slika svoje elemente, ta pa lahko vsebuje elemente, ki niso z definicijskega območja.

**Zaloga vrednosti** je množica vseh dejanskih vrednosti, ki jih funkcija zazvzame.

**Izolipse** so krivulje, ki povezujejo točke z enako vrednostjo neke funkcije dveh spremenljivk. *\[ "isos" (enak) in "lipsa" (vrednost)]*
*Izolipsa za dano $f(x,y)$ je množica točk za katero velja $f(x,y) = C$.*

Izolipse se ne sekajo, ker bi drugače to pomenilo da ima $f$ dve različni vrednosti pri istem $x$.

Goste izolipse nakazuje strmost, redke položnost.

Izolipse so tudi presek grafa z ravnino.

Funkcije rišemo s pomočjo izolips, tako da 

**Limita funkcije** naj bo $(a,b) \in \mathbb{R}^k$ **stekališče**. Potem velja da je $L$ limita funkcije če velja

$$ \forall  \varepsilon > 0\;\; \exists \delta > 0 \;\;\forall (x,y) \in D : $$ 
$$ 0 < \Vert  (x,y)-(a,b)\Vert < \delta \Rightarrow   | f(x,y) - L | < \varepsilon$$

Desna in leva limita v večdimnezijah nimata pomena.

***

> Če obstaja limita je enolična

***

> Limita vsote, razlike, produkta in kvocienta funkcij je enaka vsoti, razliki, produktu, kvocientu limit funkcij.






