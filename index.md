
## Cours sur les Dérivées


# Dérivée pour les nuls 

## Tableau des formules (à apprendre par coeur)

Les formules se limitent à ceux que tu as dans ton cours (il en manque pas mal mais je l'ai mais pas psk ta pas appris).

| Type de fonction                   | f(x)                                   | f'(x)                                             | Domaine de f (en général)                             | Exemple simple                                   |
|------------------------------------|----------------------------------------|---------------------------------------------------|-------------------------------------------------------|--------------------------------------------------|
| Constante                          | k                                      | 0                                                 | ℝ                                                     | f(x) = 5  ⇒  f'(x) = 0                           |
| Identité                           | x                                      | 1                                                 | ℝ                                                     | f(x) = x  ⇒  f'(x) = 1                           |
| Puissance                          | x^n (n entier)                         | n·x^(n-1)                                         | ℝ (si n entier)                                       | f(x) = x³ ⇒ f'(x) = 3x²                          |
| Inverse                            | 1/x = x⁻¹                              | -1/x²                                             | ℝ \ {0}                                               | f(x) = 1/x ⇒ f'(x) = -1/x²                       |
| Racine carrée                      | √x = x^(1/2)                           | 1 / (2√x)                                         | x ≥ 0 (f), x > 0 pour f'                              | f(x) = √x ⇒ f'(x) = 1/(2√x)                      |
| Multiplication par une constante  | k·u(x)                                 | k·u'(x)                                           | Domaine de u                                          | f(x) = 3x² ⇒ f'(x) = 3·(2x) = 6x                 |
| Somme / différence                | u(x) ± v(x)                            | u'(x) ± v'(x)                                     | Domaine = intersec. des domaines de u et v            | f(x) = x² + x ⇒ f'(x) = 2x + 1                   |
| Produit                           | u(x)·v(x)                              | u'(x)·v(x) + u(x)·v'(x)                           | Intersec. domaines de u et v                          | f(x) = x·e^x ⇒ f'(x) = e^x + x·e^x               |
| Quotient                          | u(x)/v(x)                              | (u'v - uv') / v²                                  | Intersec. domaines de u et v, avec v(x) ≠ 0           | f(x) = x/ln(x) ⇒ f'(x) = (lnx - 1)/ln²x          |
| Inverse d’une fonction            | 1 / u(x)                               | -u'(x) / [u(x)]²                                  | Domaine de u, avec u(x) ≠ 0                           | f(x) = 1/(x²+1) ⇒ f'(x) = -2x/(x²+1)²            |


## Exercices

### Dérivée d'une somme

Donner l'expression des dérivées des fonctions définies et dérivables sur \( I \) par :

1. \( f(x) = -5x^2 + 3x - 7 \), \( I = \mathbb{R} \)
2. \( g(x) = \sqrt{x} + \dfrac{1}{x} \), \( I = ]0; +\infty[ \)
3. \( h(x) = x^3 - 3x^2 + 2x - 7 \), \( I = \mathbb{R} \)

---

## 1. \( f(x) = -5x^2 + 3x - 7 \), sur \( I = \mathbb{R} \)

On dérive **terme par terme** en utilisant :

- \( (x^n)' = n x^{n-1} \)
- \( (k \cdot u(x))' = k \cdot u'(x) \)
- La dérivée d’une **constante** est 0.

### Étapes

1. Dérivée de \(-5x^2\)  
   \[
   (-5x^2)' = -5 \cdot (x^2)' = -5 \cdot 2x = -10x
   \]

2. Dérivée de \(3x\)  
   \[
   (3x)' = 3 \cdot (x)' = 3 \cdot 1 = 3
   \]

3. Dérivée de \(-7\)  
   \[
   (-7)' = 0
   \]

4. On additionne :
   \[
   f'(x) = -10x + 3 + 0 = -10x + 3
   \]

**Résultat :**

\[
\boxed{f'(x) = -10x + 3}, \quad \boxed{I = \mathbb{R}}
\]

---

## 2. \( g(x) = \sqrt{x} + \dfrac{1}{x} \), sur \( I = ]0; +\infty[ \)

On réécrit sous forme de puissances :

- \(\sqrt{x} = x^{1/2}\)
- \(\dfrac{1}{x} = x^{-1}\)

On utilise la règle : \( (x^n)' = n x^{n-1} \).

### Étapes

1. Dérivée de \(\sqrt{x} = x^{1/2}\)  
   \[
   (\sqrt{x})' = (x^{1/2})' = \frac{1}{2} x^{1/2 - 1} = \frac{1}{2} x^{-1/2}
   \]
   \[
   \frac{1}{2} x^{-1/2} = \frac{1}{2\sqrt{x}}
   \]

2. Dérivée de \(\dfrac{1}{x} = x^{-1}\)  
   \[
   \left(\frac{1}{x}\right)' = (x^{-1})' = -1 \cdot x^{-2} = -x^{-2} = -\frac{1}{x^2}
   \]

3. On additionne :
   \[
   g'(x) = \frac{1}{2\sqrt{x}} - \frac{1}{x^2}
   \]

4. Domaine :  
   - \(\sqrt{x}\) est définie pour \(x \ge 0\)  
   - \(\dfrac{1}{x}\) est définie pour \(x \ne 0\)  
   - Intersection avec l’intervalle donné : \(x > 0\).

**Résultat :**

\[
\boxed{g'(x) = \dfrac{1}{2\sqrt{x}} - \dfrac{1}{x^2}}, \quad \boxed{I = ]0; +\infty[}
\]

---

## 3. \( h(x) = x^3 - 3x^2 + 2x - 7 \), sur \( I = \mathbb{R} \)

On dérive **terme par terme** (polynôme).

### Étapes

1. Dérivée de \(x^3\)  
   \[
   (x^3)' = 3x^2
   \]

2. Dérivée de \(-3x^2\)  
   \[
   (-3x^2)' = -3 \cdot (x^2)' = -3 \cdot 2x = -6x
   \]

3. Dérivée de \(2x\)  
   \[
   (2x)' = 2 \cdot 1 = 2
   \]

4. Dérivée de \(-7\)  
   \[
   (-7)' = 0
   \]

5. On additionne :
   \[
   h'(x) = 3x^2 - 6x + 2 + 0 = 3x^2 - 6x + 2
   \]

**Résultat :**

\[
\boxed{h'(x) = 3x^2 - 6x + 2}, \quad \boxed{I = \mathbb{R}}
\]


### Dérivées (un peu de tout)

Donner l'expression des dérivées des fonctions définies et dérivables sur \( I \) par :

1. \( f(x) = x^2 \), \( I = \mathbb{R} \)
2. \( g(x) = \sqrt{x} \), \( I = ]0; +\infty[ \)
3. \( h(x) = \dfrac{1}{x} \), \( I = \mathbb{R} \setminus \{0\} \)
4. \( i(x) = -2x + 7 \), \( I = \mathbb{R} \)
5. \( j(x) = x^{2024} \), \( I = \mathbb{R} \)

---

## 1. \( f(x) = x^2 \), sur \( I = \mathbb{R} \)

On utilise la règle :  
\[
(x^n)' = n x^{n-1}
\]

### Étapes
\[
f'(x) = (x^2)' = 2x^{2-1} = 2x
\]

**Résultat :**
\[
\boxed{f'(x) = 2x}, \quad \boxed{I = \mathbb{R}}
\]

---

## 2. \( g(x) = \sqrt{x} \), sur \( I = ]0; +\infty[ \)

On réécrit :
\[
\sqrt{x} = x^{1/2}
\]

### Étapes
\[
g'(x) = (x^{1/2})' = \frac{1}{2}x^{1/2-1} = \frac{1}{2}x^{-1/2}
= \frac{1}{2\sqrt{x}}
\]

**Résultat :**
\[
\boxed{g'(x) = \dfrac{1}{2\sqrt{x}}}, \quad \boxed{I = ]0; +\infty[}
\]

---

## 3. \( h(x) = \dfrac{1}{x} \), sur \( I = \mathbb{R} \setminus \{0\} \)

On écrit :
\[
\frac{1}{x} = x^{-1}
\]

### Étapes
\[
h'(x) = (x^{-1})' = -1 \cdot x^{-2} = -x^{-2} = -\frac{1}{x^2}
\]

**Résultat :**
\[
\boxed{h'(x) = -\dfrac{1}{x^2}}, \quad \boxed{I = \mathbb{R} \setminus \{0\}}
\]

---

## 4. \( i(x) = -2x + 7 \), sur \( I = \mathbb{R} \)

- Dérivée de \(-2x\) : \((-2x)' = -2\)
- Dérivée de \(7\) : \(7' = 0\)

### Étapes
\[
i'(x) = -2 + 0 = -2
\]

**Résultat :**
\[
\boxed{i'(x) = -2}, \quad \boxed{I = \mathbb{R}}
\]

---

## 5. \( j(x) = x^{2024} \), sur \( I = \mathbb{R} \)

On utilise encore :
\[
(x^n)' = n x^{n-1}
\]

### Étapes
\[
j'(x) = (x^{2024})' = 2024 \, x^{2023}
\]

**Résultat :**
\[
\boxed{j'(x) = 2024\,x^{2023}}, \quad \boxed{I = \mathbb{R}}
\]

### Dérivée d'un produit

Pour chacune des fonctions suivantes, on détermine :
- sur quel ensemble elle est dérivable ;
- l’expression de sa dérivée ;
- le résultat sous la forme d’un seul quotient (quand il y a un dénominateur).

Les fonctions sont :
1. \( f(x) = \dfrac{1}{x}(3x - 7) \)
2. \( g(x) = -x^2(1 - 4x) \)
3. \( h(x) = (7 - 3x)\sqrt{x} \)

---

## 1. \( f(x) = \dfrac{1}{x}(3x - 7) \)

### Domaine / Ensemble de dérivabilité

- \( \dfrac{1}{x} \) n’est pas définie en \( x = 0 \).
- \( 3x - 7 \) est définie partout.
- Donc \( f \) est définie et dérivable sur \( \mathbb{R} \setminus \{0\} \).

### Dérivée

On pose \( u(x) = 3x - 7 \), \( v(x) = x \), donc  
\[
f(x) = \frac{u(x)}{v(x)}
\]

- \( u'(x) = 3 \)
- \( v'(x) = 1 \)

Règle du quotient :
\[
f'(x) = \frac{u'v - uv'}{v^2}
       = \frac{3x - (3x - 7)}{x^2}
       = \frac{3x - 3x + 7}{x^2}
       = \frac{7}{x^2}
\]

**Résultat :**
\[
\boxed{f'(x) = \dfrac{7}{x^2}}, \quad \boxed{\text{dérivable sur } \mathbb{R} \setminus \{0\}}
\]

---

## 2. \( g(x) = -x^2(1 - 4x) \)

### Domaine / Ensemble de dérivabilité

- Produit de polynômes ⇒ définie et dérivable sur tout \( \mathbb{R} \).

\[
\boxed{\text{dérivable sur } \mathbb{R}}
\]

### Dérivée

On peut soit utiliser le produit, soit développer.

**Méthode produit :**  
\( u(x) = -x^2 \), \( v(x) = 1 - 4x \)

- \( u'(x) = -2x \)
- \( v'(x) = -4 \)

\[
g'(x) = u'v + uv'
      = (-2x)(1 - 4x) + (-x^2)(-4)
\]
\[
g'(x) = -2x + 8x^2 + 4x^2
      = -2x + 12x^2
\]

On peut écrire :
\[
\boxed{g'(x) = 12x^2 - 2x}, \quad \boxed{\text{sur } \mathbb{R}}
\]

---

## 3. \( h(x) = (7 - 3x)\sqrt{x} \)

### Domaine / Ensemble de dérivabilité

- \( \sqrt{x} \) est définie pour \( x \ge 0 \).
- Mais sa dérivée \( \dfrac{1}{2\sqrt{x}} \) n’existe pas en \( x = 0 \).
- Donc \( h \) est dérivable seulement pour \( x > 0 \).

\[
\boxed{\text{dérivable sur } ]0; +\infty[}
\]

### Dérivée

On pose \( u(x) = 7 - 3x \), \( v(x) = \sqrt{x} = x^{1/2} \).

- \( u'(x) = -3 \)
- \( v'(x) = \dfrac{1}{2\sqrt{x}} \)

Règle du produit :
\[
h'(x) = u'v + uv'
      = -3\sqrt{x} + (7 - 3x)\frac{1}{2\sqrt{x}}
\]

On met tout sur **un seul quotient** de dénominateur \(2\sqrt{x}\).

1. On réécrit \(-3\sqrt{x}\) avec ce dénominateur :
   \[
   -3\sqrt{x} = -3\sqrt{x} \cdot \frac{2\sqrt{x}}{2\sqrt{x}}
              = \frac{-6x}{2\sqrt{x}}
   \]

2. On additionne les deux fractions :
   \[
   h'(x) = \frac{-6x}{2\sqrt{x}} + \frac{7 - 3x}{2\sqrt{x}}
         = \frac{-6x + 7 - 3x}{2\sqrt{x}}
         = \frac{7 - 9x}{2\sqrt{x}}
   \]

**Résultat :**
\[
\boxed{h'(x) = \dfrac{7 - 9x}{2\sqrt{x}}}, \quad \boxed{\text{sur } ]0; +\infty[}
\]

### Dérivée d'un quotient

Donner l'expression des dérivées des fonctions définies et dérivables sur \( I \) par :

1. \( f(x) = \dfrac{-3}{x^2} \), \( I = \mathbb{R} \setminus \{0\} \)
2. \( g(x) = \dfrac{3x - 2}{x + 3} \), \( I = \mathbb{R} \setminus \{-3\} \)
3. \( h(x) = \dfrac{3(x - 1)}{4(2x - 1)} \), \( I = \mathbb{R} \setminus \left\{\dfrac12\right\} \)

On utilise la règle du quotient :  
\[
\left(\frac{u}{v}\right)' = \frac{u'v - uv'}{v^2}
\]

---

## 1. \( f(x) = \dfrac{-3}{x^2} \), \( I = \mathbb{R} \setminus \{0\} \)

### Domaine
- Le dénominateur \(x^2\) s’annule en \(x = 0\) ⇒ on exclut 0.
- Donc \(f\) est définie et dérivable sur \(\mathbb{R} \setminus \{0\}\).

### Dérivée (méthode quotient)

On pose :
- \( u(x) = -3 \Rightarrow u'(x) = 0 \)
- \( v(x) = x^2 \Rightarrow v'(x) = 2x \)

\[
f'(x) = \frac{u'v - uv'}{v^2}
      = \frac{0\cdot x^2 - (-3)\cdot 2x}{x^4}
      = \frac{6x}{x^4}
      = \frac{6}{x^3}
\]

**Résultat :**
\[
\boxed{f'(x) = \dfrac{6}{x^3}}, \quad \boxed{I = \mathbb{R} \setminus \{0\}}
\]

---

## 2. \( g(x) = \dfrac{3x - 2}{x + 3} \), \( I = \mathbb{R} \setminus \{-3\} \)

### Domaine
- Le dénominateur \(x+3\) s’annule en \(x = -3\).
- Donc \(g\) est dérivable sur \(\mathbb{R} \setminus \{-3\}\).

### Dérivée

On pose :
- \( u(x) = 3x - 2 \Rightarrow u'(x) = 3 \)
- \( v(x) = x + 3 \Rightarrow v'(x) = 1 \)

\[
g'(x) = \frac{u'v - uv'}{v^2}
      = \frac{3(x+3) - (3x-2)\cdot 1}{(x+3)^2}
\]

On développe et simplifie le numérateur :

\[
3(x+3) = 3x + 9
\]
\[
3x + 9 - (3x - 2) = 3x + 9 - 3x + 2 = 11
\]

Donc :

\[
g'(x) = \frac{11}{(x+3)^2}
\]

**Résultat :**
\[
\boxed{g'(x) = \dfrac{11}{(x+3)^2}}, \quad \boxed{I = \mathbb{R} \setminus \{-3\}}
\]

---

## 3. \( h(x) = \dfrac{3(x - 1)}{4(2x - 1)} \), \( I = \mathbb{R} \setminus \left\{\dfrac12\right\} \)

On peut sortir la constante \(\dfrac{3}{4}\) pour simplifier :

\[
h(x) = \frac{3}{4}\cdot \frac{x-1}{2x-1}
\]

### Domaine
- \(2x - 1 = 0 \Rightarrow x = \dfrac12\), point interdit.
- Donc \(h\) est dérivable sur \(\mathbb{R} \setminus \left\{\dfrac12\right\}\).

### Dérivée de \(\dfrac{x-1}{2x-1}\)

On pose :
- \( u(x) = x - 1 \Rightarrow u'(x) = 1 \)
- \( v(x) = 2x - 1 \Rightarrow v'(x) = 2 \)

\[
\left(\frac{u}{v}\right)' = \frac{u'v - uv'}{v^2}
      = \frac{1\cdot(2x-1) - (x-1)\cdot 2}{(2x-1)^2}
\]

Numérateur :

\[
2x - 1 - 2(x-1) = 2x - 1 - 2x + 2 = 1
\]

Donc :

\[
\left(\frac{x-1}{2x-1}\right)' = \frac{1}{(2x-1)^2}
\]

On remet le facteur \(\dfrac{3}{4}\) :

\[
h'(x) = \frac{3}{4} \cdot \frac{1}{(2x-1)^2}
      = \frac{3}{4(2x-1)^2}
\]

**Résultat :**
\[
\boxed{h'(x) = \dfrac{3}{4(2x-1)^2}}, \quad
\boxed{I = \mathbb{R} \setminus \left\{\dfrac12\right\}}
\]
