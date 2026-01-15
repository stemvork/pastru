# Complexe getallen

Wiskunde heeft geen eindpunt: het is een actief onderzoeksgebied met vele praktische toepassingen. Misschien is wiskunde wel begonnen met tellen. Aan de behoefte om te tellen danken we de natuurlijke getallen:

$$
\mathbb{N}_0=\{0,1,2,3,\ldots\}
$$

Hoeveel balen hooi zijn er op voorraad? Hoeveel schapen en kippen hebben wij? Maar het blijft geen feest, er zijn ook tekorten. Om daarmee te rekenen zijn negatieve getallen best handig. Zo kregen we de verzameling van gehele getallen:

$$
\mathbb{Z}=\{\ldots,-3,-2,-1,0,1,2,3,\ldots\}
$$

Op de basisschool leerde jij over delingen. Wanneer we vijf door twee delen, krijgen we twee rest één. Op zich prima, maar om te rekenen met dit soort uitkomsten zijn breuken handiger! De verzameling van alle gebroken getallen heet de **rationele** getallen:

$$
\mathbb{Q}=\left\{\frac{p}{q}\mid p,q\in\mathbb{Z},\ q\neq 0\right\}
$$

Op de middelbare school leerde je dan weer over kwadraten en hun inverse: wortels. Die uitkomsten zijn (meestal) niet te schrijven als breuk. Ondertussen bereiken we de verzameling van reële getallen:

$$
\mathbb{R}
$$

Daar behoort ook $\pi$ toe.

---

## Vergelijkingen en het “domein” van oplossingen

Een groot aantal problemen binnen de wiskunde vereist het oplossen van vergelijkingen of ongelijkheden. Het aantal oplossingen van een vergelijking hangt af van een keuze: **in welke verzameling getallen gaan we zoeken?**

In de natuurlijke getallen $\mathbb{N}_0$ heeft de vergelijking

$$
x+1=0
$$

bijvoorbeeld geen oplossing. Want de oplossing $x=-1$ behoort tot de verzameling van gehele getallen $\mathbb{Z}$.

Bedenk zelf eens een vergelijking die je kunt oplossen en ga na in welke verzameling de oplossingen thuishoren.

Een andere situatie zonder oplossingen kwamen we tegen bij kwadratische vergelijkingen. De vergelijking

$$
x^2+4=0
$$

heeft geen oplossingen in $\mathbb{R}$, want bij $x^2=-4$ kunnen we geen worteltrekken: het rechterlid is negatief.

Of je zou ook de discriminant van

$$
x^2-4x+10=0
$$

kunnen bepalen:

$$
D=16-40=-24
$$

Omdat $D<0$ zijn er geen reële oplossingen. Nou ja… **in welke verzameling getallen dan?** De grootste verzameling die je tot nu toe kent is die van de reële getallen.

---

## Zijn er meer getallen?

Zijn er meer getallen? Wat is überhaupt een getal? Jeetje, dan gaan we wel erg diep hoor.

Zoals je hierboven leest, zou je kunnen stellen dat getallen oplossingen van vergelijkingen zijn. En dat nieuwe verzamelingen getallen ons nieuwe oplossingen van vergelijkingen kunnen geven.

Voor het werken met getallen hebben we allerlei regels en vaardigheden geleerd. Die hoorden dan bij die soort getallen. We leerden regels over breuken, negatieve getallen en wortels, die soms algemeen (voor alle getallen) en dan weer specifiek waren.

Er is in de geschiedenis vaak genoeg weerstand geweest tegen nieuwe soorten getallen. Want _nul_ bestaat toch helemaal niet? Eindeloze discussies. En negatieve getallen, daar waren de Babyloniërs bang voor! Zelf heb je misschien ook wel eens het achterhoofd gekrabt als je leerde over de verschillende soorten getallen.

Ze zijn sterk verweven met hoe wij als mensen denken. Maar één ding is duidelijk: als een verzameling getallen een praktisch nut had, dan was de acceptatie dichtbij.

---

## Een nieuw getal: $i$

In dit hoofdstuk leer je een nieuwe verzameling getallen: de **complexe getallen**. Daarmee kunnen we meer soorten vergelijkingen oplossen, en krijgen we nieuwe getallen met hun eigen rekenregels en bijzonderheden.

Die ontdekkingstocht begint bij de volgende vraag:

> Wat als er een getal is, dat in het kwadraat $-1$ geeft?

Dat kan toch niet, want een kwadraat is altijd positief… *(weerstand!)*  
Vanaf nu spreken we af dat er tóch zo’n getal bestaat. We noemen het $i$ en we leggen vast:

$$
i^2=-1
$$

Dit $i$ heet de **imaginaire eenheid**.

---

## Complexe oplossingen bij een kwadratische vergelijking

Nu kunnen we bijvoorbeeld de vergelijking

$$
z^2+25=0
$$

oplossen. Want dat komt neer op:

$$
z^2=-25
$$

En omdat $i^2=-1$, mogen we ook schrijven:

$$
-25 = 25i^2
\quad\Rightarrow\quad
z^2 = 25i^2
$$

Hier zou je misschien willen worteltrekken:

$$
z=\sqrt{25i^2}=\sqrt{25}\sqrt{i^2}=5i
$$

Maar eerlijk is eerlijk: we hebben nog niet geleerd of dat *altijd* mag in deze nieuwe wereld. Misschien ontploft de wereld dan wel, zoals bij delen door nul 😉

Dus we redeneren vanaf de andere kant:

- $z=5i$ kan een oplossing zijn, want

  $$
  z^2=(5i)^2=25i^2=-25
  $$

  en dus klopt $z^2+25=0$.

Maar er zijn er meer, want $z=-5i$ is ook een oplossing!

$$
z^2=(-5i)^2=25i^2=-25
\quad\Rightarrow\quad
z^2+25=0
$$

Er zijn dus twee complexe oplossingen, namelijk:

$$
z=5i
\quad\text{en}\quad
z=-5i
$$

Net zoals de vergelijking

$$
x^2=16
$$

twee oplossingen heeft:

$$
x=4
\quad\text{en}\quad
x=-4
$$

De getallen die een veelvoud van $i$ zijn noemen we **imaginair**, omdat we ze ons vroeger moeilijk konden voorstellen. We schrijven de imaginaire getallen als:

$$
bi \quad \text{met } b\in\mathbb{R}
$$

En voor het imaginaire getal $i$ geldt dus altijd:

$$
i^2=-1
$$

Vanaf nu kun je dus ineens **alle kwadratische vergelijkingen** oplossen…  
(in $\mathbb{C}$, de verzameling van complexe getallen dan, dat dan weer wel 😉).
