# Cy_model
Краткая сводка информации по циановым меткам, которые мы используем

## Циановые метки
| Флюорофоры        | Ex(nm)           | Em(nm)  |Q<sub>y</sub> |Радиус красителя (Å)|
| ----------------- |:----------------:|:-------:|:------------:|:--------------:|
| Cy3 | 553<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup> | 568<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup>|0,15<sup>[2](https://www.atdbio.com/content/32/Cyanine-dyeshttps://www.atdbio.com/content/32/Cyanine-dyes)</sup>|7|
| Cy5 | 653<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup> | 672<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup>|0,27<sup>[2](https://www.atdbio.com/content/32/Cyanine-dyes)</sup> |8|\
- Ex (нм): длина волны возбуждения в нанометрах
- Em (нм): длина волны излучения в нанометрах
- Q<sub>y</sub>: квантовый выход
<img src="https://github.com/intbio/Cy_model/blob/main/Image/Cyanine3and5.png" width="600">

 Мы использыем Cy3 и Cy5 с линкерами от [Lumiprobe](https://ru.lumiprobe.com/order-oligo/) и [Syntol](https://www.syntol.ru/catalog/modifitsirovannye-oligonukleotidy/aminolinkery.html)
 ## Циановые метки от Lumiprobe
 
 <img src="https://github.com/intbio/Cy_model/blob/main/Image/cy_lumiprobe_side.png" width="850">

 ## Циановые метки от Syntol

 <img src="https://github.com/intbio/Cy_model/blob/main/Image/Cy_all.png" width="850">

|Компания|Флюорофоры|Радиус красителя (Å)|Длина Линкера|Медиальная длина красителя с линкером (Å)|
| -------| -------- |:------------------:|:-----------:|--------------------------:|
|Lumiprobe|Cy3      |7                   |10|28|
|Lumiprobe|Cy5|8|10|25|
|Syntol|Cy3|7|9|25|
|Syntol|Cy5|8|9|25|

Расчеты длины линкера быле произведены по упращенной моделе (где линке представлен в виде алкана), из кол-ва связей и длины связи С-С раситывалась средняя длина линкера<sup>[3](http://www.chem.msu.su/rus/teaching/lachinov-basic/part012.html)</sup>.\
Формула: 

![\begin{align*}
R=\sqrt(\frac{1+ cos \theta}{1-cos\theta}N)l
\end{align*}
](https://render.githubusercontent.com/render/math?math=%5Chuge+%5Ctextstyle+%5Cbegin%7Balign%2A%7D%0AR%3D%5Csqrt%28%5Cfrac%7B1%2B+cos+%5Ctheta%7D%7B1-cos%5Ctheta%7DN%29l%0A%5Cend%7Balign%2A%7D%0A)

Где N - число связий; l - длинна связи = 0,15 нм(1.5 A); θ = 70.33°
