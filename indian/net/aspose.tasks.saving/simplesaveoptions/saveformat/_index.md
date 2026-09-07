---
title: "SimpleSaveOptions.SaveFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SimpleSaveOptions प्रॉपर्टी। वह फ़ॉर्मेट प्राप्त करता है या सेट करता है जिसमें दस्तावेज़ को सहेजा जाएगा यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/simplesaveoptions/saveformat/
---
## SimpleSaveOptions.SaveFormat property

यदि इस सहेजने विकल्प वस्तु का उपयोग किया जाता है तो दस्तावेज़ को सहेजने के लिए उपयोग किए जाने वाले स्वरूप को प्राप्त करता है या सेट करता है।

```csharp
public SaveFileFormat SaveFormat { get; }
```

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

* enum [SaveFileFormat](../../savefileformat/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


