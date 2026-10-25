---
title: "Project.SetBaseline"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Tüm proje için belirtilen baseline'e baseline alanlarını kaydeder"
type: docs
weight: 1250
url: /tr/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Tüm proje için belirtilen temel çizgiye temel alan alanlarını kaydeder.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baselineType | BaselineType | Baseline verilerini kaydetmek için baseline türü. |

## Örnekler

Bir bütün proje için baseline'lar oluşturmayı gösterir.

```csharp
var project = new Project();

// Görev ekleme
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Belirtilen görevler için baseline ayarla
project.SetBaseline(BaselineType.Baseline);
```

### Ayrıca Bakınız

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Seçilen görevler için belirtilen temel çizgiye temel alan alanlarını kaydeder.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baselineType | BaselineType | Baseline verilerini kaydetmek için baseline türü. |
| taskCollection | IEnumerable`1 | Baseline verilerini kaydetmek için görevlerin listesi. |

## Örnekler

Belirli görevler için set baseline'ları oluşturmayı gösterir.

```csharp
var project = new Project();

// Görev ekleme
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Belirtilen görevler için baseline ayarla
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### Ayrıca Bakınız

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


