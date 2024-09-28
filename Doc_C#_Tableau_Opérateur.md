

## **1. Opérateurs arithmétiques**
Ces opérateurs sont utilisés pour effectuer des opérations mathématiques.

| Opérateur | Description                   | Exemple          |
|-----------|-------------------------------|------------------|
| `+`       | Additionne deux opérandes      | `a + b`          |
| `-`       | Soustrait le deuxième opérande | `a - b`          |
| `*`       | Multiplie deux opérandes       | `a * b`          |
| `/`       | Divise le premier opérande par le second | `a / b`    |
| `%`       | Renvoie le reste d’une division (modulo) | `a % b`    |
| `++`      | Incrémente de 1 l'opérande     | `a++` ou `++a`   |
| `--`      | Décrémente de 1 l'opérande     | `a--` ou `--a`   |

---

## **2. Opérateurs de comparaison**
Ces opérateurs comparent deux valeurs et renvoient un booléen (`true` ou `false`).

| Opérateur | Description                            | Exemple        |
|-----------|----------------------------------------|----------------|
| `==`      | Égalité                               | `a == b`       |
| `!=`      | Différence                            | `a != b`       |
| `>`       | Supérieur à                           | `a > b`        |
| `<`       | Inférieur à                           | `a < b`        |
| `>=`      | Supérieur ou égal à                   | `a >= b`       |
| `<=`      | Inférieur ou égal à                   | `a <= b`       |

---

## **3. Opérateurs logiques**
Utilisés pour effectuer des opérations logiques sur des booléens.

| Opérateur | Description                            | Exemple              |
|-----------|----------------------------------------|----------------------|
| `&&`      | ET logique (AND)                       | `a && b` (vrai si les deux sont vrais) |
| `||`      | OU logique (OR)                        | `a || b` (vrai si l'un ou l'autre est vrai) |
| `!`       | NON logique (NOT)                      | `!a` (inverse la valeur de `a`) |

---

## **4. Opérateurs d'affectation**
Ces opérateurs assignent des valeurs aux variables.

| Opérateur | Description                            | Exemple         |
|-----------|----------------------------------------|-----------------|
| `=`       | Affecte la valeur de droite à la gauche | `a = b`         |
| `+=`      | Ajoute et affecte                      | `a += b` (équivaut à `a = a + b`) |
| `-=`      | Soustrait et affecte                   | `a -= b` (équivaut à `a = a - b`) |
| `*=`      | Multiplie et affecte                   | `a *= b`        |
| `/=`      | Divise et affecte                      | `a /= b`        |
| `%=`      | Modulo et affecte                      | `a %= b`        |

---

## **5. Opérateurs bit à bit**
Ces opérateurs manipulent les bits des opérandes.

| Opérateur | Description                                     | Exemple         |
|-----------|-------------------------------------------------|-----------------|
| `&`       | ET bit à bit                                    | `a & b`         |
| `|`       | OU bit à bit                                    | `a | b`         |
| `^`       | OU exclusif bit à bit (XOR)                     | `a ^ b`         |
| `~`       | NON bit à bit (complément)                      | `~a`            |
| `<<`      | Décalage à gauche                               | `a << b`        |
| `>>`      | Décalage à droite                               | `a >> b`        |

---

## **6. Opérateurs ternaires**
Utilisé pour simplifier les expressions conditionnelles.

| Opérateur | Description                           | Exemple                                      |
|-----------|---------------------------------------|----------------------------------------------|
| `?:`      | Opérateur conditionnel (ternaire)     | `condition ? valeur_si_vrai : valeur_si_faux`|

---

## **7. Opérateurs de type**
Utilisés pour effectuer des vérifications ou conversions de types.

| Opérateur  | Description                            | Exemple        |
|------------|----------------------------------------|----------------|
| `is`       | Vérifie si un objet est d'un type donné | `a is string`  |
| `as`       | Conversion de type sécurisé            | `a as string`  |
| `typeof`   | Renvoie le type d'une classe ou d'une valeur | `typeof(int)` |
| `sizeof`   | Renvoie la taille d’un type en octets   | `sizeof(int)`  |

---

## **8. Opérateurs de nullité**
Ces opérateurs sont utilisés pour gérer les valeurs null.

| Opérateur    | Description                                      | Exemple                  |
|--------------|--------------------------------------------------|--------------------------|
| `??`         | Opérateur de coalescence de null                 | `a ?? b` (renvoie `a` si non nul, sinon `b`) |
| `??=`        | Affectation avec coalescence de null             | `a ??= b` (assigne `b` à `a` si `a` est null) |

---

## **9. Opérateurs d'accès**
Ces opérateurs permettent d'accéder à des membres ou des éléments d'un type.

| Opérateur  | Description                            | Exemple        |
|------------|----------------------------------------|----------------|
| `.`        | Accès aux membres d’un type            | `obj.method()` |
| `[]`       | Accès aux éléments d’un tableau/liste  | `array[0]`     |
| `->`       | Accès à un membre via un pointeur      | `ptr->field`   |
| `?`        | Accès conditionnel (null safe)         | `obj?.method()`|

---

Avec ces opérateurs, vous pouvez manipuler les données et contrôler le flux d'exécution dans vos programmes C#.