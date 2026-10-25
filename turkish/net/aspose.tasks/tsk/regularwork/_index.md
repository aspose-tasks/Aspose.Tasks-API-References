---
title: "Tsk.RegularWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kaynaklar tarafından gerçekleştirilecek planlanan fazla mesai dışı toplam iş miktarı"
type: docs
weight: 940
url: /tr/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

Kaynaklar tarafından yapılması planlanan toplam fazla mesai dışı iş miktarı.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Örnekler

Tsk.RegularWork özelliğini nasıl okuyup/yazacağınızı gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


