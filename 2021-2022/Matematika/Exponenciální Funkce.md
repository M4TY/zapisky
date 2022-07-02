# Exponenciální Funkce

| **Číslo matematika** |**Část piva**||
|:-:|:-:|-:|
|0|1|$(\frac 1 2)^0$|
|1|$\frac 1 2$|$(\frac 1 2)^1$|
|2|$\frac 1 4$|$(\frac 1 2)^2$|
|3|$\frac 1 8$|$(\frac 1 2)^3$|
|4|$\frac 1 {16}$|$(\frac 1 2)^4$|
|**x**|**y**|$(\frac 1 2)^x$|
|-1|2|$(\frac 1 2)^{-1}$|
|-2|4|$(\frac 1 2)^{-2}$|
|-3|8|$(\frac 1 2)^{-1}$|

<hr>

### $f: y = (\frac 1 2)^x$  
### $D_f = \mathbb{R}$  
### $H_f = \mathbb{R}^+$
<iframe src="https://www.desmos.com/calculator/6mzsphqqot?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
<hr>

### Def: <u>Exponenciální funkce</u> o základu <u>a</u> je funkce $y=a^x$, kde $a \in \mathbb{R}^+-\{1\}$
### Pozorování: 
- $D = \mathbb{R}, H = \mathbb{R}^+$
- Nemají maximum ani minimum
- Zdola omezená 0 (shora ne)
- Je na celém D prostá
- $a \in (0, 1)...klesající$
- $a \in (1, \infin)...rostoucí$
- Grafem je exponenciála
- Graf vždy prochází bodem $[0; 1]$  

<hr>

**Př.:**  
$1.5^p > 1.5^r$  
$p >r$ 

$0.3^p > 0.3^r$  
$p < r$

$(\frac 3 7)^{6.24} < 1$  

$(\frac 8 5)^{2\pi} > (\frac 8 5)^{0.5\pi}$  

<hr>

## Transformace grafů exponenciálních funkcí
**Př.:** Nakreslete grafy funkcí:  
$f: y = 2^x$  
<iframe src="https://www.desmos.com/calculator/kjdubacbni?embed" width="300" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>  

$g: y = -2^x$  
<iframe src="https://www.desmos.com/calculator/3bojmdze6g?embed" width="300" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>

$h: y = 2^{-x}$  
<iframe src="https://www.desmos.com/calculator/6j7gg2py0b?embed" width="300" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>

$i: y = 2^{x+3}$  
<iframe src="https://www.desmos.com/calculator/5mtpiminmk?embed" width="300" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>

$j: y = 2^{3-x}$  
<iframe src="https://www.desmos.com/calculator/tw56m7ny3c?embed" width="300" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>

$k: y = 2^x-5$  
<iframe src="https://www.desmos.com/calculator/12itqqtvrp?embed" width="300" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>


<span style="font-size: 32px">$a^{x+n}+m$</span>  
### Když je $a$ záporné, graf se převrácí podle osy x  
### $n$ posouvá podle osy x
### $m$ posouvá podle osy y
### Když je $a$ v intervalu $(0; 1)$, graf se převrácí podle osy y
### Když je $x$ záporné, graf se převrácí podle osy y

<hr>

$l: y = -2^{x-2}+3$  
<iframe src="https://www.desmos.com/calculator/tu01drzfjn?embed" width="300" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>  

<hr>

## Exponenciální rovnice

**Př.:**  
$$
\begin{aligned}
    5^3 & = 5^x \\
    x & = 3
\end{aligned}
$$  

**Platí:** Pro každé $x$ a $y$ $\in \mathbb{R}$ a pro každé $a \in \mathbb{R}-\{1\}$ platí:   
$$
a^x = a^y => x = y
$$

<hr>

**Př.:** Řešte rovnice pro $x \in \mathbb{R}$:
### 1) $(\frac 1 3)^{x-4} = (\frac 1 3)^{19x+2}$
$$
\begin{aligned}
    (\frac 1 3)^{x-4} & = (\frac 1 3)^{19x+2} \\
    x-4 & = 19x+2 \\
    -6 & = 18x \\
    -\frac 6 {18} & = x \\
    -\frac 1 3 & = x
\end{aligned}
$$
### 2) $15^3 * 15^{x*2} = 15^{-x}$
$$
\begin{aligned}
    15^3 * 15^{x*2} & = 15^{-x} \\
    3 +x*2 & = -x \\
    3x & = -3 \\
    x & = -1
\end{aligned}
$$
### 3) $\frac{6.8^{x^{2}}}{6.8^3} = 6.8^{-2x}$
$$
\begin{aligned}
    \frac{6.8^{x^{2}}}{6.8^3} & = 6.8^{-2x} \\
    6.8^{x^2-3} & = 6.8^{-2x} \\
    x^2-3 & = -2x \\
    x^2+2x-3 & = 0 \\
    x_1 & = 1 \\
    x_2 & = -3
\end{aligned}
$$
### 4) $13^{2+x} = (\frac 1 {13})^x$
$$
\begin{aligned}
    13^{2+x} & = (\frac 1 {13})^x \\
    13^{2+x} & = 13^{-x} \\
    2+x & = -x \\
    2 & = -2x \\
    -1 & = x
\end{aligned}
$$
### 5) $25^x = 5^2*5^3/5^5$
$$
\begin{aligned}
    25^x & = 5^2*5^3/5^5 \\
    5^{x^2} & = 5^2*5^3/5^5 \\
    5^{x^2} & = 5^0 \\
    x^2 & = 0 \\
    x & = 0
\end{aligned}
$$