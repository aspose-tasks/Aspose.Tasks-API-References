---
title: "Tsk.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Gerçekleştirilen işin bütçelenmiş maliyetini (BCWP) hesaplamak için Tamamlandı mı yoksa Fiziksel Tamamlandı mı alanının kullanılacağını belirler."
type: docs
weight: 350
url: /tr/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

% Complete veya Physical % Complete alanının gerçekleştirilen işin bütçelenen maliyetini (BCWP) hesaplamak için kullanılıp kullanılmayacağını belirler.

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Örnekler

Tsk.EarnedValueMethod özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


