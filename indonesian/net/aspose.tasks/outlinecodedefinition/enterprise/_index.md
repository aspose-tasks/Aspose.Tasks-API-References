---
title: "OutlineCodeDefinition.Enterprise"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "OutlineCodeDefinition properti. Mendapatkan atau mengatur nilai yang menunjukkan apakah kode outline khusus merupakan kode outline khusus enterprise"
type: docs
weight: 40
url: /id/net/aspose.tasks/outlinecodedefinition/enterprise/
---
## OutlineCodeDefinition.Enterprise property

Mendapatkan atau mengatur nilai yang menunjukkan apakah kode outline khusus merupakan kode outline khusus enterprise.

```csharp
public bool Enterprise { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan definisi kode outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// buat definisi kode outline baru
var outline = new OutlineCodeDefinition();

// atur nomor bidang dari sebuah kode outline
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// atur nama kode outline khusus
outline.FieldName = "Outline Code1";

// atur Guid dari sebuah kode outline
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// atur nilai yang menunjukkan apakah nilai yang ditentukan dalam bidang kode outline ini harus berupa nilai daun
outline.LeafOnly = false;

// atur alias dari kode outline khusus
outline.Alias = "My Outline Code";

// atur pelafalan fonetik alias dari kode outline khusus
outline.PhoneticAlias = "Outline Code";

// atur nilai yang menunjukkan apakah kode baru harus memiliki semua level. Tidak tersedia untuk Kode Enterprise.
outline.AllLevelsRequired = true;

// atur nilai yang menunjukkan apakah kode outline khusus merupakan kode outline khusus enterprise
outline.Enterprise = false;

// atur referensi ke bidang khusus lain yang definisi kode outline ini menjadi aliasnya
outline.EnterpriseOutlineCodeAlias = 0;

// tambahkan mask outline
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// atur nilai yang menunjukkan apakah nilai yang ditentukan harus berasal dari tabel nilai
outline.OnlyTableValuesAllowed = false;

// atur nilai yang menunjukkan apakah kode outline khusus dapat digunakan
// oleh Wizard Substitusi Sumber Daya di Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// atur nilai yang menunjukkan apakah indentasi kode outline ini harus ditampilkan.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Lihat Juga

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


