---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API-referens"
description: "Innehåller detaljer för en PDF-kryptering."
type: docs
weight: 189
url: /sv/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Innehåller detaljer för en PDF-kryptering.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Initierar en ny instans av klassen [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Hämtar krypteringsläget. |
| [getOwnerPassword()](#getOwnerPassword--) | Hämtar ägarlösenordet. |
| [getPermissions()](#getPermissions--) | Hämtar behörigheterna. |
| [getUserPassword()](#getUserPassword--) | Hämtar användarlösenordet. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Ställer in krypteringsläget. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Ställer in ägarlösenordet. |
| [setPermissions(int value)](#setPermissions-int-) | Ställer in behörigheterna. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Ställer in användarlösenordet. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Initierar en ny instans av klassen [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| userPassword | java.lang.String | Användarlösenordet som möjliggör att öppna skyddade dokument. |
| ownerPassword | java.lang.String | Ägarlösenordet som möjliggör att öppna skyddade dokument. |
| encryptionAlgorithm | int | Instansen av [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) som anger krypteringsalgoritmen. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Hämtar krypteringsläget.

**Returns:**
int - krypteringsläget.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Hämtar ägarlösenordet.

--------------------

Att öppna dokumentet med rätt ägarlösenord (förutsatt att det inte är samma som användarlösenordet) ger full (ägare) åtkomst till dokumentet. Denna obegränsade åtkomst inkluderar möjligheten att ändra dokument\\u2019s lösenord och åtkomstbehörigheter.

**Returns:**
java.lang.String - ägarlösenordet.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Hämtar behörigheterna.

**Returns:**
int - behörigheterna.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Hämtar användarlösenordet.

--------------------

Att öppna dokumentet med rätt användarlösenord (eller öppna ett dokument som inte har ett användarlösenord) möjliggör ytterligare operationer som utförs enligt användarens åtkomstbehörigheter som anges i dokument\\u2019s krypteringsordbok.

**Returns:**
java.lang.String - användarlösenordet.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Ställer in krypteringsläget.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | krypteringsläget. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Ställer in ägarlösenordet.

--------------------

Att öppna dokumentet med rätt ägarlösenord (förutsatt att det inte är samma som användarlösenordet) ger full (ägare) åtkomst till dokumentet. Denna obegränsade åtkomst inkluderar möjligheten att ändra dokument\\u2019s lösenord och åtkomstbehörigheter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ägarlösenordet. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Ställer in behörigheterna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | behörigheterna. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Ställer in användarlösenordet.

--------------------

Att öppna dokumentet med rätt användarlösenord (eller öppna ett dokument som inte har ett användarlösenord) möjliggör ytterligare operationer som utförs enligt användarens åtkomstbehörigheter som anges i dokument\\u2019s krypteringsordbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | användarlösenordet. |

