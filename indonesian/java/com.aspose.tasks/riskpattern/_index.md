---
title: "RiskPattern"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili pola risiko untuk tugas proyek."
type: docs
weight: 268
url: /id/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Mewakili pola risiko untuk tugas proyek.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Menginisialisasi sebuah instance baru dari kelas [RiskPattern](../../com.aspose.tasks/riskpattern). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Mendapatkan tingkat kepercayaan yang sesuai dengan persentase waktu nilai yang dihasilkan sebenarnya berada dalam perkiraan optimis dan pesimis. |
| [getDistribution()](#getDistribution--) | Mendapatkan distribusi probabilitas yang digunakan dalam simulasi Monte Carlo. |
| [getOptimistic()](#getOptimistic--) | Mendapatkan persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik. |
| [getPessimistic()](#getPessimistic--) | Mendapatkan persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk. |
| [getTask()](#getTask--) | Mendapatkan tugas proyek yang diterapkan pola risiko ini. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Mengatur tingkat kepercayaan yang sesuai dengan persentase waktu nilai yang dihasilkan sebenarnya berada dalam perkiraan optimis dan pesimis. |
| [setDistribution(int value)](#setDistribution-int-) | Mengatur distribusi probabilitas yang digunakan dalam simulasi Monte Carlo. |
| [setOptimistic(int value)](#setOptimistic-int-) | Mengatur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik. |
| [setPessimistic(int value)](#setPessimistic-int-) | Mengatur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Menginisialisasi sebuah instance baru dari kelas [RiskPattern](../../com.aspose.tasks/riskpattern).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | tugas proyek yang ditentukan untuk mana risiko ini akan diterapkan dalam simulasi Monte Carlo. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Mendapatkan tingkat kepercayaan yang sesuai dengan persentase waktu nilai yang dihasilkan sebenarnya berada dalam perkiraan optimis dan pesimis. Nilai default adalah CL99.

--------------------

Dapat menjadi salah satu nilai yang didefinisikan dalam enumerasi `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)).

**Returns:**
int - tingkat kepercayaan yang sesuai dengan persentase waktu nilai yang dihasilkan sebenarnya berada dalam perkiraan optimis dan pesimis.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Mendapatkan distribusi probabilitas yang digunakan dalam simulasi Monte Carlo. Nilai default adalah ProbabilityDistributionType.Normal.

--------------------

Dapat menjadi salah satu nilai yang didefinisikan dalam enumerasi [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype).

**Returns:**
int - distribusi probabilitas yang digunakan dalam simulasi Monte Carlo.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Mendapatkan persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik. Nilai default adalah 75, yang berarti jika durasi tugas yang diperkirakan adalah 4 hari maka durasi optimis akan menjadi 3 hari.

**Returns:**
int - persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Mendapatkan persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk. Nilai default adalah 125, yang berarti jika durasi tugas yang diperkirakan adalah 4 hari maka durasi pesimis akan menjadi 5 hari.

**Returns:**
int - persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk.
### getTask() {#getTask--}
```
public final Task getTask()
```


Mendapatkan tugas proyek yang diterapkan pola risiko ini.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Mengatur tingkat kepercayaan yang sesuai dengan persentase waktu nilai yang dihasilkan sebenarnya berada dalam perkiraan optimis dan pesimis. Nilai default adalah CL99.

--------------------

Dapat menjadi salah satu nilai yang didefinisikan dalam enumerasi `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tingkat kepercayaan yang sesuai dengan persentase waktu nilai yang dihasilkan sebenarnya berada dalam perkiraan optimis dan pesimis. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Mengatur distribusi probabilitas yang digunakan dalam simulasi Monte Carlo. Nilai default adalah ProbabilityDistributionType.Normal.

--------------------

Dapat menjadi salah satu nilai yang didefinisikan dalam enumerasi [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | distribusi probabilitas yang digunakan dalam simulasi Monte Carlo. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Mengatur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik. Nilai default adalah 75, yang berarti jika durasi tugas yang diperkirakan adalah 4 hari maka durasi optimis akan menjadi 3 hari.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terbaik. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Mengatur persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk. Nilai default adalah 125, yang berarti jika durasi tugas yang diperkirakan adalah 4 hari maka durasi pesimis akan menjadi 5 hari.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | persentase durasi tugas yang paling mungkin yang dapat terjadi dalam skenario proyek terburuk. |

