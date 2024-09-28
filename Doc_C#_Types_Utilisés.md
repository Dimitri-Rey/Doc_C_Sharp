
# Explication des Types Utilisés dans le Programme

## 1. `int` (entier)

- **Définition** :  
  Le type `int` (abréviation d'**integer**) représente un nombre entier, c'est-à-dire un nombre sans décimale. Il peut être positif, négatif ou zéro.

- **Exemples de valeurs valides** :  
  - `int a = 5;`  // Un nombre entier positif.  
  - `int b = -3;` // Un nombre entier négatif.  
  - `int c = 0;`  // Le zéro est également un entier valide.

- **Plage de valeurs** :  
  De `-2 147 483 648` à `2 147 483 647`.

- **Utilisation** :  
  Utilisé pour stocker des valeurs numériques discrètes, comme des comptages, des choix de menu ou des indices.

```csharp
int choix = 1;
```

---

## 2. `double` (nombre à virgule flottante double précision)

- **Définition** :  
  Le type `double` représente un nombre réel, c'est-à-dire un nombre qui peut avoir une partie décimale. Il permet de travailler avec des valeurs plus précises que `int` et est utilisé lorsque des nombres avec des fractions sont nécessaires.

- **Exemples de valeurs valides** :  
  - `double x = 5.12;` // Un nombre réel positif.  
  - `double y = -0.75;` // Un nombre réel négatif.  
  - `double z = 0.0;`   // Le zéro avec une précision décimale.

- **Plage de valeurs** :  
  De `±5.0 × 10^−324` à `±1.7 × 10^308`, avec une précision d'environ 15 à 16 chiffres significatifs.

- **Utilisation** :  
  Il est utilisé pour des calculs nécessitant des valeurs décimales, comme les calculs financiers (ex. : montant HT/TTC, taux de TVA).

```csharp
double montantHT = 100.50;
```

---

## 3. `bool` (booléen)

- **Définition** :  
  Le type `bool` est utilisé pour stocker une valeur logique, qui peut être soit `true` (vrai), soit `false` (faux). Il est souvent utilisé pour contrôler des conditions et des boucles.

- **Exemples de valeurs valides** :  
  - `bool isActive = true;` // Variable booléenne initialisée à vrai.  
  - `bool isComplete = false;` // Variable booléenne initialisée à faux.

- **Plage de valeurs** :  
  Seulement `true` ou `false`.

- **Utilisation** :  
  On l'utilise pour des conditions ou des décisions, par exemple pour vérifier si un choix utilisateur est valide ou pour savoir si une boucle doit continuer.

```csharp
bool continuer = true;
```

---

## 4. `string` (chaîne de caractères)

- **Définition** :  
  Le type `string` représente une chaîne de caractères, c'est-à-dire une séquence de caractères Unicode. Il est utilisé pour stocker du texte.

- **Exemples de valeurs valides** :  
  - `string nom = "Jean";` // Une chaîne de caractères contenant du texte.  
  - `string phrase = "Bonjour, comment ça va ?";` // Une phrase complète.  
  - `string vide = "";` // Une chaîne de caractères vide est également valide.

- **Plage de valeurs** :  
  Il n'y a pas de longueur maximale spécifique dans la plupart des cas, mais la taille de la mémoire disponible peut limiter la longueur.

- **Utilisation** :  
  Utilisé pour stocker des informations textuelles, comme des messages à afficher, des réponses de l'utilisateur ou des noms.

```csharp
string reponse = "O";
```

---

## 5. `char` (caractère)

- **Définition** :  
  Le type `char` représente un seul caractère Unicode. Contrairement à une `string` qui peut contenir plusieurs caractères, un `char` ne contient qu'un seul.

- **Exemples de valeurs valides** :  
  - `char lettre = 'A';` // Un seul caractère.  
  - `char symbole = '!';` // Un caractère spécial.  
  - `char chiffre = '5';` // Un chiffre peut être représenté comme un caractère.

- **Plage de valeurs** :  
  Un caractère unique peut aller de `\0` (caractère nul) à `\uFFFF` (dernier caractère Unicode).

- **Utilisation** :  
  Utilisé pour des valeurs simples de type caractère, par exemple pour analyser une seule lettre ou un symbole.

```csharp
char initiale = 'J';
```

---

## Comparaison des Types

| **Type**   | **Utilisation**                            | **Exemples de valeurs**        |
|------------|--------------------------------------------|--------------------------------|
| `int`      | Pour des nombres entiers                   | `-5`, `0`, `42`, `1500`        |
| `double`   | Pour des nombres réels avec décimales      | `3.14`, `-0.001`, `123.456`    |
| `bool`     | Pour des valeurs logiques (vrai/faux)      | `true`, `false`                |
| `string`   | Pour des chaînes de caractères (texte)     | `"Bonjour"`, `"123"`, `""`     |
| `char`     | Pour un seul caractère Unicode             | `'A'`, `'&'`, `'7'`            |

---

## Conclusion

- **`int`** : Utilisé pour manipuler des nombres entiers (sans décimale).  
- **`double`** : Utilisé pour des nombres réels (avec des décimales).  
- **`bool`** : Utilisé pour représenter des valeurs logiques (vrai ou faux).  
- **`string`** : Utilisé pour manipuler des chaînes de texte.  
- **`char`** : Utilisé pour stocker un seul caractère.

Chaque type a une utilité spécifique selon le contexte et les besoins des opérations.

