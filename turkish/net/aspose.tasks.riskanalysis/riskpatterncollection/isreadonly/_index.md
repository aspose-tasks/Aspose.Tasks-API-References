---
title: "RiskPatternCollection.IsReadOnly"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RiskPatternCollection özelliği. Bu koleksiyonun readonly olup olmadığını gösteren bir değer alır; aksi takdirde false."
type: docs
weight: 20
url: /tr/net/aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/
---
## RiskPatternCollection.IsReadOnly property

Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false.

```csharp
public bool IsReadOnly { get; }
```

## Örnekler

Risk pattern koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var settings = new RiskAnalysisSettings
{
    // Monte Carlo simülasyonu için yineleme sayısını ayarlayın (varsayılan değer 100'dür).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// RiskPatternCollection bir salt-okunur olmadıkça
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// yeni desenler eklenebilir 
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

// eklenen desenler üzerinde yineleme yapın
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

// indeks erişimi kullanarak koleksiyondaki deseni düzenleyin
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// düzenlemelerden sonra desenleri kontrol edin
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

// deseni kaldırabiliriz
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// desenin koleksiyonda olmadığını kontrol edin
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// koleksiyonu iki şekilde temizleyebilirsiniz

// desenleri diziye kopyalayın ve tek tek silin
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// ya da bir desen koleksiyonunu tamamen temizleyebilirsiniz
settings.Patterns.Clear();
```

### Ayrıca Bakınız

* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


