### 1. **Namespace**
Le **namespace** est utilisé pour organiser et regrouper des classes, interfaces et méthodes. Il empêche les conflits entre noms similaires dans différents projets.

```csharp
namespace MonProjet
{
    // Code du projet ici
}
```

### 2. **Classes**
Les classes sont les blocs de construction principaux en C#. Elles définissent des objets qui contiennent des champs, des propriétés et des méthodes.

```csharp
public class MaClasse
{
    // Champs, méthodes, propriétés
}
```

### 3. **Méthode Main**
La méthode `Main` est le point d'entrée de tout programme C#. C'est ici que l'exécution du programme commence.

```csharp
class Program
{
    static void Main(string[] args)
    {
        // Code à exécuter
    }
}
```

### 4. **Variables**
Les **variables** stockent des données. Elles sont déclarées avec un type, comme `int`, `string`, etc.

```csharp
int age = 25;
string nom = "Jean";
```

### 5. **Conditions**
Les conditions permettent d'exécuter du code en fonction d'une condition donnée.

```csharp
if (age > 18)
{
    Console.WriteLine("Vous êtes majeur.");
}
else
{
    Console.WriteLine("Vous êtes mineur.");
}
```

### 6. **Boucles**
Voici une explication des différentes boucles en C# : **for**, **while** et **do-while**.

---

## **1. La boucle `for`**

### **Principe :**
La boucle `for` est utilisée lorsque vous savez à l'avance combien de fois vous souhaitez exécuter un bloc de code. Elle est particulièrement adaptée aux situations où vous devez incrémenter ou décrémenter un compteur de façon prédéfinie.

### **Syntaxe :**
```csharp
for (initialisation; condition; incrémentation/décrémentation)
{
    // Bloc de code à exécuter
}
```

### **Explication :**
- **initialisation** : Vous initialisez une variable de contrôle (généralement un compteur).
- **condition** : Tant que la condition est vraie, la boucle continue de s’exécuter.
- **incrémentation/décrémentation** : Modifie la variable de contrôle après chaque itération.

### **Exemple :**
```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine("i vaut : " + i);
}
```

### **Explication de l'exemple :**
- La boucle commence avec `i = 0`.
- Elle s'exécute tant que `i` est inférieur à 5.
- À chaque itération, `i` est incrémenté de 1 (grâce à `i++`).
- Elle va donc afficher `0, 1, 2, 3, 4` avant de s'arrêter.

---

## **2. La boucle `while`**

### **Principe :**
La boucle `while` est utilisée lorsqu’on ne sait pas exactement combien de fois la boucle doit être exécutée à l'avance. Elle continue de s'exécuter tant qu'une condition est vraie.

### **Syntaxe :**
```csharp
while (condition)
{
    // Bloc de code à exécuter
}
```

### **Explication :**
- **condition** : Tant que la condition est vraie, la boucle s'exécute.
- Si la condition est fausse au début, la boucle ne sera jamais exécutée.

### **Exemple :**
```csharp
int i = 0;
while (i < 5)
{
    Console.WriteLine("i vaut : " + i);
    i++;  // Incrémente i pour éviter une boucle infinie
}
```

### **Explication de l'exemple :**
- `i` commence à 0.
- La boucle continue tant que `i` est inférieur à 5.
- `i` est incrémenté à chaque itération, donc la boucle s'arrête lorsque `i` atteint 5.

---

## **3. La boucle `do-while`**

### **Principe :**
La boucle `do-while` est similaire à la boucle `while`, mais avec une différence majeure : elle garantit que le bloc de code est exécuté **au moins une fois**, même si la condition est fausse dès le départ.

### **Syntaxe :**
```csharp
do
{
    // Bloc de code à exécuter
} while (condition);
```

### **Explication :**
- Le bloc de code est exécuté une fois avant que la condition ne soit vérifiée.
- Ensuite, tant que la condition est vraie, la boucle continue de s'exécuter.

### **Exemple :**
```csharp
int i = 0;
do
{
    Console.WriteLine("i vaut : " + i);
    i++;
} while (i < 5);
```

### **Explication de l'exemple :**
- Ici, la boucle commence à exécuter le code même si la condition est évaluée **après** la première itération.
- `i` commence à 0 et la boucle continue tant que `i` est inférieur à 5.
- La boucle affichera `0, 1, 2, 3, 4`.

---

### **Différences entre les trois boucles :**

| Boucle     | Utilisation principale                                | Exécution garantie au moins une fois |
|------------|-------------------------------------------------------|--------------------------------------|
| `for`      | Lorsque vous savez à l'avance combien de fois itérer   | Non                                 |
| `while`    | Lorsque vous ne savez pas combien de fois itérer, mais que vous avez une condition préalable | Non                                 |
| `do-while` | Similaire à `while`, mais vous voulez toujours exécuter le bloc au moins une fois | Oui                                 |

---

### **Quand utiliser quelle boucle ?**
- **Utilisez `for`** : lorsque vous avez un nombre d'itérations connu à l'avance, par exemple parcourir un tableau ou répéter un nombre fixe de fois.
- **Utilisez `while`** : lorsque vous avez une condition qui doit être vraie pour continuer à exécuter la boucle, mais que vous ne savez pas combien de fois la boucle doit s'exécuter.
- **Utilisez `do-while`** : lorsque vous devez vous assurer que le bloc de code est exécuté au moins une fois, quelle que soit la condition initiale.


