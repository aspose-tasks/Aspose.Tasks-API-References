---
title: "ResourceAssignment.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceAssignment. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas ResourceAssignment."
type: docs
weight: 690
url: /id/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas [`ResourceAssignment`](../).

```csharp
public bool Equals(ResourceAssignment other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | ResourceAssignment | Instance tertentu dari kelas [`ResourceAssignment`](../) untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan penugasan sumber daya.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Lihat Juga

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan penugasan sumber daya.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Lihat Juga

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


