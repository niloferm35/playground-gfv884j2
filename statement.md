# Welcome!

Test : tri et fusion de collections d'objet

```C# runnable
// { autofold
using System;
using System.Collections.Generic.Dictionary;

class Ville 
{
    public Ville(string name, int nbHabitant, decimal surface)
    {
        NbHabitant = nbHabitant;
        Surface = surface;
        Name = name;
    }

    public int NbHabitant { get; set; }
    public decimal Surface { get; set; }
    public string Name { get; set; }

    public override string ToString()
    {
        return $"{Name} - Habitants: {NbHabitant}, Surface: {Surface} km²";
    }
}

class Hello 
{
    static void Main() 
    {
        Dictionary<string, int> villeHabitants = new Dictionary<string, int>() {
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
        {"Saint-Denis (La Réunion)",145238},
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
        {"Saint-Paul (La Réunion)",104646},
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
// }

foreach(var v in villeHabitants) {
    Console.WriteLine($"{v.key} - {v.Value}");
}

// { autofold
    }
}
// }
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced C# template](https://tech.io/select-repo/386)
