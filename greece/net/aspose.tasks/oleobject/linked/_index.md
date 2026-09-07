---
title: "OleObject.Linked"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα OleObject. Λαμβάνει μια τιμή που υποδεικνύει εάν το αρχείο έργου περιέχει μόνο έναν σύνδεσμο στα πραγματικά δεδομένα που αποθηκεύονται στην πηγή του συνδέσμου"
type: docs
weight: 90
url: /el/net/aspose.tasks/oleobject/linked/
---
## OleObject.Linked property

Λαμβάνει μια τιμή που υποδεικνύει εάν το αρχείο έργου περιέχει μόνο έναν σύνδεσμο προς τα πραγματικά δεδομένα που αποθηκεύονται στην πηγή του συνδέσμου.

```csharp
public bool Linked { get; }
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


