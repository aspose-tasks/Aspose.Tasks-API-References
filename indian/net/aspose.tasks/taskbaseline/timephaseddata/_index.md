---
title: "TaskBaseline.TimephasedData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaseline प्रॉपर्टी। इस ऑब्जेक्ट के लिए एक TimephasedDataCollection इंस्टेंस प्राप्त करता है या सेट करता है। टास्क बेसलाइन से जुड़ा समय‑फ़ेज़्ड डेटा"
type: docs
weight: 80
url: /hi/net/aspose.tasks/taskbaseline/timephaseddata/
---
## TaskBaseline.TimephasedData property

इस वस्तु के लिए एक `TimephasedDataCollection` उदाहरण प्राप्त करता है या सेट करता है। कार्य बेसलाइन से संबंधित समय-फ़ेज़्ड डेटा।

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## उदाहरण

बेसलाइन जानकारी तक पहुँच कैसे प्राप्त करें, यह दर्शाता है।

```csharp
var project = new Project();

// `TaskBaseline` बनाना
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// कार्य बेसलाइन अवधि प्रदर्शित करें
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// यह एक अंतरिम बेसलाइन है या नहीं, यह दर्शाने वाला मान
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// कार्य बेसलाइन का समय-फ़ेज़्ड डेटा प्रिंट करें
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### संबंधित देखें

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


