---
title: "Κλάση License"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.License. Παρέχει μεθόδους για την αδειοδότηση του στοιχείου"
type: docs
weight: 980
url: /el/net/aspose.tasks/license/
---
## License class

Παρέχει μεθόδους για την άδεια του στοιχείου.

```csharp
public sealed class License
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [License](license/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `License`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Αδειοδοτεί το στοιχείο. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Αδειοδοτεί το στοιχείο. |

## Παραδείγματα

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να βρεθεί ένα αρχείο άδειας με όνομα MyLicense.lic στο φάκελο που περιέχει το στοιχείο, στο φάκελο που περιέχει το καλούν σύνολο, στο φάκελο του κύριου συνόλου και στη συνέχεια στους ενσωματωμένους πόρους του καλούντος συνόλου.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

το αρχείο component jar:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Δείχνει πώς να εφαρμόσετε μια άδεια του Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


