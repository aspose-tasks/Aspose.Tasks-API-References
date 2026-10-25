---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API 参考"
description: "包含 PDF 加密的详细信息。"
type: docs
weight: 189
url: /zh/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

包含 PDF 加密的详细信息。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | 初始化一个新的 [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | 获取加密模式。 |
| [getOwnerPassword()](#getOwnerPassword--) | 获取 Owner 密码。 |
| [getPermissions()](#getPermissions--) | 获取权限。 |
| [getUserPassword()](#getUserPassword--) | 获取 User 密码。 |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | 设置加密模式。 |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | 设置 Owner 密码。 |
| [setPermissions(int value)](#setPermissions-int-) | 设置权限。 |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | 设置 User 密码。 |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


初始化一个新的 [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| userPassword | java.lang.String | 允许打开受保护文档的用户密码。 |
| ownerPassword | java.lang.String | 允许打开受保护文档的所有者密码。 |
| encryptionAlgorithm | int | 指示加密算法的 [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) 实例。 |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


获取加密模式。

**Returns:**
int - 加密模式。
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


获取 Owner 密码。

--------------------

使用正确的 owner 密码打开文档（假设它与 user 密码不同）可获得对文档的完整（owner）访问权限。此无限制的访问包括更改文档\\u2019s 密码和访问权限的能力。

**Returns:**
java.lang.String - Owner 密码。
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


获取权限。

**Returns:**
int - 权限。
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


获取 User 密码。

--------------------

使用正确的 user 密码打开文档（或打开没有 user 密码的文档）可根据文档\\u2019s 加密字典中指定的用户访问权限执行额外操作。

**Returns:**
java.lang.String - 用户密码。
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


设置加密模式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 加密模式。 |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


设置 Owner 密码。

--------------------

使用正确的 owner 密码打开文档（假设它与 user 密码不同）可获得对文档的完整（owner）访问权限。此无限制的访问包括更改文档\\u2019s 密码和访问权限的能力。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 所有者密码。 |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


设置权限。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 权限。 |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


设置 User 密码。

--------------------

使用正确的 user 密码打开文档（或打开没有 user 密码的文档）可根据文档\\u2019s 加密字典中指定的用户访问权限执行额外操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用户密码。 |

