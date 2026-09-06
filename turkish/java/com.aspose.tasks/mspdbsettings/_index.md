---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API Referansı"
description: "MS Project Server veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamaya izin verir."
type: docs
weight: 161
url: /tr/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

MS Project Server veritabanından proje verilerini okumak için gerekli seçenekleri ayarlamaya izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Yeni bir [MspDbSettings](../../com.aspose.tasks/mspdbsettings) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Okunacak projenin guid'ini alır. |
| [getSchema()](#getSchema--) | MS Project Server'ın şemasını alır. |
| [setSchema(String value)](#setSchema-java.lang.String-) | MS Project Server'ın şemasını ayarlar. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Yeni bir [MspDbSettings](../../com.aspose.tasks/mspdbsettings) sınıfının örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| connectionString | java.lang.String | Belirtilen bağlantı dizesi. |
| projectGuid | java.util.UUID | Okunacak bir projenin belirtilen guid'i. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Okunacak projenin guid'ini alır.

**Returns:**
java.util.UUID - okunacak projenin guid'i.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


MS Project Server'ın şemasını alır. Varsayılan değer "pub"'dur.

**Returns:**
java.lang.String - MS Project Server'ın şeması.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


MS Project Server'ın şemasını ayarlar. Varsayılan değer "pub"'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | MS Project Server'ın şeması. |

