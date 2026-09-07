---
title: "Baseline.op_Equality"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Baseline method. एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं"
type: docs
weight: 100
url: /hi/net/aspose.tasks/baseline/op_equality/
---
## Baseline Equality operator

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public static bool operator ==(Baseline a, Baseline b)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एक | Baseline | पहला बेसलाइन। |
| b | Baseline | दूसरा बेसलाइन। |

### रिटर्न वैल्यू

एक मान जो दर्शाता है कि यह उदाहरण निर्दिष्ट वस्तु के बराबर है या नहीं।

## उदाहरण

असाइनमेंट की बेसलाइन के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// जब पूरे प्रोजेक्ट पर बेसलाइन सेट की जाती है तो असाइनमेंट बेसलाइन सेट हो जाती हैं।
project.SetBaseline(BaselineType.Baseline);

// असाइनमेंट बेसलाइन जानकारी पढ़ें
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// बेसलाइन समानता जाँचें
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// बेसलाइन को 'Equals' मेथड ओवरलोड का उपयोग करके तुलना किया जा सकता है
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// या ओवरलोडेड अंकगणितीय ऑपरेशन का उपयोग करके
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// बेसलाइन हैशकोड बेसलाइन नंबर पर आधारित है
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### संबंधित देखें

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


