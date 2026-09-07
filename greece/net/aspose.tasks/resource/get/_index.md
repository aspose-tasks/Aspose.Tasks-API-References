---
title: "Resource.Get"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Resource. Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο"
type: docs
weight: 830
url: /el/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Επιστρέφει την τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | ο τύπος της αντιστοιχισμένης τιμής. |
| key | το καθορισμένο κλειδί ιδιότητας. [`Rsc`](../../rsc/) για λήψη του κλειδιού ιδιότητας. |

### Τιμή Επιστροφής

η τιμή στην οποία αντιστοιχίζεται η ιδιότητα σε αυτό το δοχείο.

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε κοινές ιδιότητες πόρων.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Προσθέστε πόρο και ορίστε κάποιες ιδιότητες
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


