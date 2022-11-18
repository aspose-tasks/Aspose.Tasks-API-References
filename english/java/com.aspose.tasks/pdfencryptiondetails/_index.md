---
title: PdfEncryptionDetails
second_title: Aspose.Tasks for Java API Reference
description: Contains details for a PDF encryption.
type: docs
weight: 176
url: /java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Contains details for a PDF encryption.
## Constructors

| Constructor | Description |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Initializes a new instance of the [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) class. |
## Methods

| Method | Description |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Gets the encryption mode. |
| [getOwnerPassword()](#getOwnerPassword--) | Gets the Owner password. |
| [getPermissions()](#getPermissions--) | Gets the permissions. |
| [getUserPassword()](#getUserPassword--) | Gets the User password. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Sets the encryption mode. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Sets the Owner password. |
| [setPermissions(int value)](#setPermissions-int-) | Sets the permissions. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Sets the User password. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Initializes a new instance of the [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| userPassword | java.lang.String | The user password allowing to open protected documents. |
| ownerPassword | java.lang.String | The owner password allowing to open protected documents. |
| encryptionAlgorithm | int | The [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) instance which indicate encryption algorithm. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Gets the encryption mode.

**Returns:**
int - the encryption mode.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Gets the Owner password.

--------------------

Opening the document with the correct owner password (assuming it is not the same as the user password) allows full (owner) access to the document. This unlimited access includes the ability to change the document\\u2019s passwords and access permissions.

**Returns:**
java.lang.String - the Owner password.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Gets the permissions.

**Returns:**
int - the permissions.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Gets the User password.

--------------------

Opening the document with the correct user password (or opening a document that does not have a user password) allows additional operations to be performed according to the user access permissions specified in the document\\u2019s encryption dictionary.

**Returns:**
java.lang.String - the User password.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Sets the encryption mode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the encryption mode. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Sets the Owner password.

--------------------

Opening the document with the correct owner password (assuming it is not the same as the user password) allows full (owner) access to the document. This unlimited access includes the ability to change the document\\u2019s passwords and access permissions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the Owner password. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Sets the permissions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the permissions. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Sets the User password.

--------------------

Opening the document with the correct user password (or opening a document that does not have a user password) allows additional operations to be performed according to the user access permissions specified in the document\\u2019s encryption dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the User password. |

