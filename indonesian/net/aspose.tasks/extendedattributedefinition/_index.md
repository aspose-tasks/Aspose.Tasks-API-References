---
title: "Kelas ExtendedAttributeDefinition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ExtendedAttributeDefinition. Mewakili definisi atribut tambahan yang terkait dengan proyek"
type: docs
weight: 540
url: /id/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Mewakili definisi atribut yang diperluas yang terkait dengan sebuah proyek.

```csharp
public class ExtendedAttributeDefinition
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Mendapatkan atau mengatur alias dari bidang khusus. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai baru yang ditambahkan ke proyek secara otomatis ditambahkan ke daftar. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah penurunan otomatis ke penugasan diaktifkan. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Mendapatkan atau mengatur tipe perhitungan nilai atribut khusus. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Mendapatkan tipe dari bidang khusus. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Mendapatkan atau mengatur nilai default dalam daftar. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Mendapatkan atau mengatur Guid dari entri tabel pencarian default. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Mendapatkan atau mengatur apakah atribut tambahan terkait dengan tugas, sumber daya, atau penugasan. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Mendapatkan atau mengatur yang sesuai dengan id proyek dari bidang khusus. Gunakan representasi string dari konstanta dari kelas [`ExtendedAttributeTask`](../extendedattributetask/) untuk menentukan properti [`FieldId`](./fieldid/). |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Mendapatkan nama bidang khusus. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Mendapatkan atau mengatur rumus yang Microsoft Project gunakan untuk mengisi bidang tugas khusus. |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | Mendapatkan atau mengatur informasi indikator grafis yang terkait dengan atribut yang diperluas. Berlaku untuk format MPP. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Mendapatkan atau mengatur Guid dari bidang khusus. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Mendapatkan Guid dari tabel lookup yang terkait dengan bidang khusus. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Mendapatkan atau mengatur jumlah maksimum nilai yang dapat Anda atur dalam pick list. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Mendapatkan proyek induk untuk instance `ExtendedAttributeDefinition`. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Mendapatkan atau mengatur pengucapan fonetik alias bidang khusus. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai bidang khusus dibatasi pada nilai dalam [`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Mendapatkan atau mengatur cara rollup dihitung. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Mendapatkan atau mengatur guid sekunder dari atribut yang diperluas. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Mendapatkan atau mengatur PID sekunder dari bidang khusus. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Mendapatkan atau mengatur tipe perhitungan nilai atribut khusus untuk baris ringkasan. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah bidang khusus didefinisikan pengguna. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Mendapatkan List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Mendapatkan atau mengatur cara daftar nilai diurutkan. Nilainya: 0=Menurun, 1=Naik. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai Lookup dan hanya dapat digunakan pada Resources. Anda harus menentukan *fieldId* dan *alias* saat memanggil metode ini. Tipe bidang disimpulkan dari field id. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai Lookup dan hanya dapat digunakan pada Resources. Anda harus menentukan *customFieldType*, *fieldId*, dan *alias* saat memanggil metode ini. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai Lookup dan hanya dapat digunakan pada Tasks. Anda harus menentukan *fieldId* dan *alias* saat memanggil metode ini. Tipe bidang disimpulkan dari field id. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai Lookup dan hanya dapat digunakan pada Tasks. Anda harus menentukan *customFieldType*, *fieldId*, dan *alias* saat memanggil metode ini. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut yang diperluas sederhana, yang ditampilkan Microsoft Project sebagai "None". Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai None dan hanya dapat digunakan pada Resource. Anda harus menentukan *fieldId* dan *alias* saat memanggil metode ini. Tipe bidang disimpulkan dari field id. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut yang diperluas sederhana, yang ditampilkan Microsoft Project sebagai "None". Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai None dan hanya dapat digunakan pada Resource. Anda harus menentukan *customFieldType*, *fieldId*, dan *alias* saat memanggil metode ini. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut yang diperluas sederhana, yang ditampilkan Microsoft Project sebagai "None". Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai None dan hanya dapat digunakan pada Tasks. Anda harus menentukan *fieldId* dan *alias* saat memanggil metode ini. Tipe bidang disimpulkan dari field id. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut yang diperluas sederhana, yang ditampilkan Microsoft Project sebagai "None". Metode ini memiliki [`CalculationType`](./calculationtype/) bernilai None dan hanya dapat digunakan pada Tasks. Anda harus menentukan *customFieldType*, *fieldId*, dan *alias* saat memanggil metode ini. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Menambahkan nilai ke daftar lookup internal. Ini adalah cara yang lebih disarankan untuk manipulasi dengan [`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai flag yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai tanggal yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai numerik yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai durasi yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Membuat atribut ekstensi baru dengan field ID yang sama dengan nilai field ID objek ini dan nilai teks yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Membuat atribut ekstensi baru yang terhubung dengan item [`Value`](../value/) yang ditentukan. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Mengembalikan kode hash untuk instance dari kelas `ExtendedAttributeDefinition`. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Menghapus nilai dari daftar pencarian internal. Ini adalah cara yang disarankan untuk manipulasi dengan [`ValueList`](./valuelist/). |

## Contoh

Menampilkan cara menggunakan fungsi matematika umum dengan atribut ekstensi.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Atur Rumus
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Cetak nilai atribut ekstensi
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // Atur Rumus
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Cetak nilai atribut ekstensi
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Atur Rumus
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Cetak nilai atribut ekstensi
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


