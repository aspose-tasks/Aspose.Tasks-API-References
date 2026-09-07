---
title: "Rsc.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική εργασία."
type: docs
weight: 80
url: /el/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

Το ποσό εργασίας μέσω του οποίου προστατεύεται η πραγματική εργασία.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


