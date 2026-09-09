---
title: "Asn.LinkedFields"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Projenin başka bir OLE nesnesine bağlı olup olmadığını belirler."
type: docs
weight: 320
url: /tr/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

Projenin başka bir OLE nesnesine bağlı olup olmadığını belirler.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## Örnekler

Asn.LinkedFields özelliğini nasıl okuyacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


