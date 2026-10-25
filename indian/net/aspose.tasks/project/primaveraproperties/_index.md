---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। Primavera फ़ाइल से पढ़े गए प्रोजेक्ट के लिए Primavera-विशिष्ट प्रॉपर्टी वाला ऑब्जेक्ट प्राप्त करता है।"
type: docs
weight: 720
url: /hi/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Primavera फ़ाइल से पढ़े गए प्रोजेक्ट के लिए Primavera-विशिष्ट गुणों वाला ऑब्जेक्ट प्राप्त करता है।

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## उदाहरण

Primavera फ़ाइल से प्रोजेक्ट को पढ़ने और प्रोजेक्ट की Primavera-विशिष्ट प्रॉपर्टी की जांच करने का तरीका दिखाता है।

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// विशेष UID वाला प्रोजेक्ट लौटाता है।
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// यदि प्रोजेक्ट के शेड्यूल विकल्पों में डिफ़ॉल्ट मान हैं तो PrimaveraProperties null हो सकता है।
if (project.PrimaveraProperties != null)
{
    Console.WriteLine("Project's schedule options:");
    Console.WriteLine("Relationship Lag Calendar: " + project.PrimaveraProperties.RelationshipLagCalendar);
    Console.WriteLine("Make Open Ended Activities Critical: " + project.PrimaveraProperties.MakeOpenEndedActivitiesCritical);
    Console.WriteLine("Ignore Other Project Relationships: " + project.PrimaveraProperties.IgnoreOtherProjectRelationships);
    Console.WriteLine("Use Expected Finish Dates: " + project.PrimaveraProperties.UseExpectedFinishDates);

    Console.WriteLine("How critical activities are defined: " +
                      project.PrimaveraProperties.CriticalActivitiesDefiningMethod);

    if (project.PrimaveraProperties.CriticalActivitiesDefiningMethod == PrimaveraCriticalActivitiesDefiningMethod.TotalFloat)
    {
        Console.WriteLine("Total Float threshold for critical activities: " + project.PrimaveraProperties.CriticalTotalFloatLimit);
    }
}
```

### संबंधित देखें

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


