---
title: "Project.Project"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project कंस्ट्रक्टर। Project क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/project/project/
---
## Project() {#constructor}

एक नया इंस्टेंस इनिशियलाइज़ करता है [`Project`](../) क्लास का।

```csharp
public Project()
```

## उदाहरण

दिखाता है कि एक प्रोजेक्ट कैसे बनाया जाए और उसे MPP फ़ॉर्मेट में सहेजा जाए बिना किसी MPP टेम्प्लेट फ़ाइल को पास किए।

```csharp
var project = new Project();

// प्रोजेक्ट को आंतरिक MPP टेम्प्लेट का उपयोग करके MPP में सहेजा जाएगा।
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

एक नया इंस्टेंस पासवर्ड-सुरक्षित टेम्प्लेट (मौजूदा mpp या mpt फ़ाइल) से इनिशियलाइज़ करता है [`Project`](../) क्लास का।

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | स्ट्रिंग | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पाथ। |
| protectionPassword | स्ट्रिंग | सुरक्षा पासवर्ड। |

## टिप्पणियाँ

वर्तमान में केवल MSP 2003 फ़ाइल फ़ॉर्मेट के लिए पासवर्ड-सुरक्षित फ़ाइलों को पढ़ना समर्थित है।

## उदाहरण

दिखाता है कि पासवर्ड-सुरक्षित MPP फ़ाइलें कैसे पढ़ी जाएँ।

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

एक नया इंस्टेंस टेम्प्लेट (मौजूदा mpp या mpt फ़ाइल) से इनिशियलाइज़ करता है [`Project`](../) क्लास का।

```csharp
public Project(string projectTemplate)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | स्ट्रिंग | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पाथ। |

## उदाहरण

दिखाता है कि MPP फ़ाइल कैसे पढ़ी जाए।

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

एक नया इंस्टेंस स्ट्रीम से इनिशियलाइज़ करता है, साथ ही निर्दिष्ट [`PrimaveraReadOptions`](../../primaverareadoptions/) क्लास का इंस्टेंस।

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | प्रोजेक्ट Streamclass की स्ट्रीम |
| options | PrimaveraReadOptions | निर्दिष्ट [`PrimaveraReadOptions`](../../primaverareadoptions/) क्लास की इंस्टेंस जो Primavera फ़ॉर्मेट्स (XER या XML) को पढ़ने को अनुकूलित करने की अनुमति देती है। |

## उदाहरण

दिखाता है कि कैसे कई प्रोजेक्ट्स वाली Primavera XML या Primavera XER फ़ाइल से स्ट्रीम के माध्यम से प्रोजेक्ट पढ़ा जाए।

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // विशेष UID वाला प्रोजेक्ट लौटाता है।
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### संबंधित देखें

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

एक नया इंस्टेंस टेम्प्लेट (मौजूदा mpp या mpt फ़ाइल) से इनिशियलाइज़ करता है [`Project`](../) क्लास का।

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | स्ट्रिंग | प्रोजेक्ट बनाने के लिए टेम्प्लेट का पाथ। |
| parseErrorHandler | ParseErrorCallback | निर्दिष्ट कॉलबैक मेथड जो XML पार्स त्रुटियों को संभालता है। |

## उदाहरण

अमान्य अक्षरों वाले XML फ़ाइल के साथ स्ट्रीम से प्रोजेक्ट पढ़ने का तरीका दिखाता है।

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // टूटा हुआ टाइमस्पैन वाला XML शामिल करने वाली फ़ाइल खोलें
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### संबंधित देखें

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

