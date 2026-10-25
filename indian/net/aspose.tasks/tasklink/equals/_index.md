---
title: "TaskLink.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskLink मेथड। यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं"
type: docs
weight: 90
url: /hi/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public bool Equals(TaskLink other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | TaskLink | इस इंस्टेंस के साथ तुलना करने के लिए निर्दिष्ट [`TaskLink`](../) क्लास का इंस्टेंस। |

### रिटर्न वैल्यू

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## उदाहरण

टास्क लिंक की समानता की जाँच कैसे करें दिखाता है।

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// टास्क लिंक की समानता पूर्व और उत्तर कार्यों पर आधारित है।
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### संबंधित देखें

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | इस इंस्टेंस के साथ तुलना करने के लिए वस्तु। |

### रिटर्न वैल्यू

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## उदाहरण

टास्क लिंक की समानता की जाँच कैसे करें दिखाता है।

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// टास्क लिंक की समानता पूर्व और उत्तर कार्यों पर आधारित है।
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### संबंधित देखें

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


