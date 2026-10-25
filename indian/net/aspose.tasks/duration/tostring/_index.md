---
title: "Duration.ToString"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। इस उदाहरण का स्ट्रिंग प्रतिनिधित्व लौटाता है।"
type: docs
weight: 120
url: /hi/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

इस इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है।

```csharp
public override string ToString()
```

### रिटर्न वैल्यू

इस उदाहरण का स्ट्रिंग प्रतिनिधित्व।

## उदाहरण

एक duration को स्ट्रिंग में बदलने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// कार्य की अवधि प्राप्त करें
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### संबंधित देखें

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


