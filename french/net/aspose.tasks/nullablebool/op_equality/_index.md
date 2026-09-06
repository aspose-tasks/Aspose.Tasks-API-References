---
title: "NullableBool.op_Equality"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode NullableBool. Retourne une valeur indiquant si cette instance est égale à un objet spécifié"
type: docs
weight: 70
url: /fr/net/aspose.tasks/nullablebool/op_equality/
---
## NullableBool Equality operator

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public static bool operator ==(NullableBool a, NullableBool b)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| a | NullableBool | Le premier [`NullableBool`](../). |
| b | NullableBool | Le deuxième [`NullableBool`](../). |

### Valeur de retour

une valeur indiquant si cette instance est égale à un objet spécifié

## Exemples

Montre comment comparer les instances &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// L'égalité des booléens est vérifiée par rapport aux propriétés 'IsDefined' et 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// vérifie la conversion implicite en booléen : bool1 est True car il est défini et Value est défini sur True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// vérifie la conversion implicite en booléen : bool2 est False car il n'est pas défini.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// vérifie la conversion implicite en booléen
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Voir aussi

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


