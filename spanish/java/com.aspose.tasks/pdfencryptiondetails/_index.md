---
title: "PdfEncryptionDetails"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Contiene detalles para un cifrado PDF."
type: docs
weight: 189
url: /es/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Contiene detalles para un cifrado PDF.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Inicializa una nueva instancia de la clase [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Obtiene el modo de cifrado. |
| [getOwnerPassword()](#getOwnerPassword--) | Obtiene la contraseña del propietario. |
| [getPermissions()](#getPermissions--) | Obtiene los permisos. |
| [getUserPassword()](#getUserPassword--) | Obtiene la contraseña del usuario. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Establece el modo de cifrado. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Establece la contraseña del propietario. |
| [setPermissions(int value)](#setPermissions-int-) | Establece los permisos. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Establece la contraseña del usuario. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Inicializa una nueva instancia de la clase [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| userPassword | java.lang.String | La contraseña de usuario que permite abrir documentos protegidos. |
| ownerPassword | java.lang.String | La contraseña de propietario que permite abrir documentos protegidos. |
| encryptionAlgorithm | int | La instancia de [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) que indica el algoritmo de cifrado. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Obtiene el modo de cifrado.

**Returns:**
int - el modo de cifrado.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Obtiene la contraseña del propietario.

--------------------

Abrir el documento con la contraseña de propietario correcta (asumiendo que no es la misma que la contraseña de usuario) permite acceso total (propietario) al documento. Este acceso ilimitado incluye la capacidad de cambiar las contraseñas del documento\\u2019s y los permisos de acceso.

**Returns:**
java.lang.String - la contraseña del propietario.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Obtiene los permisos.

**Returns:**
int - los permisos.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Obtiene la contraseña del usuario.

--------------------

Abrir el documento con la contraseña de usuario correcta (o abrir un documento que no tiene contraseña de usuario) permite realizar operaciones adicionales según los permisos de acceso de usuario especificados en el diccionario de cifrado del documento\\u2019s.

**Returns:**
java.lang.String - la contraseña de usuario.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Establece el modo de cifrado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el modo de cifrado. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Establece la contraseña del propietario.

--------------------

Abrir el documento con la contraseña de propietario correcta (asumiendo que no es la misma que la contraseña de usuario) permite acceso total (propietario) al documento. Este acceso ilimitado incluye la capacidad de cambiar las contraseñas del documento\\u2019s y los permisos de acceso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la contraseña del propietario. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Establece los permisos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | los permisos. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Establece la contraseña del usuario.

--------------------

Abrir el documento con la contraseña de usuario correcta (o abrir un documento que no tiene contraseña de usuario) permite realizar operaciones adicionales según los permisos de acceso de usuario especificados en el diccionario de cifrado del documento\\u2019s.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la contraseña de usuario. |

