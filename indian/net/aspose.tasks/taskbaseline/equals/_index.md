---
title: "TaskBaseline.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaseline मेथड। एक मान लौटाता है जो यह दर्शाता है कि यह इंस्टेंस निर्दिष्ट TaskBaseline ऑब्जेक्ट के बराबर है या नहीं"
type: docs
weight: 100
url: /hi/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

यह दर्शाने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट `TaskBaseline` वस्तु के बराबर है या नहीं।

```csharp
public bool Equals(TaskBaseline other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| अन्य | TaskBaseline | इस उदाहरण से तुलना करने के लिए निर्दिष्ट AssignmentBaseline वस्तु। |

### रिटर्न वैल्यू

यदि यह इंस्टेंस निर्दिष्ट TaskBaseline ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।

## उदाहरण

दिखाता है कि कैसे बेसलाइन की समानता जांचें।

```csharp
var project = new Project();

// TaskBaseline बनाना
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// टास्क बेसलाइन अवधि दिखाएँ
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// बेसलाइन की समानता को बेसलाइन के संख्याओं के विरुद्ध जाँच किया जाता है।
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### संबंधित देखें

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_2}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | इस इंस्टेंस के साथ तुलना करने के लिए वस्तु। |

### रिटर्न वैल्यू

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

## उदाहरण

दिखाता है कि कैसे बेसलाइन की समानता जांचें।

```csharp
var project = new Project();

// TaskBaseline बनाना
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// टास्क बेसलाइन अवधि दिखाएँ
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// बेसलाइन की समानता को बेसलाइन के संख्याओं के विरुद्ध जाँच किया जाता है।
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### संबंधित देखें

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


