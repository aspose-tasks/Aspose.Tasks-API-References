---
title: "PdfEncryptionDetails"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحتوي على تفاصيل لتشفير PDF."
type: docs
weight: 189
url: /ar/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

يحتوي على تفاصيل لتشفير PDF.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | ينشئ مثيلاً جديداً من الفئة [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | يحصل على وضع التشفير. |
| [getOwnerPassword()](#getOwnerPassword--) | يحصل على كلمة مرور Owner. |
| [getPermissions()](#getPermissions--) | يحصل على الأذونات. |
| [getUserPassword()](#getUserPassword--) | يحصل على كلمة مرور User. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | يضبط وضع التشفير. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | يضبط كلمة مرور Owner. |
| [setPermissions(int value)](#setPermissions-int-) | يضبط الأذونات. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | يضبط كلمة مرور User. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


ينشئ مثيلاً جديداً من الفئة [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| userPassword | java.lang.String | كلمة مرور المستخدم التي تسمح بفتح المستندات المحمية. |
| ownerPassword | java.lang.String | كلمة مرور المالك التي تسمح بفتح المستندات المحمية. |
| encryptionAlgorithm | int | مثيل [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) الذي يشير إلى خوارزمية التشفير. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


يحصل على وضع التشفير.

**Returns:**
int - وضع التشفير.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


يحصل على كلمة مرور Owner.

--------------------

فتح المستند باستخدام كلمة مرور المالك الصحيحة (مع افتراض أنها ليست هي نفسها كلمة مرور المستخدم) يسمح بالوصول الكامل (كمالك) إلى المستند. هذا الوصول غير المحدود يشمل القدرة على تغيير كلمات مرور المستند\\u2019s والأذونات.

**Returns:**
java.lang.String - كلمة مرور Owner.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


يحصل على الأذونات.

**Returns:**
int - الأذونات.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


يحصل على كلمة مرور User.

--------------------

فتح المستند باستخدام كلمة مرور المستخدم الصحيحة (أو فتح مستند لا يحتوي على كلمة مرور مستخدم) يسمح بإجراء عمليات إضافية وفقاً لأذونات وصول المستخدم المحددة في قاموس تشفير المستند\\u2019s.

**Returns:**
java.lang.String - كلمة مرور المستخدم.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


يضبط وضع التشفير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | وضع التشفير. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


يضبط كلمة مرور Owner.

--------------------

فتح المستند باستخدام كلمة مرور المالك الصحيحة (مع افتراض أنها ليست هي نفسها كلمة مرور المستخدم) يسمح بالوصول الكامل (كمالك) إلى المستند. هذا الوصول غير المحدود يشمل القدرة على تغيير كلمات مرور المستند\\u2019s والأذونات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | كلمة مرور المالك. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


يضبط الأذونات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الأذونات. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


يضبط كلمة مرور User.

--------------------

فتح المستند باستخدام كلمة مرور المستخدم الصحيحة (أو فتح مستند لا يحتوي على كلمة مرور مستخدم) يسمح بإجراء عمليات إضافية وفقاً لأذونات وصول المستخدم المحددة في قاموس تشفير المستند\\u2019s.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | كلمة مرور المستخدم. |

