### vektorok, normák

Két dimenzióban dolgozunk.

* _vektor:_ (geometriailag) egy "nyíl" a koordinátarendszerben, ami (algebrailag) egy sima számpár, pl: ![eq](http://latex.codecogs.com/png.latex?v=(3,2))

* _norma:_ megmondja, hogy egy vektor "mekkora", ez sokféleképpen érthető, ezért sokféle norma van, alább ![eq](http://latex.codecogs.com/png.latex?L_i)-vel jelöljük őket

* _normalizálás:_ a vektort (koordinátánként) elosztjuk a normával, azaz a méretével, így a mérete 1 lesz, azaz _egységvektort_ kapunk, a tehát méretét "elimináljuk" :arrow_right: marad az _iránya_

|név|képlet|![eq](http://latex.codecogs.com/png.latex?L_i(v))|egységvektor|intuitíve|"elhelyezkedés"|
|--|--|--|--|--:|--|
|![eq](http://latex.codecogs.com/png.latex?L_1), Manhattan, taxi|![eq](http://latex.codecogs.com/png.latex?L_1(x)=\sum{x_i})|![eq](http://latex.codecogs.com/png.latex?L_1(v)=3+2=5)|![eq](http://latex.codecogs.com/png.latex?\left(\frac35,\frac25\right))|összeg = 1|"gyémánt"|
|![eq](http://latex.codecogs.com/png.latex?L_2), euklidészi, Frobenius|![eq](http://latex.codecogs.com/png.latex?L_2(x)=\sqrt{\sum{x_i^2}})|![eq](http://latex.codecogs.com/png.latex?L_2(v)=\sqrt{3^2+2^2}=\sqrt{13})|![eq](http://latex.codecogs.com/png.latex?\left(\frac{3}{\sqrt{13}},\frac{2}{\sqrt{13}}\right))|hossz = 1|kör|
|![eq](http://latex.codecogs.com/png.latex?L_\infty), max, Csebisev, sakktábla|![eq](http://latex.codecogs.com/png.latex?L_\infty(x)=\max\\\{x_i\\\})|![eq](http://latex.codecogs.com/png.latex?L_\infty(v)=\max\\\{3,2\\\}=3)|![eq](http://latex.codecogs.com/png.latex?\left(1,\frac23\right))|max = 1|négyzet|

### ![eq](http://latex.codecogs.com/png.latex?L_1) norma, valószínűségi eloszlás

__Megfigyelés:__ ![eq](http://latex.codecogs.com/png.latex?L_1) norma esetén az egységvektor értékeinek összege 1, azaz az egységvektor egy diszkrét valószínűségi eloszlás lesz (vagy legalábbis értelmezhető akként), azaz _az ![eq](http://latex.codecogs.com/png.latex?L_1) norma "valószínűségi eloszlásra" normalizál._ (Azaz értelmezhető a valószínűségi eloszlások "iránya", ill. az összes valószínűségi eloszlás a valahány dimenziós origó közepű "gyémánt" felszínén helyezkedik el...)

Szóval, ha minden jól megy, akkor egy vektornak meg tudunk feleltetni egy valszg eloszlást és viszont. Így az egyik területen lévő dolgok alkalmazhatóvá válnak a másik területen!

A sorrend kérdése se tűnik gondnak: a vektoroknál és a valszg eloszlásoknál is _számít_ az értékek sorrendje.
![eq](http://latex.codecogs.com/png.latex?KL\left(\left(\frac35,\frac25\right),\left(\frac25,\frac35\right)\right)\neq0)


__ötlet:__ cosinus távolság valszg eloszlásokra? Oké, de csak azonos dimenzióban. (Hm.. nem is, hiszen mindenképp van bezárt szög. Hm.. de nem egyértelmű, mert úgy helyezed el a kisebb dim teret a nagyobban, ahogy szeretnéd, pl. akár úgy, hogy egybeessen a két vektor. Szóval ez problémás.)

__ötlet:__ KL-divergence (![eq](http://latex.codecogs.com/png.latex?L_1) normált) vektorokra? Oké, de ez is csak azonos dimenzióban.
