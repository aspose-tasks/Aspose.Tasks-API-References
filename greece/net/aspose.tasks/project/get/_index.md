---
title: "Project.Get"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Επιστρέφει την τιμή στην οποία η ιδιότητα αντιστοιχεί σε αυτό το container"
type: docs
weight: 1080
url: /el/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | ο τύπος της αντιστοιχισμένης τιμής. |
| key | το καθορισμένο κλειδί ιδιότητας. [`Prj`](../../prj/) για λήψη του κλειδιού ιδιότητας. |

### Τιμή Επιστροφής

η τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

## Παραδείγματα

Δείχνει πώς να ελέγξετε μια έκδοση του project.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Εμφάνιση έκδοσης έργου
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


