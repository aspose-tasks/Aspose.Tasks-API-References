---
title: "TaskBaseline.CompareTo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaseline मेथड। IComparable इंटरफ़ेस इम्प्लीमेंटेशन। इस इंस्टेंस की तुलना निर्दिष्ट Baseline ऑब्जेक्ट से करता है"
type: docs
weight: 90
url: /hi/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

IComparable इंटरफ़ेस कार्यान्वयन। इस इंस्टेंस की तुलना निर्दिष्ट Baseline ऑब्जेक्ट से करता है।

```csharp
public int CompareTo(TaskBaseline other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| अन्य | TaskBaseline | निर्दिष्ट Baseline ऑब्जेक्ट जिससे इस इंस्टेंस की तुलना की जानी है। |

### रिटर्न वैल्यू

यदि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है तो -1 लौटाता है, यदि बड़ा है तो 1 लौटाता है; अन्यथा 0 लौटाता है।

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


