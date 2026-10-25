---
title: "Asn.Confirmed"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. निर्धारित करता है कि कोई संसाधन ने अपनी सभी असाइनमेंट स्वीकार किए हैं या नहीं"
type: docs
weight: 170
url: /hi/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

निर्धारित करता है कि क्या कोई संसाधन ने अपनी सभी असाइनमेंट्स स्वीकार कर ली हैं।

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## उदाहरण

दिखाता है कि कैसे Asn.Confirmed प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Confirmed, true);

Console.WriteLine("Confirmed: " + assignment.Get(Asn.Confirmed));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


