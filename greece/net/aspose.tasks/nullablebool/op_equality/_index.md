---
title: "NullableBool.op_Equality"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος NullableBool. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο"
type: docs
weight: 70
url: /el/net/aspose.tasks/nullablebool/op_equality/
---
## NullableBool Equality operator

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public static bool operator ==(NullableBool a, NullableBool b)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | NullableBool | Η πρώτη [`NullableBool`](../). |
| b | NullableBool | Η δεύτερη [`NullableBool`](../). |

### Τιμή Επιστροφής

μια τιμή που υποδεικνύει εάν αυτή η παρουσίαση είναι ίση με ένα καθορισμένο αντικείμενο

## Παραδείγματα

Δείχνει πώς να συγκρίνετε &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt; παραδείγματα.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// η ισότητα των bool ελέγχεται σε σχέση με τις ιδιότητες 'IsDefined' και 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// ελέγχει την άμεση μετατροπή σε bool: bool1 είναι True επειδή είναι ορισμένο και το Value έχει οριστεί σε True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// ελέγχει την άμεση μετατροπή σε bool: bool2 είναι False επειδή δεν είναι ορισμένο.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// ελέγχει την άμεση μετατροπή σε bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Δείτε επίσης

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


