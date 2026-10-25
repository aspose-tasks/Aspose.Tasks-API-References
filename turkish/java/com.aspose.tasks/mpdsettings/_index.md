---
title: "MpdSettings"
second_title: "Aspose.Tasks for Java API Referansı"
description: "MPD biçimi MS Access veritabanı dosya biçiminden proje verilerini okumak için gerekli seçenekleri ayarlamayı sağlar."
type: docs
weight: 160
url: /tr/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

MPD formatından (MS Access veritabanı dosyası formatı) proje verilerini okumak için gerekli seçenekleri ayarlamaya izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | `MpdSettings` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getProjectId()](#getProjectId--) | Okunacak projenin kimliğini döndürür. |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


`MpdSettings` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| connectionString | java.lang.String | Belirtilen bağlantı dizesi. |
| projectId | int | okunacak projenin belirtilen kimliği. |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


Okunacak projenin kimliğini döndürür.

**Returns:**
int - okunacak projenin kimliği.
