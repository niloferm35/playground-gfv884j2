# Welcome!

Test : trier les ville par densite

Utiliser la classe :

```
class Ville 
{
    public Ville(string name, int nbHabitant, decimal surface, decimal densite)
    {
        NbHabitant = nbHabitant;
        Surface = surface;
        Name = name;
        Densite = densite;
    }

    public int NbHabitant { get; set; }
    public decimal Surface { get; set; }
    public string Name { get; set; }
    public decimal Densite { get; set; }

    public override string ToString()
    {
        return $"{Name} - Habitants: {NbHabitant}, Surface: {Surface} km²";
    }
}
```

```C# runnable
// { autofold
using System;
using System.Collections.Generic;

class Ville 
{
    public Ville(string name, int nbHabitant, decimal surface, decimal densite)
    {
        NbHabitant = nbHabitant;
        Surface = surface;
        Name = name;
        Densite = densite;
    }

    public int NbHabitant { get; set; }
    public decimal Surface { get; set; }
    public string Name { get; set; }
    public decimal Densite { get; set; }

    public override string ToString()
    {
        return $"{Name} - Habitants: {NbHabitant}, Surface: {Surface} km²";
    }
}

class Hello 
{
    static void Main() 
    {
        var villeHabitants = new Dictionary<string, int>() {
        {"Paris",2240621},
{"Marseille",852516},
{"Lyon",496343},
{"Toulouse",453317},
{"Nice",343629},
{"Nantes",291604},
{"Strasbourg",274394},
{"Montpellier",268456},
{"Bordeaux",241287},
{"Lille",228652},
{"Rennes",209860},
{"Reims",181893},
{"Le Havre",173142},
{"Saint-Étienne",171483},
{"Toulon",164899},
{"Grenoble",158346},
{"Dijon",152071},
{"Angers",149017},
{"Nîmes",146709},
{"Villeurbanne",146282},
{"Le Mans",143599},
{"Clermont-Ferrand",141569},
{"Aix-en-Provence",141148},
{"Brest",139676},
{"Limoges",136221},
{"Tours",134978},
{"Amiens",132727},
{"Perpignan",120489},
{"Metz",119551},
{"Boulogne-Billancourt",117126},
{"Besançon",116353},
{"Orléans",114286},
{"Rouen",111557},
{"Mulhouse",110755},
{"Caen",108365},
{"Saint-Denis",108274},
{"Nancy",105067},
{"Argenteuil",104962},
{"Montreuil",103520},
{"Roubaix",94536},
{"Tourcoing",92707},
{"Dunkerque",90995},
{"Nanterre",90722},
{"Créteil",89845},
{"Avignon",89380},
{"Vitry-sur-Seine",88102},
{"Poitiers",87646},
{"Courbevoie",86854}

        };

        var villeSuperficies = new Dictionary<string, decimal>() {
       {"Paris",105.4},
{"Marseille",240.62},
{"Lyon",47.87},
{"Toulouse",118.3},
{"Nice",71.92},
{"Nantes",65.19},
{"Strasbourg",78.26},
{"Montpellier",56.88},
{"Bordeaux",49.36},
{"Lille",34.83},
{"Rennes",50.39},
{"Reims",46.9},
{"Le Havre",46.95},
{"Saint-Étienne",79.97},
{"Toulon",42.84},
{"Grenoble",18.13},
{"Dijon",40.41},
{"Angers",42.71},
{"Nîmes",161.85},
{"Villeurbanne",14.52},
{"Le Mans",52.81},
{"Clermont-Ferrand",42.67},
{"Aix-en-Provence",186.08},
{"Brest",49.51},
{"Limoges",78.03},
{"Tours",34.67},
{"Amiens",49.76},
{"Perpignan",68.07},
{"Metz",41.94},
{"Boulogne-Billancourt",6.17},
{"Besançon",65.05},
{"Orléans",27.48},
{"Rouen",21.38},
{"Mulhouse",22.18},
{"Caen",25.7},
{"Saint-Denis",8.21},
{"Nancy",15.01},
{"Argenteuil",17.22},
{"Montreuil",6.21},
{"Roubaix",13.23},
{"Tourcoing",15.19},
{"Dunkerque",43.89},
{"Nanterre",12.19},
{"Créteil",11.46},
{"Avignon",64.91},
{"Vitry-sur-Seine",11.67},
{"Poitiers",42.11},
{"Courbevoie",4.17},



        };
// }

foreach(var v in villeHabitants) {
    Console.WriteLine($"{v.Key} - {v.Value}");
}


foreach(var v in villeSuperficies) {
    Console.WriteLine($"{v.Key} - {v.Value}");
}

// { autofold
    }
}
// }
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced C# template](https://tech.io/select-repo/386)
