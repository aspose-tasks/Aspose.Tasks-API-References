---
title: "Project.Set"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। निर्दिष्ट प्रॉपर्टी को इस कंटेनर में निर्दिष्ट मान से मैप करता है"
type: docs
weight: 1240
url: /hi/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | मैप किए गए मान का प्रकार। |
| key | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [`Prj`](../../prj/) |
| मान | मान। |

## उदाहरण

दिखाता है कि टास्क के गुण कैसे सेट किए जाएँ।

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान पर मैप करता है।

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | Key`2 | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [`Prj`](../../prj/) |
| मान | DateTime | मान। |

## उदाहरण

दिखाता है कि टास्क के गुण कैसे सेट किए जाएँ।

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