-------------------------------------


### 7. **Méthodes**
Les méthodes sont des blocs de code qui exécutent une action spécifique et qui peuvent être réutilisés.

```csharp
public void AfficherMessage()
{
    Console.WriteLine("Bonjour !");
}
```

Pour appeler la méthode dans la classe principale :

```csharp
AfficherMessage();
```

### 8. **Gestion des Entrées/Sorties**
En C#, vous pouvez lire des données de l'utilisateur avec `Console.ReadLine()` et afficher des données avec `Console.WriteLine()`.

```csharp
Console.WriteLine("Entrez votre nom : ");
string nomUtilisateur = Console.ReadLine();
Console.WriteLine("Bonjour, " + nomUtilisateur);
```

### 9. **Commentaires**
Les commentaires permettent de documenter le code et ne sont pas exécutés.

- **Commentaire sur une ligne** : `// Mon commentaire`
- **Commentaire sur plusieurs lignes** :
  ```csharp
  /* 
   Ceci est un commentaire
   sur plusieurs lignes
  */
  ```

### 10. **Imports**
Les **importations** sont des références à d'autres bibliothèques qui ajoutent des fonctionnalités supplémentaires. Elles se placent en haut du fichier.

```csharp
using System;
```

### Exemple Complet

Voici un exemple complet qui utilise plusieurs des concepts abordés :

```csharp
using System;

namespace MonProjet
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Entrez votre âge :");
            int age = int.Parse(Console.ReadLine());

            if (age >= 18)
            {
                Console.WriteLine("Vous êtes majeur.");
            }
            else
            {
                Console.WriteLine("Vous êtes mineur.");
            }

            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine("Tour : " + i);
            }
        }
    }
}
```
Je vais t'expliquer comment rajouter les concepts de **portée des variables** et de **bloc de code** dans un exemple de code en C#.

### 11. **Portée des variables**
La portée d'une variable en C# fait référence à la partie du programme où cette variable peut être utilisée. Il existe plusieurs types de portée :
- **Portée locale** : Une variable définie à l'intérieur d'un bloc de code (comme dans une méthode) ne peut être utilisée qu'à l'intérieur de ce bloc.
- **Portée globale** (ou membre) : Une variable déclarée au niveau de la classe peut être utilisée dans toutes les méthodes de la classe.

### 12. **Bloc de code**
Un bloc de code en C# est défini par des accolades `{}`. Il peut encapsuler un ensemble d'instructions, et ce bloc peut être utilisé dans des structures de contrôle comme les boucles, les conditions, ou pour définir le corps d'une méthode.

Voici un exemple de code qui explique ces concepts :

```csharp
using System;

class Exemple
{
    // Variable globale ou membre de la classe (portée globale)
    // Cette variable peut être utilisée dans toutes les méthodes de cette classe
    static int variableGlobale = 10;

    static void Main(string[] args)
    {
        // Bloc de code 1 : Début de la méthode Main
        Console.WriteLine("Exemple de portée des variables et blocs de code");

        // Variable locale à la méthode Main (portée locale)
        // Elle est accessible uniquement à l'intérieur de la méthode Main
        int variableLocale = 5;

        Console.WriteLine("Variable locale : " + variableLocale);

        // Début d'un autre bloc de code (un if)
        if (variableLocale < variableGlobale)
        {
            // Bloc de code 2 : Début du bloc de condition if
            // Cette variable est locale au bloc if
            int variableDansIf = 20;
            Console.WriteLine("Variable dans le bloc if : " + variableDansIf);
            Console.WriteLine("Variable globale dans le bloc if : " + variableGlobale);

            // Fin du bloc de code 2
        }
        // Fin du bloc de code 1

        // Ici, nous ne pouvons plus utiliser la variable `variableDansIf`, car elle est définie dans le bloc `if`
        // Si on essaye de l'utiliser ici, on aura une erreur de compilation :
        // Console.WriteLine(variableDansIf); // Erreur !

        Console.WriteLine("Fin du programme.");
    }
}
```

### Explication :

1. **Portée des variables** :
   - `variableGlobale` est définie en dehors de toute méthode, elle est accessible dans toutes les méthodes de la classe.
   - `variableLocale` est définie à l'intérieur de la méthode `Main`. Elle n'est accessible que dans cette méthode.
   - `variableDansIf` est définie dans le bloc `if` et n'est accessible qu'à l'intérieur de ce bloc.

2. **Bloc de code** :
   - Un bloc de code est délimité par des accolades `{}`. Dans cet exemple, il y a plusieurs blocs :
     - Le bloc principal de la méthode `Main`.
     - Un bloc de code supplémentaire à l'intérieur de l'instruction `if`.

### Remarques importantes :
- Les variables définies dans un bloc de code (comme dans l'instruction `if`) ne sont pas accessibles en dehors de ce bloc.
- Chaque bloc de code a sa propre portée de variable.


---
