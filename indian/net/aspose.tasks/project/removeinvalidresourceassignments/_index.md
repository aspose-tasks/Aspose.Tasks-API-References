---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। प्रोजेक्ट संसाधन असाइनमेंट सूची से अमान्य संसाधन असाइनमेंट को हटाता है।"
type: docs
weight: 1170
url: /hi/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

परियोजना संसाधन असाइनमेंट सूची से अमान्य संसाधन असाइनमेंट को हटाता है।

```csharp
public void RemoveInvalidResourceAssignments()
```

## टिप्पणियाँ

MS Project प्रत्येक कार्य के लिए एक खाली संसाधन असाइनमेंट बनाता है। उन्हें हटाने के लिए मेथड को कॉल करें।

## उदाहरण

अमान्य असाइनमेंट को हटाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// अमान्य असाइनमेंट हटाएँ
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


