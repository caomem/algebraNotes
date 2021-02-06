# Relações de Equivalência e Partições

**Partição**: União de conjuntos disjuntos;


**Relação de equivalência**: Sejam $a,b\in S$, $a\sim b$ e

- *Transitiva*. $a\sim b, b\sim c$ então $a\sim c$
- *Simétrica*. $a\sim b \implies b\sim a$
- *Reflexiva*. $a\sim a$

Partições induzem uma relação de equivalência e uma relação de equivalência *particiona o conjunto* em
**Classes de equivalência**.

**Proposição:** $d \in C_a$ e $d \in C_b \implies C_a = C_b$

**Notação:** *representante* $a\in S$, $\bar{a}\in \bar{S}$, $\bar{S}$ é o conjunto de partições ou classes de equivalência.

**Relação Induzida:** Uma aplicação $\varphi: S \longrightarrow T$ pode induzir uma relação de equivalência $\varphi(a)=\varphi(b) \implies a \sim b$.

$\varphi^{-1}(t) = \{s \in S\ | \ \varphi(s) = t\}$ é dito *imagem inversa* de $\varphi$.

**Congruência**: Se $\varphi$ é um homomorfismo, $\varphi(a) = \varphi(b) \ \Rightarrow \ a \equiv b$

**Proposição:** Se $a\equiv b$, então $a^{-1}b\in \text{nu }\varphi$, isto é, $b = an$ para algum $n\in \text{nu }\varphi$.

chama-se de *classe lateral em relação ao núcleo* o conjunto de elementos $b$ da proposição acima. Escreve-se $a \text{ nu }\varphi$.

As classes laterais $a \text{ nu }\varphi$ particionam a origem $G$ de $\varphi$ em **classes de congruência**.


**Proposição:** o homomorfismo $\varphi$ é injetivo se, e somente se, $\text{nu }\varphi = \{\vec 1\}$.
(só identidade é mapeada na identidade)

# Orbitas

**Órbita:** classe de equivalência dada pela relação
$$\text{para }a,b \in A,\ a\sim b \iff b=\sigma^n(a)$$
onde $\sigma$ é permutação de $A$.

*obs.: (demonstro que de fato é rel. de eq.)*

# Ciclos

**Ciclo**: é uma permutação que possui no máximo uma órbita contendo mais que um elemento (órbita não trivial).

*Comprimento* de um ciclo é o número de elementos de sua maior órbita.

**Exemplo**
$$
\begin{pmatrix}
    1 & 2 & 3 & 4 & 5 & 6 & 7 & 8\\
    \downarrow & \downarrow & \downarrow & \downarrow & \downarrow & \downarrow & \downarrow & \downarrow\\
    3 & 2 & 6 & 4 & 5 & 1 & 7 & 8
\end{pmatrix}
$$

**Notação de ciclos**: $\mu = (1,3,6)$

**Produto de ciclos:** 

$$
\sigma = 
\begin{pmatrix}
    1 & 2 & 3 & 4 & 5 & 6 & 7 & 8\\
    \downarrow & \downarrow & \downarrow & \downarrow & \downarrow & \downarrow & \downarrow & \downarrow\\
    3 & 8 & 6 & 7 & 4 & 1 & 5 & 2
\end{pmatrix}
= (1,3,6)(2,8)(4,7,5).
$$

**Proposição**: Toda permutação de um conjunto finito é um produto de ciclos disjuntos.

**Transposição:** Ciclo de comprimento 2.

**Corolário:** Qualquer permutação de um conjunto finito ($\geq$ 2 elementos) pode ser escrito como produto de transposições.

**Permutações pares e impares**, quantidade de transposições.

**Proposição**: uma permutação em $S_n$ é par, ou (exclusivo) é impar.

*obs: $S_n$ é um grupo simétrico sobre $n$ símbolos, isto é, todas as $n!$ permutações de um conjunto de $n$ símbolos. Teorema de cayley afirma que todo grupo finito $G$ é isomorfo a um grupo de permutações, isso é, um subgrupo de $S_n$ com $n=|G|$*

**Proposição**: todas as permutações impares (ou pares) de $S_n, n\geq 2$ formam um subgrupo de $S_n$ de ordem $\frac{n!}{2}$. 

**Grupo alternado**: é o subgrupo de $S_n$ formado por suas permutações ímpares.

*obs: parece que o fato de não existirem soluções por radicais para polinomios de grau $\geq 5$ se deve pela estrutura de $A_n$. O jhon jurou.*

# Classe lateral

**Classe lateral a esquerda:** é o subconjunto 
$$aH = \{ah \ |\  h \in H\},$$ 
$H\leq G$.

**Proposição**: A classe lateral a esquerda induz a relação de congruência
$$b = ah \Rightarrow a \equiv b, \text{para algum } h,$$
que particiona o grupo $G$ em classes de equivalência.

**Índice de um subgrupo:** é a quantidade de classes laterais a esquerda de um subgrupo $H$ em um grupo $G$. Escreve-se $[G:H]$

**Proposição:** $|G| = |H|[G:H]$.

*obs: $H$ possui a mesma cardinalidade de $aH$ (há uma bijeção), então, as classes laterias de $H$ particionam $G$ em partes de mesma ordem.*

**Teorema de Lagrange:** Seja $G$ um grupo finito e $H$ um subgrupo de $G$. A ordem de $H$ divide a ordem de $G$.

**Ordem de um elemento**: é a ordem de um grupo cíclico gerado pelo elemento. ($\{\dots,e^{-1},\vec 1,e, e^2,\dots\}$).

**Proposição**: Seja um grupo com $p$ elementos tal que $p$ é primo. Então, esse é um grupo cíclico $\{1,a,\dots,a^{p-1}\}$ gerado por $a\neq \vec 1$.

**Proposição:** Seja $\varphi: G\longrightarrow G'$ um homomorfismo onde $G$ e $G'$ são finitos. Então
$$|G| = |\text{ nu }\varphi\ |\cdot|\text{ im }\varphi\ |.$$

*obs: como as classes laterais a esquerda do núcleo são as imagens inversas, existe uma bijeção delas com a imagem. Daí, $[G:\text{nu }\varphi\ ] = |\ \text{im }\varphi\ |$. Isso é, o número das classes laterais a esquerda do núcleo é o mesmo da cardinalidade da imagem.*

**Classes laterais a direita:** são os conjuntos da forma
$$Ha = \{ha \ | \ h \in H\}$$

Também induzem uma relação de congruência, agora a direita, que particionam $G$ em classes de equivalência.

$$b = ha \implies a\equiv b.$$

**Proposição**: $H\trianglelefteq G \iff aH = Ha, \forall a \in G.$
