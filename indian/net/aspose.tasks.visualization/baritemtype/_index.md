---
title: "एनम BarItemType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.BarItemType enum. बार शैली बदलने के लिए आइटम प्रकार"
type: docs
weight: 2940
url: /hi/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

बार शैली को बदलने के लिए आइटम प्रकार।

```csharp
public enum BarItemType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Task | `0` | टास्क बार आइटम प्रकार को दर्शाता है। |
| Summary | `1` | समरी बार आइटम प्रकार को दर्शाता है। |
| ProjectSummary | `2` | प्रोजेक्ट समरी बार आइटम प्रकार को दर्शाता है। |
| ManualTask | `3` | मैन्युअल टास्क बार आइटम प्रकार को दर्शाता है। |
| InactiveTask | `4` | निष्क्रिय टास्क बार आइटम प्रकार को दर्शाता है। |
| CriticalTask | `5` | क्रिटिकल टास्क बार आइटम प्रकार को दर्शाता है। |
| Milestone | `6` | माइलस्टोन टास्क बार आइटम प्रकार को दर्शाता है। |
| ManualSummary | `7` | मैन्युअल समरी बार आइटम प्रकार को दर्शाता है। |
| Split | `8` | स्प्लिट बार आइटम प्रकार को दर्शाता है। |
| ExternalTasks | `9` | बाहरी टास्क्स बार आइटम प्रकार को दर्शाता है। |
| ExternalMilestone | `10` | बाहरी माइलस्टोन बार आइटम प्रकार को दर्शाता है। |
| Deadline | `11` | डेडलाइन बार आइटम प्रकार को दर्शाता है। |
| Progress | `12` | प्रोग्रेस बार आइटम प्रकार को दर्शाता है। |
| StartOnly | `13` | केवल-स्टार्ट बार आइटम प्रकार को दर्शाता है। |
| FinishOnly | `14` | केवल-फ़िनिश बार आइटम प्रकार को दर्शाता है। |
| DurationOnly | `15` | केवल-ड्यूरेशन बार आइटम प्रकार को दर्शाता है। |
| InactiveMilestone | `16` | निष्क्रिय माइलस्टोन बार आइटम प्रकार को दर्शाता है। |
| InactiveSummary | `17` | निष्क्रिय सारांश बार आइटम प्रकार को दर्शाता है। |
| SummaryRollup | `18` | सारांश रोलअप बार आइटम प्रकार। |

## उदाहरण

कार्य बार को अनुकूलित करने के लिए &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s का उपयोग कैसे दिखाता है।

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

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


