---
title: "OleObject.Content"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα OleObject. Λαμβάνει ή ορίζει τα δεδομένα των ενσωματωμένων αρχείων, null εάν δεν έχουν ενσωματωθεί δεδομένα"
type: docs
weight: 30
url: /el/net/aspose.tasks/oleobject/content/
---
## OleObject.Content property

Λαμβάνει ή ορίζει τα δεδομένα του ενσωματωμένου αρχείου· null εάν δεν ενσωματώθηκαν δεδομένα.

```csharp
public byte[] Content { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε πληροφορίες σχετικά με τα αντικείμενα OLE.

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

### Δείτε επίσης

* class [OleObject](../)
* namespace [Aspose.Tasks](../../oleobject/)
* assembly [Aspose.Tasks](../../../)


