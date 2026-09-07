---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceAssignment. Mendapatkan jumlah pekerjaan berwaktu untuk interval tanggal dan waktu yang ditentukan"
type: docs
weight: 730
url: /id/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Mendapatkan jumlah pekerjaan berwaktu fase untuk interval tanggal-waktu yang ditentukan.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Awal interval tanggal dan waktu. |
| akhir | DateTime | Akhir interval tanggal dan waktu. |
| timephasedDataType | TimephasedDataType | Tipe data berwaktu yang akan digunakan. |

## Contoh

Menampilkan cara menghitung pekerjaan penugasan untuk interval tanggal dan waktu yang arbitrer.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Cetak pekerjaan penugasan untuk setiap jam.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Lihat Juga

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Mendapatkan jumlah pekerjaan berwaktu fase untuk interval tanggal-waktu yang ditentukan.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Awal interval tanggal dan waktu. |
| akhir | DateTime | Akhir interval tanggal dan waktu. |

### Lihat Juga

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


