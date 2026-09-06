---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir önceki bağlantıyı temsil eder."
type: docs
weight: 295
url: /tr/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Bir önceki bağlantıyı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getCrossProjectName()](#getCrossProjectName--) | Dış öncül projeyi alır. |
| [getLagFormat()](#getLagFormat--) | Gecikme formatını ifade etmek için kullanılan biçimi alır. |
| [getLinkLag()](#getLinkLag--) | Dakikanın onda birimi veya yüzde olarak gecikmeyi alır. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | LagFormat'a bağlı olarak gecikme süresini alır. |
| [getLinkType()](#getLinkType--) | Bir bağlantının türünü alır. |
| [getPredTask()](#getPredTask--) | Öncül görevi alır. |
| [getSuccTask()](#getSuccTask--) | Sonraki görevi alır. |
| [hashCode()](#hashCode--) | [TaskLink](../../com.aspose.tasks/tasklink) sınıfının örneği için bir hash code değeri döndürür. |
| [isCrossProject()](#isCrossProject--) | Bir öncülün başka bir projenin parçası olup olmadığını belirten bir değeri alır. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Bir öncülün başka bir projenin parçası olup olmadığını belirten bir değeri ayarlar. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Dış öncül projeyi ayarlar. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Gecikme formatını ifade etmek için kullanılan biçimi ayarlar. |
| [setLinkLag(int value)](#setLinkLag-int-) | Dakikanın onda birimi veya yüzde olarak gecikmeyi ayarlar. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | LagFormat'a bağlı olarak gecikme süresini ayarlar. |
| [setLinkType(int value)](#setLinkType-int-) | Bir bağlantının türünü ayarlar. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Öncül görevi ayarlar. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Sonraki görevi ayarlar. |
| [toString()](#toString--) | Bir TaskLink'in dize temsilini döndürür. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | Bu örnek ile karşılaştırmak için belirtilen [TaskLink](../../com.aspose.tasks/tasklink) sınıfı örneği. |

**Returns:**
boolean - **True** eğer belirtilen [TaskLink](../../com.aspose.tasks/tasklink) sınıfı örneği bu örnek ile aynı öncül ve sonraki görevlere sahipse; aksi takdirde, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak nesne. |

**Returns:**
boolean - **True** eğer belirtilen nesne bu örnekle aynı öncül ve ardıl olan bir TaskLink ise; aksi takdirde **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Dış öncül projeyi alır.

**Returns:**
java.lang.String - dış öncül proje.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Gecikme formatını ifade etmek için kullanılan biçimi alır.

**Returns:**
byte - gecikme biçimini ifade etmek için kullanılan format.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Dakikanın onda birimi veya yüzde olarak gecikmeyi alır.

**Returns:**
int - dakikanın onda birinde veya yüzde olarak gecikme.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


LagFormat'a bağlı olarak gecikme süresini alır.

**Returns:**
double - gecikme süresi, LagFormat'a bağlı olarak.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Bir bağlantının türünü alır.

**Returns:**
int - bir bağlantının türü.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Öncül görevi alır.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Sonraki görevi alır.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[TaskLink](../../com.aspose.tasks/tasklink) sınıfının örneği için bir hash code değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Bir öncülün başka bir projenin parçası olup olmadığını belirten bir değeri alır.

**Returns:**
boolean - bir öncülün başka bir projenin parçası olup olmadığını gösteren değer.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Bir öncülün başka bir projenin parçası olup olmadığını belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir öncülün başka bir projenin parçası olup olmadığını gösteren değer. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Dış öncül projeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | dış öncül proje. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Gecikme formatını ifade etmek için kullanılan biçimi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte | gecikme biçimini ifade etmek için kullanılan format. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Dakikanın onda birimi veya yüzde olarak gecikmeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | dakikanın onda birinde veya yüzde olarak gecikme. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


LagFormat'a bağlı olarak gecikme süresini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | gecikme süresi, LagFormat'a bağlı olarak. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Bir bağlantının türünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir bağlantının türü. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Öncül görevi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | öncül görev. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Sonraki görevi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | ardıl görev. |

### toString() {#toString--}
```
public String toString()
```


Bir TaskLink'in dize temsili döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişikliğe açıktır.

**Returns:**
java.lang.String - TaskLink nesnesini temsil eden dize.
