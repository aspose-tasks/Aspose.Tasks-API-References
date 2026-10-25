---
title: "Tsk.FixedCostAccrual"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। यह निर्धारित करता है कि स्थिर लागतों को कार्य की लागत में कब और कैसे चार्ज या संचित किया जाना चाहिए"
type: docs
weight: 440
url: /hi/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

निर्धारित करता है कि स्थिर लागतों को कार्य की लागत में कैसे और कब चार्ज या संचित किया जाना चाहिए।

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## उदाहरण

दिखाता है कि Tsk.FixedCostAccrual प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


