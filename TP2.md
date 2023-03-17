``` java
 public class Calculator {
    private double result;
    
    public void add(double num) {
        result += num;
    }
    
    public void subtract(double num) {
        result -= num;
    }
    
    public void multiply(double num) {
        result *= num;
    }
    
    public void divide(double num) {
        if (num != 0) {
            result /= num;
        }
    }
    
    public double getResult() {
        return result;
    }
}
```

Dans cet exemple, la classe Calculatrice n'a qu'une seule responsabilité : effectuer des opérations arithmétiques de base. Les méthodes et les attributs de la classe sont étroitement liés et servent un objectif unique, ce qui se traduit par une valeur TCC élevée. La classe n'est pas non plus étroitement liée à d'autres classes du système, puisqu'elle peut fonctionner de manière indépendante, ce qui se traduit par une valeur LCC égale. Par conséquent, cette classe a des valeurs LCC et TCC égales.





Oui, il est possible qu'une classe ait un LCC inférieur au TCC. Cela peut se produire lorsqu'une classe présente un degré élevé de cohésion interne (c'est-à-dire une valeur TCC élevée), mais qu'elle est étroitement liée à d'autres classes du système, ce qui se traduit par une valeur LCC inférieure.

Prenons l'exemple d'une classe qui gère une connexion à une base de données et qui comprend des méthodes permettant d'établir une connexion, d'exécuter des requêtes et de fermer la connexion. Les méthodes de cette classe sont étroitement liées et servent un objectif unique, ce qui se traduit par une valeur élevée de TCC. Cependant, cette classe est également étroitement liée à d'autres classes du système, telles que les classes qui définissent le schéma de la base de données ou effectuent l'analyse des données, ce qui se traduit par une valeur LCC plus faible.

Dans ce scénario, la classe présente un degré élevé de cohésion interne mais est étroitement liée à d'autres classes du système, ce qui se traduit par une valeur LCC inférieure à la valeur TCC.

