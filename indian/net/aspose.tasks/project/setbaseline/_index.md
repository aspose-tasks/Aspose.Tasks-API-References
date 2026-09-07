---
title: "Project.SetBaseline"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड. पूरे प्रोजेक्ट के लिए निर्दिष्ट बेसलाइन में बेसलाइन फ़ील्ड्स को सहेजता है"
type: docs
weight: 1250
url: /hi/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

पूरी परियोजना के लिए निर्दिष्ट बेसलाइन में बेसलाइन फ़ील्ड को सहेजता है।

```csharp
public void SetBaseline(BaselineType baselineType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| baselineType | BaselineType | बेसलाइन डेटा को सहेजने के लिए बेसलाइन प्रकार |

## उदाहरण

पूरे प्रोजेक्ट के लिए बेसलाइन बनाने का तरीका दिखाता है।

```csharp
var project = new Project();

// टास्क जोड़ना
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// निर्दिष्ट टास्क के लिए बेसलाइन सेट करें
project.SetBaseline(BaselineType.Baseline);
```

### संबंधित देखें

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

चयनित कार्यों के लिए निर्दिष्ट बेसलाइन में बेसलाइन फ़ील्ड को सहेजता है।

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| baselineType | BaselineType | बेसलाइन डेटा को सहेजने के लिए बेसलाइन प्रकार |
| taskCollection | IEnumerable`1 | बेसलाइन डेटा सहेजने के लिए टास्क की सूची। |

## उदाहरण

विशिष्ट टास्क के लिए सेट बेसलाइन बनाने का तरीका दिखाता है।

```csharp
var project = new Project();

// टास्क जोड़ना
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// निर्दिष्ट टास्क के लिए बेसलाइन सेट करें
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### संबंधित देखें

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


