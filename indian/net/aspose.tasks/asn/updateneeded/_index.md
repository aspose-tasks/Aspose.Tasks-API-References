---
title: "Asn.UpdateNeeded"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। निर्धारित करता है कि कार्य को सौंपा गया संसाधन कार्य की स्थिति के अनुसार अपडेट करने की आवश्यकता है या नहीं।"
type: docs
weight: 580
url: /hi/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

निर्धारित करता है कि कार्य को सौंपे गए संसाधन को कार्य की स्थिति के अनुसार अपडेट करने की आवश्यकता है या नहीं।

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## उदाहरण

दिखाता है कि कैसे Asn.UpdateNeeded प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


