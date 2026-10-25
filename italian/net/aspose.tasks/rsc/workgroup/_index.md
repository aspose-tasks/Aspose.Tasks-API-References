---
title: "Rsc.Workgroup"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il tipo di gruppo di lavoro a cui appartiene una risorsa"
type: docs
weight: 700
url: /it/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

Il tipo di gruppo di lavoro a cui appartiene una risorsa.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Workgroup.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


