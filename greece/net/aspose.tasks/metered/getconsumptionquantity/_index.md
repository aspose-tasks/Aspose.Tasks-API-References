---
title: "Metered.GetConsumptionQuantity"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Metered. Λαμβάνει το μέγεθος του αρχείου κατανάλωσης"
type: docs
weight: 60
url: /el/net/aspose.tasks/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Λαμβάνει το μέγεθος αρχείου κατανάλωσης.

```csharp
public static decimal GetConsumptionQuantity()
```

### Τιμή Επιστροφής

Επιστρέφει τον αριθμό των καταναλωμένων byte.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε &lt;see cref="Aspose.Tasks.Metered" /&gt; τύπο άδειας με Aspose.Tasks.

```csharp
// Ας χρησιμοποιήσουμε άδεια με μέτρηση (δείτε https://purchase.aspose.com/faqs/licensing/metered)
// ορίστε άδεια με μέτρηση
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// εργαστείτε με το έργο...
// ...

// Μπορούμε να λάβουμε τα τρέχοντα credits και την κατανάλωση bytes.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // καταγραφή εξαίρεσης
}

// πρόσφατα ο χρήστης μπορεί να επαναφέρει μια μετρημένη άδεια και να σταματήσει την καταμέτρηση των bytes
metered.ResetMeteredKey();
```

### Δείτε επίσης

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


