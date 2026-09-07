---
title: "क्लास Baseline"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Baseline क्लास. एक संसाधन के बेसलाइन मानों का प्रतिनिधित्व करता है।"
type: docs
weight: 110
url: /hi/net/aspose.tasks/baseline/
---
## Baseline class

एक संसाधन के बेसलाइन मानों का प्रतिनिधित्व करता है।

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Baseline](baseline/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | बेसलाइन डेटा रिकॉर्ड की विशिष्ट संख्या प्राप्त करता है या सेट करता है। |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | एक प्रोजेक्ट के लिए संसाधन द्वारा किए गए कार्य की अब तक बजटेड लागत प्राप्त करता है या सेट करता है। |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | संसाधन के लिए निर्धारित कार्य की बजट लागत प्राप्त करता है या सेट करता है। |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | जब बेसलाइन सहेजी जाती है तो संसाधन की अनुमानित लागत प्राप्त करता है या सेट करता है। |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | जब बेसलाइन सहेजी जाती है तो संसाधन को सौंपा गया कार्य प्राप्त करता है या सेट करता है। जब बेसलाइन सहेजी गई थी तो संसाधन को सौंपा गया कार्य की मात्रा। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable इंटरफ़ेस कार्यान्वयन। इस इंस्टेंस की तुलना निर्दिष्ट Baseline ऑब्जेक्ट से करता है। |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | बेसलाइन के लिए हैश कोड मान लौटाता है। |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं। |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं। |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं। |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


