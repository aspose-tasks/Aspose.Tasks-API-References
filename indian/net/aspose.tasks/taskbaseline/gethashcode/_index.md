---
title: "TaskBaseline.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaseline मेथड। TaskBaseline क्लास के इंस्टेंस के लिए एक हैश कोड वैल्यू लौटाता है"
type: docs
weight: 110
url: /hi/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

[`TaskBaseline`](../) क्लास के इंस्टेंस के लिए एक हैश कोड वैल्यू लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

एक टास्क बेसलाइन का हैश कोड कैसे प्राप्त करें, यह दर्शाता है।

```csharp
var project = new Project();

// TaskBaseline बनाना
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// टास्क बेसलाइन अवधि दिखाएँ
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// कैलेंडर का हैश कोड बेसलाइन नंबर के बराबर होता है
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### संबंधित देखें

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


