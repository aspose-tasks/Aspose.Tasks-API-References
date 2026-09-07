---
title: "Κλάση Metered"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Metered. Παρέχει μεθόδους για τον ορισμό του κλειδιού μετρητή"
type: docs
weight: 1020
url: /el/net/aspose.tasks/metered/
---
## Metered class

Παρέχει μεθόδους για τον ορισμό κλειδιού μετρητή.

```csharp
public class Metered
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Metered](metered/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Ελέγχει αν το προϊόν είναι επιτυχώς αδειοδοτημένο χρησιμοποιώντας άδεια Metered. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Αφαιρεί την προηγουμένως ρυθμισμένη άδεια. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Ορίζει δημόσια και ιδιωτικά κλειδιά μετρητή. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Λαμβάνει το πιστωτικό κατανάλωσης. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Λαμβάνει το μέγεθος αρχείου κατανάλωσης. |

## Παραδείγματα

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να οριστούν τα δημόσια και ιδιωτικά κλειδιά μετρητή

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

το αρχείο component jar:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


