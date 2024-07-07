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
       {"Paris",105.4m},
{"Marseille",240.62m},
{"Lyon",47.87m},
{"Toulouse",118.3m},
{"Nice",71.92m},
{"Nantes",65.19m},
{"Strasbourg",78.26m},
{"Montpellier",56.88m},
{"Bordeaux",49.36m},
{"Lille",34.83m},
{"Rennes",50.39m},
{"Reims",46.9m},
{"Le Havre",46.95m},
{"Saint-Étienne",79.97m},
{"Toulon",42.84m},
{"Grenoble",18.13m},
{"Dijon",40.41m},
{"Angers",42.71m},
{"Nîmes",161.85m},
{"Villeurbanne",14.52m},
{"Le Mans",52.81m},
{"Clermont-Ferrand",42.67m},
{"Aix-en-Provence",186.08m},
{"Brest",49.51m},
{"Limoges",78.03m},
{"Tours",34.67m},
{"Amiens",49.76m},
{"Perpignan",68.07m},
{"Metz",41.94m},
{"Boulogne-Billancourt",6.17m},
{"Besançon",65.05m},
{"Orléans",27.48m},
{"Rouen",21.38m},
{"Mulhouse",22.18m},
{"Caen",25.7m},
{"Saint-Denis",8.21m},
{"Nancy",15.01m},
{"Argenteuil",17.22m},
{"Montreuil",6.21m},
{"Roubaix",13.23m},
{"Tourcoing",15.19m},
{"Dunkerque",43.89m},
{"Nanterre",12.19m},
{"Créteil",11.46m},
{"Avignon",64.91m},
{"Vitry-sur-Seine",11.67m},
{"Poitiers",42.11m},
{"Courbevoie",4.17m}




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
