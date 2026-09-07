---
title: "WBSCodeDefinition.CodePrefix"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "WBSCodeDefinition properti. Mendapatkan atau mengatur awalan kode proyek"
type: docs
weight: 30
url: /id/net/aspose.tasks/wbscodedefinition/codeprefix/
---
## WBSCodeDefinition.CodePrefix property

Mendapatkan atau mengatur awalan kode proyek.

```csharp
public string CodePrefix { get; set; }
```

## Contoh

Menampilkan cara menambahkan masker kode WBS.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


