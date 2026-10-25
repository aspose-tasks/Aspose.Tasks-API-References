---
title: "OutlineCode.ValueGuid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineCode प्रॉपर्टी। वैल्यू सूची में मान का GUID प्राप्त या सेट करता है। ValueGuid, वैल्यू सूची में FieldGuid से मेल खाता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

वैल्यू लिस्ट में मान का GUID प्राप्त करता है या सेट करता है। ValueGuid वैल्यू लिस्ट में FieldGuid से मेल खाता है।

```csharp
public string ValueGuid { get; set; }
```

## उदाहरण

टास्क के outline कोड्स को पढ़ने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// outline कोड्स पढ़ें
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### संबंधित देखें

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


