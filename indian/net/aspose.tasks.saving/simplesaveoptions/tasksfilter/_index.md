---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SimpleSaveOptions प्रॉपर्टी। वह शर्त प्राप्त करता है या सेट करता है जिसका उपयोग Gantt टास्क शीट और टास्क उपयोग चार्ट पर प्रदर्शित कार्यों को फ़िल्टर करने के लिए किया जाता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Gantt, टास्क शीट और टास्क उपयोग चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त को प्राप्त करता है या सेट करता है।

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## टिप्पणियाँ

यदि मान निर्दिष्ट नहीं किया गया है तो डिफ़ॉल्ट फ़िल्टर उपयोग किया जाता है जो अदृश्य कार्यों को हटाता है — अर्थात् संकुचित कार्यों के वंशज कार्य।

## उदाहरण

दिखाता है कि MS Project फ़ाइल को सहेजते समय कस्टम टास्क फ़िल्टर का उपयोग कैसे किया जाए।

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // एक टास्क फ़िल्टर सेट करें ताकि टास्क 'Task5' और 'Task3' को छोड़ दिया जाए।
        TasksFilter = new CustomTasksFilter()
    };

    // आइए सहेजने के फ़ॉर्मेट की जाँच करें।
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // परियोजना को छवि के रूप में सहेजें
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// उदाहरण: कस्टम टास्क फ़िल्टर जो MS Project फ़ाइल को PDF फ़ॉर्मेट में सहेजते समय (उदाहरण के लिए) उपयोग किया जा सकता है।
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### संबंधित देखें

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


