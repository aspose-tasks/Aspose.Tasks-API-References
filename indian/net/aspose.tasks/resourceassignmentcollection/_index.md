---
title: "क्लास ResourceAssignmentCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ResourceAssignmentCollection क्लास। ResourceAssignment ऑब्जेक्ट्स का संग्रह दर्शाता है।"
type: docs
weight: 1760
url: /hi/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

एक संग्रह दर्शाता है [`ResourceAssignment`](../resourceassignment/) ऑब्जेक्ट्स का।

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | ResourceAssignmentCollection में सम्मिलित ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | ResourceAssignmentCollection ऑब्जेक्ट के पैरेंट प्रोजेक्ट को प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकती है। |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है। |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है। |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है। |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | निर्दिष्ट uid वाला असाइनमेंट लौटाता है। |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | यदि संग्रह केवल-पढ़ने योग्य नहीं है तो निर्दिष्ट असाइनमेंट को संग्रह से हटाता है, अन्यथा NotSupportedException फेंकता है। |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | यदि संग्रह केवल-पढ़ने योग्य नहीं है तो निर्दिष्ट इंडेक्स पर असाइनमेंट को हटाता है, अन्यथा NotSupportedException फेंकता है। |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | ResourceAssignmentCollection ऑब्जेक्ट को [`ResourceAssignment`](../resourceassignment/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

रिसोर्स असाइनमेंट संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TemplateResource2010.mpp");

var task = project.RootTask.Children.Add("Task 1");
var resource = project.Resources.Add("Resource 1");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignment.Set(Asn.Work, project.GetWork(40));
assignment.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithUnits = project.ResourceAssignments.Add(task, resource, 1d);
assignmentWithUnits.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithUnits.Set(Asn.Work, project.GetWork(40));
assignmentWithUnits.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithCost = project.ResourceAssignments.Add(task, resource);
assignmentWithCost.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithCost.Set(Asn.Work, project.GetWork(40));
assignmentWithCost.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

Console.WriteLine("Print assignments for the project: " + project.ResourceAssignments.ParentProject.Get(Prj.Name));
Console.WriteLine("Resource assignment count: " + project.ResourceAssignments.Count);
foreach (var resourceAssignment in project.ResourceAssignments)
{
    Console.WriteLine("Task Name: " + resourceAssignment.Get(Asn.Task).Get(Tsk.Name));
    Console.WriteLine("Uid: " + resourceAssignment.Get(Asn.Uid));
    Console.WriteLine("Start: " + resourceAssignment.Get(Asn.Start));
    Console.WriteLine("Work: " + resourceAssignment.Get(Asn.Work));
    Console.WriteLine("Finish: " + resourceAssignment.Get(Asn.Finish));
}

var assignmentByUid = project.ResourceAssignments.GetByUid(2);
Console.WriteLine("Assignment By Uid Start: " + assignmentByUid.Get(Asn.Start));

// असाइनमेंट के साथ काम करें...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// संग्रह को सूची में परिवर्तित करें
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// सूची पर पुनरावृत्ति करें
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### संबंधित देखें

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


