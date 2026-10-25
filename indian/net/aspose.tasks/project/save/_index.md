---
title: "Project.Save"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project method. निर्दिष्ट सहेजने विकल्पों का उपयोग करके दस्तावेज़ को फ़ाइल में सहेजता है"
type: docs
weight: 1200
url: /hi/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

निर्दिष्ट सहेजने विकल्पों का उपयोग करके दस्तावेज़ को फ़ाइल में सहेजता है।

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइलनाम | स्ट्रिंग | फ़ाइल का नाम। |
| विकल्प | SimpleSaveOptions | सहेजने विकल्प। |

## उदाहरण

दिखाता है कि प्रोजेक्ट को MPP फ़ाइल के रूप में कैसे सहेजा जाए।

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### संबंधित देखें

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

परियोजना डेटा को फ़ाइल में सहेजता है।

```csharp
public void Save(string filename, SaveFileFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइलनाम | स्ट्रिंग | फ़ाइल का नाम। |
| फ़ॉर्मेट | SaveFileFormat | सहेजने फ़ाइल फ़ॉर्मेट। |

## उदाहरण

दिखाता है कि एक प्रोजेक्ट कैसे बनाया जाए और उसे MPP फ़ॉर्मेट में सहेजा जाए बिना किसी MPP टेम्प्लेट फ़ाइल को पास किए।

```csharp
var project = new Project();

// प्रोजेक्ट को आंतरिक MPP टेम्प्लेट का उपयोग करके MPP में सहेजा जाएगा।
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

परियोजना डेटा को mpp फ़ॉर्मेट में फ़ाइल में सहेजता है।

```csharp
public void Save(string filename)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइलनाम | स्ट्रिंग | फ़ाइल का नाम। |

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

निर्दिष्ट सहेजने विकल्पों का उपयोग करके परियोजना को स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | स्ट्रीम। |
| विकल्प | SimpleSaveOptions | सहेजने विकल्प। |

## उदाहरण

दिखाता है कि MPP सहेजने विकल्पों का उपयोग करके प्रोजेक्ट को स्ट्रीम में MPP फ़ाइल के रूप में कैसे सहेजा जाए।

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // MPPSaveOptions का उपयोग करके हम इसे MPP फ़ॉर्मेट में सहेजते हैं
    project.Save(stream, options);
}
```

दिखाता है कि प्रोजेक्ट को स्ट्रीम में छवि के रूप में कैसे सहेजा जाए और छवि विकल्पों को कैसे नियंत्रित किया जाए।

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // ImageSaveOptions का उपयोग करके हम प्रोजेक्ट को इमेज़ फ़ॉर्मेट में सहेजते हैं
    project.Save(stream, options);
}
```

### संबंधित देखें

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

परियोजना डेटा को स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | स्ट्रीम। |
| format | SaveFileFormat | निर्दिष्ट सहेजने फ़ाइल फ़ॉर्मेट।[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## उदाहरण

दिखाता है कि प्रोजेक्ट को स्ट्रीम में XML MS Project फ़ाइल के रूप में कैसे सहेजा जाए।

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // स्ट्रीम को XML फ़ॉर्मेट में लिखें
    project.Save(stream, SaveFileFormat.Xml);
}
```

### संबंधित देखें

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


