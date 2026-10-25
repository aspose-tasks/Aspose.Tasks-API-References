---
title: "AssignmentBaseline.Finish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AssignmentBaseline प्रॉपर्टी। निर्धारित समाप्ति तिथि प्राप्त या सेट करता है जब बेसलाइन सहेजा गया था। यह बेसलाइन सहेजे जाने पर संसाधन असाइनमेंट की समाप्ति तिथि है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/assignmentbaseline/finish/
---
## AssignmentBaseline.Finish property

जब बेसलाइन सहेजी गई थी तो संसाधन असाइनमेंट की निर्धारित समाप्ति तिथि प्राप्त करता है या सेट करता है। जब यह बेसलाइन सहेजी गई थी तो संसाधन असाइनमेंट की समाप्ति तिथि।

```csharp
public DateTime? Finish { get; set; }
```

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

* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


