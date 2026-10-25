---
title: "Project.GetWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। निर्दिष्ट Double मान और डिफ़ॉल्ट कार्य फ़ॉर्मेट के साथ Duration ऑब्जेक्ट प्राप्त करता है"
type: docs
weight: 1130
url: /hi/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

निर्दिष्ट Double मान और डिफ़ॉल्ट कार्य फ़ॉर्मेट के साथ [`Duration`](../../duration/) ऑब्जेक्ट प्राप्त करता है।

```csharp
public Duration GetWork(double val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | Double | निर्दिष्ट double मान। |

### रिटर्न वैल्यू

Duration ऑब्जेक्ट।

## टिप्पणियाँ

इस मेथड का उपयोग सावधानी से किया जाना चाहिए क्योंकि यह Project.WorkFormat सेटिंग के आधार पर अलग-अलग अवधि लौटाता है। उदाहरण के लिए, GetWork(1.0) 1 घंटे लौटाएगा जब Project.WorkFormat TimeUnitType.Hour है या 1 दिन जब Project.WorkFormat TimeUnitType.Day है।

## उदाहरण

डिफ़ॉल्ट कार्य फ़ॉर्मेट के साथ कार्य प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// प्रोजेक्ट के डिफ़ॉल्ट कार्य फ़ॉर्मेट के साथ एक कार्य मान बनाएं
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### संबंधित देखें

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


