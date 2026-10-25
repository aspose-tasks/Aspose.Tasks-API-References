---
title: "Class TaskBaseline"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskBaseline class. टास्क की बेसलाइन का प्रतिनिधित्व करता है"
type: docs
weight: 2370
url: /hi/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

एक कार्य की बेसलाइन का प्रतिनिधित्व करता है।

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | `TaskBaseline` वर्ग का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | बेसलाइन डेटा रिकॉर्ड की विशिष्ट संख्या प्राप्त करता है या सेट करता है। |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | एक प्रोजेक्ट के लिए संसाधन द्वारा किए गए कार्य की अब तक बजटेड लागत प्राप्त करता है या सेट करता है। |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | संसाधन के लिए निर्धारित कार्य की बजट लागत प्राप्त करता है या सेट करता है। |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | जब बेसलाइन सहेजी जाती है तो संसाधन की अनुमानित लागत प्राप्त करता है या सेट करता है। |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | जब बेसलाइन सहेजी गई थी, तब कार्य की निर्धारित अवधि को प्राप्त करता है या सेट करता है। |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | कार्य की बेसलाइन अवधि का अनुमान लगाया गया था या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | जब बेसलाइन सहेजी गई थी, तब कार्य की निर्धारित समाप्ति तिथि को प्राप्त करता है या सेट करता है। |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | जब बेसलाइन सहेजी गई थी, तब कार्य की निश्चित लागत को प्राप्त करता है या सेट करता है। |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | यह एक अंतरिम बेसलाइन है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | जब बेसलाइन सहेजी गई थी, तब कार्य की निर्धारित प्रारंभ तिथि को प्राप्त करता है या सेट करता है। |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | इस वस्तु के लिए एक `TimephasedDataCollection` उदाहरण प्राप्त करता है या सेट करता है। कार्य बेसलाइन से संबंधित समय-फ़ेज़्ड डेटा। |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | जब बेसलाइन सहेजी जाती है तो संसाधन को सौंपा गया कार्य प्राप्त करता है या सेट करता है। जब बेसलाइन सहेजी गई थी तो संसाधन को सौंपा गया कार्य की मात्रा। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable इंटरफ़ेस कार्यान्वयन। इस इंस्टेंस की तुलना निर्दिष्ट Baseline ऑब्जेक्ट से करता है। |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | IComparable इंटरफ़ेस कार्यान्वयन। इस इंस्टेंस की तुलना निर्दिष्ट Baseline ऑब्जेक्ट से करता है। |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | यह दर्शाने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट `TaskBaseline` वस्तु के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | `TaskBaseline` वर्ग के उदाहरण के लिए हैश कोड मान लौटाता है। |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


