---
title: CreateExtendedAttribute
second_title: Aspose.Tasks untuk Referensi .NET API
description: Membuat atribut tambahan baru dengan ID bidang yang sama dengan nilai ID bidang objek ini.
type: docs
weight: 300
url: /id/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Membuat atribut tambahan baru dengan ID bidang yang sama dengan nilai ID bidang objek ini.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Nilai Pengembalian

mengembalikan instance yang dibuat dari[`ExtendedAttribute`](../../extendedattribute/)kelas dengan fieldID yang sama dengan nilai fieldID objek ini.

### Lihat juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai teks yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| textValue | String | Nilai teks yang ditentukan. |

### Nilai Pengembalian

mengembalikan instance yang dibuat dari[`ExtendedAttribute`](../../extendedattribute/)kelas dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika saat ini[`CfType`](../cftype/) bukan 'Teks' |

### Lihat juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai numerik yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| numericValue | Decimal | Nilai numerik yang ditentukan. |

### Nilai Pengembalian

mengembalikan instance yang dibuat dari[`ExtendedAttribute`](../../extendedattribute/)kelas dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika saat ini[`CfType`](../cftype/) bukan 'Jumlah' atau 'Biaya' |

### Lihat juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai tanggal yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| dateTimeValue | DateTime | Nilai waktu tanggal yang ditentukan. |

### Nilai Pengembalian

mengembalikan instance yang dibuat dari[`ExtendedAttribute`](../../extendedattribute/)kelas dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika saat ini[`CfType`](../cftype/) bukan 'Tanggal', 'Mulai' atau 'Selesai' |

### Lihat juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai durasi yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| durationValue | Duration | Nilai durasi yang ditentukan. |

### Nilai Pengembalian

mengembalikan instance yang dibuat dari[`ExtendedAttribute`](../../extendedattribute/)kelas dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika saat ini[`CfType`](../cftype/) bukan 'Durasi' |

### Lihat juga

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Membuat atribut baru yang diperluas dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai bendera yang ditentukan.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| flagValue | Boolean | Nilai bendera yang ditentukan. |

### Nilai Pengembalian

mengembalikan instance yang dibuat dari[`ExtendedAttribute`](../../extendedattribute/)kelas dengan fieldID yang sama dengan nilai fieldID objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika saat ini[`CfType`](../cftype/) bukan 'Bendera' |

### Lihat juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Membuat atribut tambahan baru yang ditautkan dengan yang ditentukan[`Value`](../../value/) barang.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| lookupValue | Value | Yang ditentukan[`Value`](../../value/) barang. |

### Nilai Pengembalian

mengembalikan instance yang dibuat dari[`ExtendedAttribute`](../../extendedattribute/) kelas terkait dengan ditentukan[`Value`](../../value/) barang.

### Perkataan

*lookupValue* sebelumnya harus ditambahkan ke[`ExtendedAttributeDefinition`](../) menggunakan[`AddLookupValue`](../addlookupvalue/) metode.

### Contoh

Gunakan kode ini untuk membuat yang baru[`ExtendedAttribute`](../../extendedattribute/) menggunakan nilai tertentu:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

### Lihat juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* ruang nama [Aspose.Tasks](../../extendedattributedefinition/)
* perakitan [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
