---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks untuk Referensi .NET API
description: Mewakili definisi atribut yang diperluas terkait dengan proyek.
type: docs
weight: 540
url: /id/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Mewakili definisi atribut yang diperluas terkait dengan proyek.

```csharp
public class ExtendedAttributeDefinition
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Mendapat atau menyetel alias dari bidang khusus. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah nilai baru yang ditambahkan ke proyek secara otomatis ditambahkan ke daftar. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah roll down otomatis ke tugas diaktifkan. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Mendapat atau menetapkan jenis penghitungan nilai atribut khusus. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Mendapatkan jenis bidang khusus. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Mendapat atau menyetel nilai default dalam daftar. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Mendapat atau menyetel Panduan dari entri tabel pencarian default. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Mendapat atau menyetel atribut yang diperluas dikaitkan dengan tugas, sumber daya, atau tugas. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Mendapat atau menyetel sesuai dengan id proyek bidang khusus. Gunakan representasi string konstanta dari[`ExtendedAttributeTask`](../extendedattributetask/) kelas untuk ditentukan[`FieldId`](./fieldid/) properti. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Mendapatkan nama bidang khusus. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Mendapat atau menyetel rumus yang digunakan Microsoft Project untuk mengisi bidang tugas kustom. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Mendapat atau menyetel Panduan bidang khusus. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Mendapat Panduan tabel pencarian yang terkait dengan bidang khusus. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Mendapat atau menetapkan jumlah nilai maksimum yang dapat Anda atur dalam daftar pilihan. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Mendapatkan proyek induk untuk`ExtendedAttributeDefinition` contoh. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Mendapat atau menyetel pengucapan fonetik dari alias bidang khusus. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah nilai bidang khusus dibatasi untuk nilai di[`ValueList`](./valuelist/) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Mendapat atau menyetel cara perhitungan rollup. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Mendapat atau menyetel panduan sekunder dari atribut yang diperluas. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Mendapat atau menyetel PID sekunder dari bidang khusus. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Mendapat atau menetapkan jenis penghitungan nilai atribut khusus untuk baris ringkasan. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah bidang khusus ditentukan pengguna. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Mendapatkan Daftar&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Mendapat atau mengatur cara daftar nilai diurutkan. Nilainya adalah: 0=Menurun, 1=Menaik. |

## Metode

| Nama | Keterangan |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Memiliki[`CalculationType`](./calculationtype/) sama denganLookup dan hanya dapat digunakan di Sumber Daya. Anda harus menentukan*fieldId* Dan*alias* saat memanggil metode ini. Jenis bidang disimpulkan dari id bidang. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Memiliki[`CalculationType`](./calculationtype/) sama denganLookup dan hanya dapat digunakan di Sumber Daya. Anda harus menentukan*customFieldType* ,*fieldId* Dan*alias* saat memanggil metode ini. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Memiliki[`CalculationType`](./calculationtype/) sama denganLookup dan hanya dapat digunakan di Tugas. Anda harus menentukan*fieldId* Dan*alias* saat memanggil metode ini. Jenis bidang disimpulkan dari id bidang. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut yang diperluas dengan lookup. Memiliki[`CalculationType`](./calculationtype/) sama denganLookup dan hanya dapat digunakan di Tugas. Anda harus menentukan*customFieldType* ,*fieldId* Dan*alias* saat memanggil metode ini. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "Tidak Ada". Memiliki[`CalculationType`](./calculationtype/) sama denganNone dan hanya dapat digunakan di Resource. Anda harus menentukan*fieldId* Dan*alias* saat memanggil metode ini. Jenis bidang disimpulkan dari id bidang. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "Tidak Ada". Memiliki[`CalculationType`](./calculationtype/) sama denganNone dan hanya dapat digunakan di Resource. Anda harus menentukan*customFieldType* ,*fieldId* Dan*alias* saat memanggil metode ini. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "Tidak Ada". Memiliki[`CalculationType`](./calculationtype/) sama denganNone dan hanya dapat digunakan di Tugas. Anda harus menentukan*fieldId* Dan*alias* saat memanggil metode ini. Jenis bidang disimpulkan dari bidang id. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metode pabrik yang membuat definisi atribut tambahan sederhana, yang ditampilkan Microsoft Project sebagai "Tidak Ada". Memiliki[`CalculationType`](./calculationtype/) sama denganNone dan hanya dapat digunakan di Tugas. Anda harus menentukan*customFieldType* ,*fieldId* Dan*alias* saat memanggil metode ini. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Menambahkan nilai ke daftar pencarian internal. Ini adalah cara yang lebih disukai untuk manipulasi dengan[`ValueList`](./valuelist/) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Membuat atribut tambahan baru dengan ID bidang yang sama dengan nilai ID bidang objek ini. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai bendera yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai tanggal yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai numerik yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai durasi yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai teks yang ditentukan. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Membuat atribut tambahan baru yang ditautkan dengan yang ditentukan[`Value`](../value/) barang. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Mengembalikan kode hash untuk instance dari`ExtendedAttributeDefinition` kelas. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Menghapus nilai dari daftar pencarian internal. Ini adalah cara yang lebih disukai untuk manipulasi dengan[`ValueList`](./valuelist/) . |

### Lihat juga

* ruang nama [Aspose.Tasks](../../aspose.tasks/)
* perakitan [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
