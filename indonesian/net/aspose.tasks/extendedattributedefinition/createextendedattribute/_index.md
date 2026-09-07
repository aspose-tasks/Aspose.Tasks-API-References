---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeDefinition. Membuat atribut ekstensi baru dengan ID bidang yang sama dengan nilai ID bidang objek ini"
type: docs
weight: 310
url: /id/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Nilai Kembali

mengembalikan instance yang dibuat dari kelas [`ExtendedAttribute`](../../extendedattribute/) dengan fieldID yang sama dengan nilai fieldID objek ini.

## Contoh

Menampilkan cara membuat atribut ekstensi.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Jika bidang Kustom tidak ada dalam Proyek, buatlah.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Hasilkan Atribut Ekstensi dari definisi
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Tambahkan atribut ekstensi ke tugas
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai teks yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| textValue | String | Nilai teks yang ditentukan. |

### Nilai Kembali

mengembalikan instance yang dibuat dari kelas [`ExtendedAttribute`](../../extendedattribute/) dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika [`CfType`](../cftype/) saat ini bukan 'Text' |

## Contoh

Menampilkan cara membuat definisi atribut ekstensi dan mengatur nilai string atribut saat konstruksinya.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// buat atribut ekstensi dengan nilai yang sama dengan 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// tambahkan atribut ekstensi yang diinisialisasi dengan nilai 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai numerik yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| numericValue | Decimal | Nilai numerik yang ditentukan. |

### Nilai Kembali

mengembalikan instance yang dibuat dari kelas [`ExtendedAttribute`](../../extendedattribute/) dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika [`CfType`](../cftype/) saat ini bukan 'Number' atau 'Cost' |

## Contoh

Menampilkan cara membuat definisi atribut ekstensi dan mengatur nilai desimal atribut saat konstruksinya.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// buat atribut ekstensi dengan nilai yang sama dengan 999m 
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// tambahkan atribut ekstensi yang diinisialisasi dengan nilai 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai tanggal yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dateTimeValue | DateTime | Nilai tanggal dan waktu yang ditentukan. |

### Nilai Kembali

mengembalikan instance yang dibuat dari kelas [`ExtendedAttribute`](../../extendedattribute/) dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika [`CfType`](../cftype/) saat ini bukan 'Date', 'Start' atau 'Finish' |

## Contoh

Menampilkan cara membuat definisi atribut ekstensi dan mengatur nilai datetime atribut saat sedang dibangun.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// buat atribut ekstensi dengan nilai yang sama dengan DateTime.Now 
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// tambahkan atribut ekstensi
task.ExtendedAttributes.Add(extendedAttribute);
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai durasi yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| durationValue | Durasi | Nilai durasi yang ditentukan. |

### Nilai Kembali

mengembalikan instance yang dibuat dari kelas [`ExtendedAttribute`](../../extendedattribute/) dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika [`CfType`](../cftype/) saat ini bukan 'Duration' |

## Contoh

Menampilkan cara membuat definisi atribut ekstensi dan mengatur durasi saat sedang dibangun.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// atribut ekstensi Duration1 = 2 hari
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// tambahkan atribut ekstensi ke tugas
task.ExtendedAttributes.Add(extendedAttribute);
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai flag yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| flagValue | Boolean | Nilai flag yang ditentukan. |

### Nilai Kembali

mengembalikan instance yang dibuat dari kelas [`ExtendedAttribute`](../../extendedattribute/) dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika [`CfType`](../cftype/) saat ini bukan 'Flag' |

## Contoh

Menampilkan cara membuat definisi atribut yang diperluas dan mengatur nilai flag saat sedang dibangun.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// buat definisi untuk bidang khusus boolean
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// buat atribut dan atur nilai awal menjadi 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Membuat atribut ekstensi baru yang terhubung dengan item [`Value`](../../value/) yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lookupValue | Value | Item [`Value`](../../value/) yang ditentukan. |

### Nilai Kembali

mengembalikan instance yang dibuat dari kelas [`ExtendedAttribute`](../../extendedattribute/) yang terhubung dengan item [`Value`](../../value/) yang ditentukan.

## Catatan

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Contoh

Gunakan kode ini untuk membuat [`ExtendedAttribute`](../../extendedattribute/) baru menggunakan nilai tertentu:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Menampilkan cara membuat definisi atribut ekstensi dan mengatur nilai saat sedang dibangun.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Buat definisi bidang khusus berdasarkan tabel lookup, yang telah dideklarasikan di atas.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// buat atribut ekstensi untuk nilai 
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// tambahkan atribut ekstensi ke tugas
task.ExtendedAttributes.Add(extendedAttribute);
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


