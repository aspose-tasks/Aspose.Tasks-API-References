---
title: "Tsk.LevelingCanSplit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kaynak dengeleme işlevinin bu görevde kalan iş üzerinde bölünmelere neden olup olmayacağını belirler"
type: docs
weight: 760
url: /tr/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Kaynak dengeleme işlevinin bu görevdeki kalan işi bölümlere ayırıp ayırmayacağını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Örnekler

Tsk.LevelingCanSplit özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


