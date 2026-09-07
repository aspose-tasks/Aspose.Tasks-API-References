---
title: "Project.GetDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। निर्दिष्ट यूनिट्स की संख्या और डिफ़ॉल्ट अवधि फ़ॉर्मेट के साथ Duration ऑब्जेक्ट प्राप्त करता है, जो प्रोजेक्ट सेटिंग्स में परिभाषित DurationFormat में है।"
type: docs
weight: 1100
url: /hi/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

निर्दिष्ट यूनिट्स की संख्या और डिफ़ॉल्ट अवधि फ़ॉर्मेट के साथ [`Duration`](../../duration/) ऑब्जेक्ट प्राप्त करता है, जो प्रोजेक्ट की सेटिंग्स में परिभाषित [`DurationFormat`](../../prj/durationformat/) में है।

```csharp
public Duration GetDuration(double val)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | Double | निर्दिष्ट यूनिट्स की संख्या। |

### रिटर्न वैल्यू

Duration ऑब्जेक्ट।

## टिप्पणियाँ

इस मेथड का उपयोग सावधानी से करना चाहिए क्योंकि यह Project.DurationFormat सेटिंग के आधार पर विभिन्न अवधि लौटाता है। उदाहरण के लिए, GetWork(1.0) 1 घंटे लौटाएगा जब Project.DurationFormat TimeUnitType.Hour है या 1 दिन जब Project.DurationFormat TimeUnitType.Day है।

## उदाहरण

प्रोजेक्ट फैब्रिक मेथड्स का उपयोग करके डिफ़ॉल्ट प्रोजेक्ट की अवधि फ़ॉर्मेट के साथ &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; इंस्टेंस बनाने का तरीका दिखाता है।

```csharp
var project = new Project();

// डिफ़ॉल्ट प्रोजेक्ट फ़ॉर्मेट के साथ अवधि प्राप्त करें।
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### संबंधित देखें

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

निर्दिष्ट संख्या में [`TimeUnitType`](../../timeunittype/) यूनिट्स के साथ [`Duration`](../../duration/) ऑब्जेक्ट प्राप्त करता है।

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | Double | निर्दिष्ट यूनिट्स की संख्या। |
| timeUnit | TimeUnitType | निर्दिष्ट TimeUnitType मान। |

### रिटर्न वैल्यू

Duration ऑब्जेक्ट।

## उदाहरण

प्रोजेक्ट फैब्रिक मेथड्स का उपयोग करके &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; इंस्टेंस बनाने का तरीका दिखाता है।

```csharp
var project = new Project();

// डिफ़ॉल्ट प्रोजेक्ट फ़ॉर्मेट के साथ अवधि प्राप्त करें।
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### संबंधित देखें

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

निर्दिष्ट TimeSpan मान और निर्दिष्ट [`TimeUnitType`](../../timeunittype/) मान के साथ [`Duration`](../../duration/) ऑब्जेक्ट प्राप्त करता है।

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| timeSpan | TimeSpan | निर्दिष्ट TimeSpan मान। |
| timeUnit | TimeUnitType | निर्दिष्ट TimeUnitType मान। |

### रिटर्न वैल्यू

Duration ऑब्जेक्ट।

### संबंधित देखें

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


