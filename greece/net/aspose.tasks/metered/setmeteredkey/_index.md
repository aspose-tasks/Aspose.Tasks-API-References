---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Metered. Ορίζει τα δημόσια και ιδιωτικά κλειδιά Metered"
type: docs
weight: 40
url: /el/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ορίζει δημόσια και ιδιωτικά κλειδιά μετρητή.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| publicKey | String | Το δημόσιο κλειδί. |
| privateKey | String | Το ιδιωτικό κλειδί. |

## Παρατηρήσεις

Εάν αγοράσετε άδεια με μέτρηση, αυτό το API πρέπει να κληθεί κατά την εκκίνηση της εφαρμογής· συνήθως, αυτό είναι αρκετό. Ωστόσο, εάν η μέτρηση αποτύχει να ανεβάσει τα δεδομένα κατανάλωσης εντός περιόδου 24 ωρών, η άδεια θα οριστεί σε κατάσταση αξιολόγησης. Για να αποφύγετε αυτή την περίπτωση, θα πρέπει να ελέγχετε τακτικά την κατάσταση της άδειας. Εάν είναι σε κατάσταση αξιολόγησης, καλέστε ξανά αυτό το API.

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


