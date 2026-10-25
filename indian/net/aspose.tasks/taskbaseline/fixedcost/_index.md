---
title: "TaskBaseline.FixedCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaseline प्रॉपर्टी। मान प्राप्त करता है या सेट करता है जो टास्क की स्थिर लागत को दर्शाता है जब बेसलाइन सहेजी गई थी"
type: docs
weight: 50
url: /hi/net/aspose.tasks/taskbaseline/fixedcost/
---
## TaskBaseline.FixedCost property

जब बेसलाइन सहेजी गई थी, तब कार्य की निश्चित लागत को प्राप्त करता है या सेट करता है।

```csharp
public double FixedCost { get; set; }
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

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


