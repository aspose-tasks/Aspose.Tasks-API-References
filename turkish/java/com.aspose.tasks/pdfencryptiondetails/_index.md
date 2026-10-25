---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API Referansı"
description: "PDF şifrelemesi için ayrıntıları içerir."
type: docs
weight: 189
url: /tr/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

PDF şifrelemesi için ayrıntıları içerir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Yeni bir [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Şifreleme modunu alır. |
| [getOwnerPassword()](#getOwnerPassword--) | Sahip (Owner) şifresini alır. |
| [getPermissions()](#getPermissions--) | İzinleri alır. |
| [getUserPassword()](#getUserPassword--) | Kullanıcı (User) şifresini alır. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Şifreleme modunu ayarlar. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Sahip (Owner) şifresini ayarlar. |
| [setPermissions(int value)](#setPermissions-int-) | İzinleri ayarlar. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Kullanıcı (User) şifresini ayarlar. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Yeni bir [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| userPassword | java.lang.String | Korunan belgeleri açmaya izin veren kullanıcı şifresi. |
| ownerPassword | java.lang.String | Korunan belgeleri açmaya izin veren sahip şifresi. |
| encryptionAlgorithm | int | Şifreleme algoritmasını gösteren [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) örneği. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Şifreleme modunu alır.

**Returns:**
int - şifreleme modu.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Sahip (Owner) şifresini alır.

--------------------

Doğru sahip şifresiyle (kullanıcı şifresiyle aynı olmadığını varsayarak) belgeyi açmak, belgeye tam (sahip) erişim sağlar. Bu sınırsız erişim, belgenin şifrelerini ve erişim izinlerini değiştirme yeteneğini içerir.

**Returns:**
java.lang.String - Sahip (Owner) şifresi.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


İzinleri alır.

**Returns:**
int - izinler.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Kullanıcı (User) şifresini alır.

--------------------

Doğru kullanıcı şifresiyle belgeyi açmak (veya kullanıcı şifresi olmayan bir belgeyi açmak), belgenin şifreleme sözlüğünde belirtilen kullanıcı erişim izinlerine göre ek işlemlerin gerçekleştirilmesine izin verir.

**Returns:**
java.lang.String - Kullanıcı şifresi.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Şifreleme modunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | şifreleme modu. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Sahip (Owner) şifresini ayarlar.

--------------------

Doğru sahip şifresiyle (kullanıcı şifresiyle aynı olmadığını varsayarak) belgeyi açmak, belgeye tam (sahip) erişim sağlar. Bu sınırsız erişim, belgenin şifrelerini ve erişim izinlerini değiştirme yeteneğini içerir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Sahip şifresi. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


İzinleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | izinler. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Kullanıcı (User) şifresini ayarlar.

--------------------

Doğru kullanıcı şifresiyle belgeyi açmak (veya kullanıcı şifresi olmayan bir belgeyi açmak), belgenin şifreleme sözlüğünde belirtilen kullanıcı erişim izinlerine göre ek işlemlerin gerçekleştirilmesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Kullanıcı şifresi. |

