---
title: "Task.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड. लौटाता है एक मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट टास्क के बराबर है या नहीं"
type: docs
weight: 1330
url: /hi/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट टास्क के बराबर है या नहीं।

```csharp
public bool Equals(Task other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| अन्य | कार्य | निर्दिष्ट टास्क जो इस इंस्टेंस से तुलना करने के लिए है। |

### रिटर्न वैल्यू

यदि निर्दिष्ट टास्क और यह इंस्टेंस समान यूनिक आईडी रखते हैं तो true लौटाता है।

## उदाहरण

दिखाता है कि टास्क के असाइनमेंट्स पर कैसे इटरेट किया जाए।

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // टास्क के असाइनमेंट प्रदर्शित करें
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | निर्दिष्ट ऑब्जेक्ट जो इस इंस्टेंस से तुलना करने के लिए है। |

### रिटर्न वैल्यू

यदि निर्दिष्ट टास्क और यह इंस्टेंस समान यूनिक आईडी रखते हैं तो true लौटाता है।

## उदाहरण

दिखाता है कि टास्क के असाइनमेंट्स पर कैसे इटरेट किया जाए।

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // टास्क के असाइनमेंट प्रदर्शित करें
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


