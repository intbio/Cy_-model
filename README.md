# Cy_model
Краткая сводка информации по циановым меткам, которые мы используем

## Циановые метки
| Флюорофоры        | Ex(nm)           | Em(nm)  |Q<sub>y</sub> |Радиус красителя (Å)|
| ----------------- |:----------------:|:-------:|:------------:|:--------------:|
| Cy3 | 553<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup> | 568<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup>|0,15<sup>[2](https://www.atdbio.com/content/32/Cyanine-dyeshttps://www.atdbio.com/content/32/Cyanine-dyes)</sup>|7<sup>[3](#id1)</sup>|
| Cy5 | 653<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup> | 672<sup>[1](https://www.chroma.com/spectra-viewer?fluorochromes=10382%2C10384)</sup>|0,27<sup>[2](https://www.atdbio.com/content/32/Cyanine-dyes)</sup> |8<sup>[3](#id1)</sup>|\
- Ex (нм): длина волны возбуждения в нанометрах
- Em (нм): длина волны излучения в нанометрах
- Q<sub>y</sub>: квантовый выход
-  Мы используем Cy3 и Cy5 с линкерами от [Lumiprobe](https://ru.lumiprobe.com/order-oligo/) и [Syntol](https://www.syntol.ru/catalog/modifitsirovannye-oligonukleotidy/aminolinkery.html)
<img src="https://github.com/intbio/Cy_model/blob/main/Image/Cyanine3and5.png" width="600"> 

<a id="id1"></a> 
**3** - Радиусы крсителей измерялся в програме [Avogadro](https://avogadro.cc/) как указано на рисунке ниже:
<img src="https://github.com/intbio/Cy_model/blob/main/Image/%D0%9D%D0%BEs.jpeg" width="500">


 ## Циановые метки от Lumiprobe
 
 <img src="https://github.com/intbio/Cy_model/blob/main/Image/cy_lumiprobe_side.png" width="850">

 ## Циановые метки от Syntol

 <img src="https://github.com/intbio/Cy_model/blob/main/Image/Cy_all.png" width="850">

|Компания|Флюорофоры|Радиус красителя (Å)|Длина линкера(Å)       |Число связей       |Медианная длина красителя с линкером (Å)|
| -------|:--------:|:------------------:|:---------------------:|:--------------------:|:-------------------------:|
|Lumiprobe|Cy3      |7<sup>[3](#id1)</sup>|10<sup>[4](#id2)</sup>|25<sup>[5](#id4)</sup>|25<sup>[6](#id3)</sup>|
|Lumiprobe|Cy5      |8<sup>[3](#id1)</sup>|10<sup>[4](#id2)</sup>|25<sup>[5](#id4)</sup>|28<sup>[6](#id3)</sup>|
|Syntol|Cy3         |7<sup>[3](#id1)</sup>|9<sup>[4](#id2)</sup> |19<sup>[5](#id4)</sup>|18<sup>[6](#id3)</sup>|
|Syntol|Cy5         |8<sup>[3](#id1)</sup>|9<sup>[4](#id2)</sup> |19<sup>[5](#id4)</sup>|20<sup>[6](#id3)</sup>|

<a id="id2"></a>
**4** - Расчеты длины линкера быле произведены по упращенной моделе (где линке представлен в виде алкана), из кол-ва связей и длины связи С-С раситывалась средняя длина линкера<sup>[7](http://www.chem.msu.su/rus/teaching/lachinov-basic/part012.html)</sup><sup>[8](https://www.theorie.physik.uni-muenchen.de/lsfrey/teaching/archiv/sose_06/softmatter/talks/Peter_Jensen-Polymers.pdf)</sup>.\
Формула: 

![\begin{align*}
R=\sqrt\frac{1+ cos \theta}{1-cos\theta}\sqrt{N}l
\end{align*}
](https://render.githubusercontent.com/render/math?math=%5CLARGE+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0AR%3D%5Csqrt%5Cfrac%7B1%2B+cos+%5Ctheta%7D%7B1-cos%5Ctheta%7D%5Csqrt%7BN%7Dl%0A%5Cend%7Balign%2A%7D%0A)

Где N - число связий; l - длинна связи = 0,15 нм(1.5 A); θ - внешний угол связи = 70.33°\
<a id="id4"></a>
**5** - Количество связей от кольца основания до N красителя\
Стосит отметить что в линкере от lumiprobe помимо большего количества связий, в центре линкера присудствует 5-ти членное кольцо с тремя N. \
<a id="id3"></a>
**6** - Медианная длина красителя с линкером расчитывалась по коду лежащему на Jupyter по пути: _projects/2020_MD_FRET_modelling_NV/Md_analysis/FRETstein (1).ipynb
