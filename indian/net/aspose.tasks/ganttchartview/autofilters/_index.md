---
title: "GanttChartView.AutoFilters"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView प्रॉपर्टी। Gantt Chart दृश्य के ऑटो फ़िल्टर की सूची प्राप्त करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Gantt Chart दृश्य के ऑटो फ़िल्टरों की सूची प्राप्त करता है।

```csharp
public FilterCollection AutoFilters { get; }
```

## उदाहरण

दिखाता है कि Gantt chart view के ऑटो फ़िल्टर कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// चलो Gantt chart view के ऑटो फ़िल्टरों पर इटररेट करें।
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// परियोजना के साथ काम करें...
```

### संबंधित देखें

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


