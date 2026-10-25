---
title: "OleObjectCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος OleObjectCollection. Μετατρέπει το στιγμιότυπο της κλάσης OleObjectCollection σε λίστα που περιέχει τα στιγμιότυπα της κλάσης OleObject"
type: docs
weight: 30
url: /el/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

Μετατρέπει το στιγμιότυπο της κλάσης [`OleObjectCollection`](../) σε λίστα που περιέχει τα στιγμιότυπα της κλάσης [`OleObject`](../../oleobject/).

```csharp
public List<OleObject> ToList()
```

### Τιμή Επιστροφής

Μετατράπηκε σε λίστα το στιγμιότυπο της κλάσης [`OleObjectCollection`](../) που περιέχει τα στιγμιότυπα της κλάσης [`OleObject`](../../oleobject/).

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογή αντικειμένων OLE.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// χρησιμοποιώντας πρόσβαση με δείκτη
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// or enumeration one can iterate over OLE objects
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Δείτε επίσης

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


