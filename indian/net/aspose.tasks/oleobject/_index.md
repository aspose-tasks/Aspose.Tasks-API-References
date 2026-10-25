---
title: "क्लास OleObject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OleObject क्लास। एक OLE ऑब्जेक्ट का प्रतिनिधित्व करता है जिसे MPP फ़ाइल के गैंट चार्ट व्यू में सम्मिलित किया जा सकता है"
type: docs
weight: 1120
url: /hi/net/aspose.tasks/oleobject/
---
## OleObject class

एक OLE ऑब्जेक्ट का प्रतिनिधित्व करता है जिसे MPP फ़ाइल के Gantt Chart View में डाला जा सकता है।

```csharp
public class OleObject
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OleObject](oleobject/)() | `OleObject` क्लास का एक नया इंस्टेंस प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | एम्बेडेड ऑब्जेक्ट को खोलने के लिए एप्लिकेशन नाम को प्राप्त करता है या सेट करता है। |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | एम्बेडेड फ़ाइल के डेटा को प्राप्त करता है या सेट करता है; यदि कोई डेटा एम्बेड नहीं किया गया तो null। |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | एक फ़्लैग को प्राप्त करता है या सेट करता है जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए। |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | एम्बेडेड ऑब्जेक्ट के फ़ाइल फ़ॉर्मेट को प्राप्त करता है या सेट करता है। |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | सम्मिलित ऑब्जेक्ट के पूर्ण पथ को प्राप्त करता है या सेट करता है। |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | ऑब्जेक्ट आईडी को प्राप्त करता है या सेट करता है। |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | सम्मिलित ऑब्जेक्ट का लेबल प्राप्त करता है या सेट करता है। |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट फ़ाइल में केवल लिंक स्रोत पर संग्रहीत वास्तविक डेटा का लिंक ही है या नहीं। |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | OLE ऑब्जेक्ट के इंस्टेंस का नाम प्राप्त करता है या सेट करता है। |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | सम्मिलित ऑब्जेक्ट की अस्थायी फ़ाइल के पथ को प्राप्त करता है या सेट करता है। |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | सम्मिलित ऑब्जेक्ट से संबंधित [`View`](./view/) क्लास के इंस्टेंस को प्राप्त करता है या सेट करता है। |

## उदाहरण

OLE ऑब्जेक्ट्स के बारे में जानकारी पढ़ने का तरीका दिखाता है।

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


