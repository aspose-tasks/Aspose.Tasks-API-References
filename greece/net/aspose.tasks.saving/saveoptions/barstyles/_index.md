---
title: "SaveOptions.BarStyles"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει τη λίστα των στιγμιοτύπων της κλάσης BarStyle που εμφανίζονται στην προβολή του έργου."
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/saveoptions/barstyles/
---
## SaveOptions.BarStyles property

Λαμβάνει ή ορίζει τη λίστα των στιγμιοτύπων της κλάσης [`BarStyle`](../../../aspose.tasks.visualization/barstyle/) που εμφανίζονται στην προβολή του έργου.

```csharp
public List<BarStyle> BarStyles { get; set; }
```

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τις γραμμές εργασιών χρησιμοποιώντας &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s.

```csharp
var project = new Project();

var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

var task3 = project.RootTask.Children.Add("Task 3");
var rsc1 = project.Resources.Add("Resource 1");
var rsc2 = project.Resources.Add("Resource 2");
var rsc3 = project.Resources.Add("Resource 3");

project.ResourceAssignments.Add(task1, rsc1);
project.ResourceAssignments.Add(task2, rsc2);
project.ResourceAssignments.Add(task3, rsc3);

SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.ThirdsOfMonths
};

var style = new BarStyle
                {
                    ItemType = BarItemType.CriticalTask,
                    LeftBarTextConverter = delegate(Task t)
                    {
                        return string.Format("This task (ID = {0}) is on critical path", t.Get(Tsk.Id));
                    }
                };

var style2 = new BarStyle { BarColor = Color.DarkOrchid, ItemType = BarItemType.Task };

options.BarStyles = new List<BarStyle> { style, style2 };

project.Save(OutDir + "CustomizeTextWithTaskBars_out.pdf", options);
```

### Δείτε επίσης

* class [BarStyle](../../../aspose.tasks.visualization/barstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


