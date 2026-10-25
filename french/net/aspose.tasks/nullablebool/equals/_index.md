---
title: "NullableBool.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode NullableBool. Retourne un indicateur indiquant si cette instance est égale à l'instance spécifiée de la classe NullableBool"
type: docs
weight: 40
url: /fr/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

Retourne un indicateur indiquant si cette instance est égale à l'instance spécifiée de la classe [`NullableBool`](../).

```csharp
public bool Equals(NullableBool other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | NullableBool | l'objet spécifié à comparer à cette instance. |

### Valeur de retour

un indicateur indiquant si cette instance est égale à l'instance spécifiée de la classe [`NullableBool`](../).

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

---

## Equals(object) {#equals_1}

Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | l'objet spécifié à comparer à cette instance. |

### Valeur de retour

un indicateur indiquant si cette instance est égale à l'objet spécifié.

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


