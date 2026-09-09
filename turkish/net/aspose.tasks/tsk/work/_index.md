---
title: "Tsk.Work"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Atanan tüm kaynaklar için bir görevde planlanan toplam süre"
type: docs
weight: 1150
url: /tr/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

Atanan tüm kaynaklar için bir görevde planlanan toplam süre.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Örnekler

Tsk.Work özelliğini nasıl okuyup/yazacağınızı gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


