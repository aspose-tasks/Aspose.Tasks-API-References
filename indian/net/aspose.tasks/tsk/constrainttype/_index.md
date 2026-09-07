---
title: "Tsk.ConstraintType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के शेड्यूलिंग के लिए लागू किए जा सकने वाले प्रतिबंध प्रकार के विकल्प प्रदान करता है"
type: docs
weight: 210
url: /hi/net/aspose.tasks/tsk/constrainttype/
---
## Tsk.ConstraintType field

टास्क के शेड्यूलिंग के लिए लागू किए जा सकने वाले प्रतिबंध प्रकार के विकल्प प्रदान करता है।

```csharp
public static readonly Key<ConstraintType, TaskKey> ConstraintType;
```

## उदाहरण

दिखाता है कि कैसे किसी कार्य के लिए प्रतिबंध को प्राप्त/सेट करें।

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// कार्य Id 11 के लिए प्रतिबंध को यथासंभव देर से सेट करें
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// सभी एकत्रित कार्यों को पार्स करें
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ConstraintType](../../constrainttype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


