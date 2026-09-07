---
title: "NullableBool.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος NullableBool. Επιστρέφει μια τιμή κωδικού κατακερματισμού για την παρουσία της κλάσης NullableBool."
type: docs
weight: 50
url: /el/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Επιστρέφει μια τιμή κωδικού κατακερματισμού για την παρουσία της κλάσης [`NullableBool`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη μέθοδο &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.GetHashCode.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// ο κωδικός κατακερματισμού των bool βασίζεται στις ιδιότητες 'IsDefined' και 'Value'
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### Δείτε επίσης

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


