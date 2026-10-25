---
title: "NullableBool.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος NullableBool. Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με την καθορισμένη παρουσία της κλάσης NullableBool."
type: docs
weight: 40
url: /el/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με την καθορισμένη παρουσία της κλάσης [`NullableBool`](../).

```csharp
public bool Equals(NullableBool other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | NullableBool | το καθορισμένο αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με την καθορισμένη παρουσία της κλάσης [`NullableBool`](../).

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

---

## Equals(object) {#equals_1}

Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | το καθορισμένο αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο.

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


