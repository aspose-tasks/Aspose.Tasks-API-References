---
title: "Project.SetBaseline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projectmethode. Slaat baseline-velden op naar de opgegeven baseline voor het gehele project"
type: docs
weight: 1250
url: /nl/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Slaat baseline-velden op naar de opgegeven baseline voor het gehele project.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| baselineType | BaselineType | Het baseline-type om baseline-gegevens in op te slaan. |

## Voorbeelden

Toont hoe baselines voor een heel project te maken.

```csharp
var project = new Project();

// Taken toevoegen
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Baseline instellen voor opgegeven taken
project.SetBaseline(BaselineType.Baseline);
```

### Zie ook

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Slaat baseline-velden op naar de opgegeven baseline voor de geselecteerde taken.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| baselineType | BaselineType | Het baseline-type om baseline-gegevens in op te slaan. |
| taskCollection | IEnumerable`1 | Lijst met taken waarvoor baseline-gegevens moeten worden opgeslagen. |

## Voorbeelden

Toont hoe baselines voor specifieke taken te maken.

```csharp
var project = new Project();

// Taken toevoegen
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Baseline instellen voor opgegeven taken
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### Zie ook

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


