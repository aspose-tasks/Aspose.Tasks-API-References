---
title: "LevelingDelayFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Bir gecikmenin süresini ifade etme biçimi."
type: docs
weight: 790
url: /tr/net/aspose.tasks/tsk/levelingdelayformat/
---
## Tsk.LevelingDelayFormat field

Bir gecikmenin süresini ifade etme biçimi.

```csharp
public static readonly Key<TimeUnitType, TaskKey> LevelingDelayFormat;
```

### Örnekler

Tsk.LevelingDelayFormat özelliğinin nasıl okunup yazıldığını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelayFormat, TimeUnitType.Hour);

Console.WriteLine("Leveling Delay Format: " + task.Get(Tsk.LevelingDelayFormat));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [TaskKey](../../taskkey)
* class [Tsk](../../tsk)
* namespace [Aspose.Tasks](../../tsk)
* assembly [Aspose.Tasks](../../../)

<!-- DÜZENLEMEYİN: xmldocmd tarafından Aspose.Tasks.dll için oluşturuldu -->
