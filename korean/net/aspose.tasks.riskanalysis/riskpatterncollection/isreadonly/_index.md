---
title: "RiskPatternCollection.IsReadOnly"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RiskPatternCollection 속성. 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. 읽기 전용이 아니면 false를 반환합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/
---
## RiskPatternCollection.IsReadOnly property

이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false.

```csharp
public bool IsReadOnly { get; }
```

## 예제

위험 패턴 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var settings = new RiskAnalysisSettings
{
    // Monte Carlo 시뮬레이션의 반복 횟수를 설정합니다(기본값은 100입니다).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// RiskPatternCollection이 읽기 전용이 아니므로
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// 새 패턴을 추가할 수 있습니다
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

// 추가된 패턴을 순회합니다
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

// 인덱스 접근을 사용하여 컬렉션의 패턴을 편집합니다.
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// 편집 후 패턴을 확인합니다.
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

// 패턴을 제거할 수 있습니다.
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// 컬렉션에 해당 패턴이 없음을 확인합니다.
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// 컬렉션을 두 가지 방법으로 정리할 수 있습니다

// 패턴을 배열에 복사하고 하나씩 삭제합니다.
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// 또는 패턴 컬렉션을 완전히 비울 수 있습니다.
settings.Patterns.Clear();
```

### 또 보기

* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


