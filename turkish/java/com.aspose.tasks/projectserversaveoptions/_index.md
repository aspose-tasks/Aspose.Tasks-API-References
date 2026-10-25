---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje Project Server veya Project Online'a kaydedildiğinde ek seçenekler belirtmeye izin verir."
type: docs
weight: 227
url: /tr/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Proje Project Server veya Project Online'a kaydedildiğinde ek seçenekler belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Kuyruk iş durumu istekleri arasındaki aralığı alır. |
| [getProjectGuid()](#getProjectGuid--) | Bir projenin benzersiz tanımlayıcısını alır. |
| [getProjectName()](#getProjectName--) | Project Server \\ Project Online projeler listesinde görüntülenen bir projenin adını alır. |
| [getTimeout()](#getTimeout--) | Project Server'ın kuyruk işleme hizmeti tarafından proje kaydetme isteğinin işlenmesi beklenirken kullanılan zaman aşımını alır. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Kuyruk iş durumu istekleri arasındaki aralığı ayarlar. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Bir projenin benzersiz tanımlayıcısını ayarlar. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Project Server \\ Project Online projeler listesinde görüntülenen bir projenin adını ayarlar. |
| [setTimeout(double value)](#setTimeout-double-) | Project Server'ın kuyruk işleme hizmeti tarafından proje kaydetme isteğinin işlenmesi beklenirken kullanılan zaman aşımını ayarlar. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


[ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) sınıfının yeni bir örneğini başlatır.

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Kuyruk iş durumu istekleri arasındaki aralığı alır. Varsayılan değer 2 saniyedir.

**Returns:**
double - kuyruk iş durumu istekleri arasındaki aralık.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Bir projenin benzersiz tanımlayıcısını alır. Project Server \\ Project Online örneği içinde benzersiz olmalıdır.

**Returns:**
java.util.UUID - bir projenin benzersiz tanımlayıcısı.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Project Server \\ Project Online projeler listesinde görüntülenen bir projenin adını alır. Project Server \\ Project Online örneği içinde benzersiz olmalıdır. Değer atlanırsa, Prj.Name özelliğinin değeri kullanılacaktır.

**Returns:**
java.lang.String - Project Server \\ Project Online projeler listesinde görüntülenen bir projenin adı.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Project Server'ın kuyruk işleme hizmeti tarafından proje kaydetme isteğinin işlenmesi beklenirken kullanılan zaman aşımını alır. Bu özelliğin varsayılan değeri 1 dakikadır.

--------------------

İşlem süresi, büyük projeler için veya Project Server örneği diğer isteklere yanıt vermekte çok meşgulse daha uzun olabilir.

**Returns:**
double - Project Server'ın kuyruk işleme servisi tarafından proje kaydetme isteğinin işlenmesini beklerken kullanılan zaman aşımı.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Kuyruk iş durumu istekleri arasındaki aralığı ayarlar. Varsayılan değer 2 saniyedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Kuyruk iş durumu istekleri arasındaki aralık. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Bir projenin benzersiz tanımlayıcısını ayarlar. Project Server \\ Project Online örneği içinde benzersiz olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.UUID | Bir projenin benzersiz tanımlayıcısı. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Project Server \\ Project Online proje listesinde görüntülenen bir projenin adını ayarlar. Project Server \\ Project Online örneği içinde benzersiz olmalıdır. Değer atlanırsa, Prj.Name özelliğinin değeri kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Project Server \\ Project Online proje listesinde görüntülenen bir projenin adı. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Project Server'ın kuyruk işleme servisi tarafından proje kaydetme isteğinin işlenmesini beklerken kullanılan zaman aşımını ayarlar. Bu özelliğin varsayılan değeri 1 dakikadır.

--------------------

İşlem süresi, büyük projeler için veya Project Server örneği diğer isteklere yanıt vermekte çok meşgulse daha uzun olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Project Server'ın kuyruk işleme servisi tarafından proje kaydetme isteğinin işlenmesini beklerken kullanılan zaman aşımı. |

