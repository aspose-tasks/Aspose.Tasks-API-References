---
title: "PrimaveraDbSettings"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Primavera veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamaya olanak tanır."
type: docs
weight: 201
url: /tr/java/com.aspose.tasks/primaveradbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class PrimaveraDbSettings extends DbSettings
```

Primavera veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamaya olanak tanır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PrimaveraDbSettings(String connectionString, int projectId)](#PrimaveraDbSettings-java.lang.String-int-) | Yeni bir [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) sınıf örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getProjectId()](#getProjectId--) | Okunacak projenin kimliğini alır. |
### PrimaveraDbSettings(String connectionString, int projectId) {#PrimaveraDbSettings-java.lang.String-int-}
```
public PrimaveraDbSettings(String connectionString, int projectId)
```


Yeni bir [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) sınıf örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| connectionString | java.lang.String | Belirtilen bağlantı dizesi. |
| projectId | int | okunacak projenin belirtilen kimliği. |

### getProjectId() {#getProjectId--}
```
public final int getProjectId()
```


Okunacak projenin kimliğini alır.

**Returns:**
int - okunacak projenin kimliği.
