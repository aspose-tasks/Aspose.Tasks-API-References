---
title: "Asn.FixedMaterial"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Atanan bir malzeme kaynağının tüketiminin tek bir sabit miktarda gerçekleşip gerçekleşmediğini belirler"
type: docs
weight: 260
url: /tr/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Atanan bir malzeme kaynağının tüketiminin tek, sabit bir miktarda gerçekleşip gerçekleşmediğini belirler.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Örnekler

Asn.FixedMaterial özelliğini nasıl okuyup yazacağınızı gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


