---
title: "Project.OleObjects"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει μια συλλογή που περιέχει τις εμφανίσεις της κλάσης OleObject οι οποίες είναι συνδεδεμένες ή ενσωματωμένες σε αυτό το αρχείο έργου. Διαθέσιμο μόνο για μορφή αρχείου mpp. Αυτή η συλλογή είναι μόνο για ανάγνωση εκτός από τη λειτουργία Clear."
type: docs
weight: 700
url: /el/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Λαμβάνει μια συλλογή που περιέχει τις εμφανίσεις της κλάσης [`OleObject`](../../oleobject/) οι οποίες είναι συνδεδεμένες ή ενσωματωμένες σε αυτό το αρχείο έργου. Διαθέσιμο μόνο για μορφή αρχείου mpp. Αυτή η συλλογή είναι μόνο για ανάγνωση εκτός από τη λειτουργία 'Clear'.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Παραδείγματα

Δείχνει πώς να εξάγετε ενσωματωμένα αντικείμενα OLE.

```csharp
IDictionary<string, string> formatExt = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !formatExt.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + formatExt[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Δείτε επίσης

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


