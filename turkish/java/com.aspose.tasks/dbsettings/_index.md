---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje veritabanından okunmak için ayarların belirtilmesine izin verir."
type: docs
weight: 75
url: /tr/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Proje veritabanından okunmak için ayarların belirtilmesine izin verir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Bağlantı dizesini alır. |
| [getDriverClassName()](#getDriverClassName--) | JDBC driver sınıfının bir adını döndürür. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Bağlantı dizesini ayarlar. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | JDBC driver sınıfının bir adını ayarlar. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Bağlantı dizesini alır.

**Returns:**
java.lang.String - bağlantı dizesi.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


JDBC driver sınıfının bir adını döndürür. Varsayılan sürücü sınıfı adı "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - sürücü sınıfı dizesi.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Bağlantı dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | bağlantı dizesi. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


JDBC driver sınıfının bir adını ayarlar. Varsayılan sürücü sınıfı adı "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | JDBC driver sınıfının bir adı. |

