---
title: "RiskPatternCollection.Add"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RiskPatternCollection मेथड। इस संग्रह में RiskPattern क्लास का एक उदाहरण जोड़ता है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks.riskanalysis/riskpatterncollection/add/
---
## RiskPatternCollection.Add method

इस संग्रह में [`RiskPattern`](../../riskpattern/) क्लास का एक उदाहरण जोड़ता है।

```csharp
public void Add(RiskPattern item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | RiskPattern | इस संग्रह में जोड़ने के लिए [`RiskPattern`](../../riskpattern/) क्लास का एक उदाहरण। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *item* टास्क null है। |

## उदाहरण

रिस्क पैटर्न संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var settings = new RiskAnalysisSettings
{
    // मॉन्टे कार्लो सिमुलेशन के लिए इटरेशन की संख्या सेट करें (डिफ़ॉल्ट मान 100 है)।
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// जब तक RiskPatternCollection केवल-पढ़ने योग्य नहीं है
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// नए पैटर्न जोड़ सकते हैं
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// जोड़े गए पैटर्न पर इटरेट करें
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// इंडेक्स एक्सेस का उपयोग करके संग्रह में पैटर्न को संपादित करें
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// संपादन के बाद पैटर्न जांचें
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// हम पैटर्न को हटा सकते हैं
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// जाँचें कि पैटर्न संग्रह में नहीं है
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// संग्रह को दो तरीकों से साफ़ किया जा सकता है

// पैटर्न को एरे में कॉपी करें और एक-एक करके हटाएँ
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// या कोई पूरी तरह से पैटर्न संग्रह को साफ़ कर सकता है
settings.Patterns.Clear();
```

### संबंधित देखें

* class [RiskPattern](../../riskpattern/)
* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


