---
title: "AssignmentBaseline"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili Baseline dari penugasan sumber daya."
type: docs
weight: 17
url: /id/java/com.aspose.tasks/assignmentbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)
```
public class AssignmentBaseline extends Baseline
```

Mewakili Baseline dari penugasan sumber daya.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AssignmentBaseline()](#AssignmentBaseline--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [compareTo(AssignmentBaseline other)](#compareTo-com.aspose.tasks.AssignmentBaseline-) | Implementasi antarmuka IComparable. |
| [equals(AssignmentBaseline other)](#equals-com.aspose.tasks.AssignmentBaseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getFinish()](#getFinish--) | Mendapatkan tanggal selesai terjadwal penugasan sumber daya saat baseline disimpan. |
| [getStart()](#getStart--) | Mendapatkan tanggal mulai terjadwal penugasan sumber daya saat baseline disimpan. |
| [getTimephasedData()](#getTimephasedData--) | Mendapatkan instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk AssignmentBaseline ini. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Mengatur tanggal selesai terjadwal penugasan sumber daya saat baseline disimpan. |
| [setStart(Date value)](#setStart-java.util.Date-) | Mengatur tanggal mulai terjadwal penugasan sumber daya saat baseline disimpan. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Mengatur instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. |
### AssignmentBaseline() {#AssignmentBaseline--}
```
public AssignmentBaseline()
```


### compareTo(AssignmentBaseline other) {#compareTo-com.aspose.tasks.AssignmentBaseline-}
```
public final int compareTo(AssignmentBaseline other)
```


Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | objek Baseline yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
int - mengembalikan -1 jika instance ini kurang dari objek yang ditentukan, 1 jika instance ini lebih besar dari objek yang ditentukan; jika tidak mengembalikan 0
### equals(AssignmentBaseline other) {#equals-com.aspose.tasks.AssignmentBaseline-}
```
public final boolean equals(AssignmentBaseline other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | objek AssignmentBaseline yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - mengembalikan true jika instance ini sama dengan objek AssignmentBaseline yang ditentukan; jika tidak, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | objek yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - mengembalikan true jika instance ini sama dengan objek yang ditentukan; jika tidak, false.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Mendapatkan tanggal selesai terjadwal penugasan sumber daya saat baseline disimpan.

Nilai: Tanggal selesai penugasan sumber daya ketika baseline ini disimpan.

**Returns:**
java.util.Date - tanggal selesai terjadwal penugasan sumber daya saat baseline disimpan.
### getStart() {#getStart--}
```
public final Date getStart()
```


Mendapatkan tanggal mulai terjadwal penugasan sumber daya saat baseline disimpan.

Nilai: Tanggal mulai penugasan sumber daya ketika baseline ini disimpan.

**Returns:**
java.util.Date - tanggal mulai terjadwal penugasan sumber daya saat baseline disimpan.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Mendapatkan instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. Data berfase waktu yang terkait dengan baseline penugasan sumber daya.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) instance for this object. Value: The collection of Time phased data associated with this baseline.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk AssignmentBaseline ini.

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Mengatur tanggal selesai terjadwal penugasan sumber daya saat baseline disimpan.

Nilai: Tanggal selesai penugasan sumber daya ketika baseline ini disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal selesai terjadwal penugasan sumber daya saat baseline disimpan. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Mengatur tanggal mulai terjadwal penugasan sumber daya saat baseline disimpan.

Nilai: Tanggal mulai penugasan sumber daya ketika baseline ini disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal mulai terjadwal penugasan sumber daya saat baseline disimpan. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Mengatur instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. Data berfase waktu yang terkait dengan baseline penugasan sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | instance [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. |

