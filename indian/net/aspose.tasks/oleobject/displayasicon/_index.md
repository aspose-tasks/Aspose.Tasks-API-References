---
title: "OleObject.DisplayAsIcon"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OleObject प्रॉपर्टी। एक फ़्लैग प्राप्त या सेट करती है जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए"
type: docs
weight: 40
url: /hi/net/aspose.tasks/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

एक फ़्लैग को प्राप्त करता है या सेट करता है जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए।

```csharp
public bool DisplayAsIcon { get; set; }
```

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

* class [OleObject](../)
* namespace [Aspose.Tasks](../../oleobject/)
* assembly [Aspose.Tasks](../../../)