स्ट्रीम से नई [`Project`](../) क्लास की इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public Project(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | टेम्पलेट लोड करने के लिए स्ट्रीम। |

## उदाहरण

दिखाता है कि कैसे स्ट्रीम से XML प्रोजेक्ट फ़ाइल पढ़ी जाए।

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

StreamReader इंस्टेंस से नई [`Project`](../) क्लास की इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public Project(StreamReader reader)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| रीडर | StreamReader | स्ट्रीम रीडर जहाँ से टेम्पलेट लोड किया जाता है। |

## उदाहरण

दिखाता है कि कैसे विशिष्ट एन्कोडिंग के साथ MPX फ़ाइलें पढ़ी जाएँ।

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

टेम्पलेट (मौजूदा MPP या MPT फ़ाइल) से नई [`Project`](../) क्लास की इंस्टेंस को निर्दिष्ट [`PrimaveraReadOptions`](../../primaverareadoptions/) क्लास की इंस्टेंस के साथ इनिशियलाइज़ करता है।

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | स्ट्रिंग | प्रोजेक्ट बनाने के लिए टेम्पलेट का पाथ |
| options | PrimaveraReadOptions | निर्दिष्ट [`PrimaveraReadOptions`](../../primaverareadoptions/) क्लास की इंस्टेंस। |

## उदाहरण

दिखाता है कि कैसे Primavera पढ़ने विकल्पों का उपयोग करके कई प्रोजेक्ट्स वाली Primavera XML या Primavera XER फ़ाइल से प्रोजेक्ट पढ़ा जाए।

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// विशेष UID वाला प्रोजेक्ट लौटाता है।
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

डेटाबेस से डेटा पढ़ने के लिए नई [`Project`](../) क्लास की इंस्टेंस को इनिशियलाइज़ करता है, जो [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) क्लास की इंस्टेंस द्वारा निर्दिष्ट है।

```csharp
public Project(DbSettings settings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | DbSettings | निर्दिष्ट [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) क्लास की इंस्टेंस। |

## उदाहरण

दिखाता है कि कैसे डेटाबेस सेटिंग्स का उपयोग करके Primavera डेटाबेस से प्रोजेक्ट इम्पोर्ट किया जाए।

```csharp
var sb = new SqlConnectionStringBuilder
{
    DataSource = "192.168.56.3,1433",
    Encrypt = true,
    TrustServerCertificate = true,
    InitialCatalog = "PrimaveraEDB",
    NetworkLibrary = "DBMSSOCN",
    UserID = "privuser",
    Password = "***",
};

// कनेक्शन स्ट्रिंग और प्रोजेक्ट आईडी के साथ PrimaveraDbSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करें
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Project क्लास की नई इंस्टेंस को इनिशियलाइज़ करें
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नई [`Project`](../) क्लास की इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | टेम्पलेट लोड करने के लिए स्ट्रीम। |
| parseErrorHandler | ParseErrorCallback | निर्दिष्ट कॉलबैक मेथड जो XML पार्स त्रुटियों को संभालता है। |

## उदाहरण

दिखाता है कि कैसे एक प्रोजेक्ट को XML फ़ाइल से अवैध अक्षरों के साथ पढ़ा जाए।

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // उस स्ट्रीम को खोलें जिसमें टूटे हुए टाइमस्पैन के साथ XML हो।
    byte[] bytes = Encoding.UTF8.GetBytes(brokenXmlData);
    using (var stream = new MemoryStream(bytes))
    {
        var project = new Project(stream, CustomDurationHandlerForStream2);
        Console.WriteLine(project.Get(Prj.Name));
    }
}

public static object CustomDurationHandlerForStream2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Debug.Print("Object field : {0}, Invalid value : {1}", args.FieldName, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Debug.Print("New value : {0}", newValue);
    return newValue;
}
```

### संबंधित देखें

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से नई [`Project`](../) क्लास की इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public Project(Stream stream, string protectionPassword)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | टेम्पलेट लोड करने के लिए स्ट्रीम। |
| protectionPassword | स्ट्रिंग | सुरक्षा पासवर्ड। |

## टिप्पणियाँ

वर्तमान में केवल MSP 2003 फ़ाइल फ़ॉर्मेट के लिए पासवर्ड-सुरक्षित फ़ाइलों को पढ़ना समर्थित है।

## उदाहरण

दिखाता है कि कैसे जांचें कि MPP पासवर्ड से सुरक्षित है या नहीं।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

दिखाता है कि कैसे स्ट्रीम से पासवर्ड-संरक्षित MPP फ़ाइलें पढ़ी जाएँ।

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

एक टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से निर्दिष्ट [`LoadOptions`](../../loadoptions/) क्लास के इंस्टेंस के साथ [`Project`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectTemplate | स्ट्रिंग | प्रोजेक्ट बनाने के लिए टेम्पलेट का पाथ |
| options | LoadOptions | निर्दिष्ट [`LoadOptions`](../../loadoptions/) क्लास का इंस्टेंस। |

## उदाहरण

दिखाता है कि कैसे एक फ़ाइल से प्रोजेक्ट को &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; इंस्टेंस का उपयोग करके लोड किया जाए।

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

दिखाता है कि कैसे एक Primavera XML फ़ाइल से त्रुटि पार्सिंग के साथ प्रोजेक्ट पढ़ा जाए।

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// विशेष UID वाला प्रोजेक्ट लौटाता है।
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

[`Project`](../) क्लास का नया इंस्टेंस स्ट्रीम से निर्दिष्ट [`LoadOptions`](../../loadoptions/) क्लास के इंस्टेंस के साथ इनिशियलाइज़ करता है।

```csharp
public Project(Stream stream, LoadOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | प्रोजेक्ट Streamclass की स्ट्रीम |
| options | LoadOptions | निर्दिष्ट [`LoadOptions`](../../loadoptions/) क्लास का इंस्टेंस |

## उदाहरण

दिखाता है कि कैसे एक स्ट्रीम से प्रोजेक्ट को &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; इंस्टेंस का उपयोग करके लोड किया जाए।

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### संबंधित देखें

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


