---
title: "NullableBool.op_Implicit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode NullableBool. Convertit implicitement une instance NullableBool en une valeur booléenne. Retourne true lorsque Value est true et IsDefined est true"
type: docs
weight: 80
url: /fr/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Convertit implicitement une instance [`NullableBool`](../) en une valeur booléenne. Retourne true lorsque [`Value`](../value/) est true et [`IsDefined`](../isdefined/) est true.

```csharp
public static implicit operator bool(NullableBool val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| val | NullableBool | La valeur à convertir. |

### Valeur de retour

une valeur booléenne.

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

## implicit operator {#op_implicit}

Convertit implicitement une valeur booléenne en l'instance [`NullableBool`](../).

```csharp
public static implicit operator NullableBool(bool val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| val | Boolean | Valeur à convertir. |

### Valeur de retour

Instance [`NullableBool`](../) convertie.

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


