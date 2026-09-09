---
title: "Tsk.ActivityId"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk field. Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı olan activity id alanını temsil eder. yalnızca Primavera projeleri için geçerlidir"
type: docs
weight: 10
url: /tr/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Aktivite kimliği alanını temsil eder - Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı. (yalnızca Primavera projeleri için geçerlidir).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Örnekler

Primavera projelerine özgü ActivityId alanı ile nasıl çalışılacağını gösterir

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Primavera kaydetme seçeneklerini oluşturun ve ActivityIds'in kaydetme sırasında üzerine yazılmamasını belirtin.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


