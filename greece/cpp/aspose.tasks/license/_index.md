---
title: "Aspose::Tasks::License κλάση"
linktitle: "Άδεια"
articleTitle: "Άδεια"
second_title: "Aspose.Tasks για C++"
description: "Παρέχει μεθόδους για την αδειοδότηση του στοιχείου."
type: docs
weight: 10
url: /el/cpp/aspose.tasks/license/
---

## License class

Παρέχει μεθόδους για την αδειοδότηση του στοιχείου.

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να βρεθεί ένα αρχείο άδειας με όνομα MyLicense.lic στον φάκελο που περιέχει <ms> το στοιχείο, στον φάκελο που περιέχει το assembly που καλεί, στον φάκελο του entry assembly και, τέλος, στους ενσωματωμένους πόρους του assembly που καλεί.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> το αρχείο jar του στοιχείου:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [License](./license/) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης Άδεια. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Παρέχει άδεια στο component. |

