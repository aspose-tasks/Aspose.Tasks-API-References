---
title: "Project.Set"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini"
type: docs
weight: 1240
url: /id/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Parameter | Deskripsi |
| --- | --- |
| T | tipe nilai yang dipetakan. |
| key | kunci properti yang ditentukan. [`Prj`](../../prj/) untuk mendapatkan kunci properti. |
| val | nilai. |

## Contoh

Menampilkan cara mengatur atribut tugas.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | Key`2 | kunci properti yang ditentukan. [`Prj`](../../prj/) untuk mendapatkan kunci properti. |
| val | DateTime | nilai. |

## Contoh

Menampilkan cara mengatur atribut tugas.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


