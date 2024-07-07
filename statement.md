# Welcome!

Test : tri et fusion de collections d'objet

```C# runnable
// { autofold
using System;

class Pays {

    Pays(int nbHabitant, decimal surface, decimal pib){
        NbHabitant = nbHabitant;
        Surface = surface;
        Pib = pib;
    }

    public int NbHabitant;
    public decimal Surface;
    public decimal Pib;
}

class Hello 
{
    static void Main() 
    {
        var pays = new List<Pays>() {
            new Pays()
        }
// }

Console.WriteLine("Hello World!");

// { autofold
    }
}
// }
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced C# template](https://tech.io/select-repo/386)
