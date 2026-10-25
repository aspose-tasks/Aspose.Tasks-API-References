---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API Reference"
description: "Enthält Details zur PDF‑Verschlüsselung."
type: docs
weight: 189
url: /de/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Enthält Details zur PDF‑Verschlüsselung.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Initialisiert eine neue Instanz der Klasse [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Liest den Verschlüsselungsmodus. |
| [getOwnerPassword()](#getOwnerPassword--) | Liest das Owner-Passwort. |
| [getPermissions()](#getPermissions--) | Liest die Berechtigungen. |
| [getUserPassword()](#getUserPassword--) | Liest das User-Passwort. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Setzt den Verschlüsselungsmodus. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Setzt das Owner-Passwort. |
| [setPermissions(int value)](#setPermissions-int-) | Setzt die Berechtigungen. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Setzt das User-Passwort. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Initialisiert eine neue Instanz der Klasse [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| userPassword | java.lang.String | Das Benutzerpasswort, das das Öffnen geschützter Dokumente ermöglicht. |
| ownerPassword | java.lang.String | Das Owner-Passwort, das das Öffnen geschützter Dokumente ermöglicht. |
| encryptionAlgorithm | int | Die [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm)-Instanz, die den Verschlüsselungsalgorithmus angibt. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Liest den Verschlüsselungsmodus.

**Returns:**
int - der Verschlüsselungsmodus.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Liest das Owner-Passwort.

--------------------

Das Öffnen des Dokuments mit dem korrekten Owner-Passwort (unter der Annahme, dass es nicht dasselbe wie das Benutzerpasswort ist) ermöglicht vollen (Owner-)Zugriff auf das Dokument. Dieser uneingeschränkte Zugriff beinhaltet die Möglichkeit, die Passwörter des Dokuments\\u2019s und die Zugriffsberechtigungen zu ändern.

**Returns:**
java.lang.String - das Owner-Passwort.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Liest die Berechtigungen.

**Returns:**
int - die Berechtigungen.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Liest das User-Passwort.

--------------------

Das Öffnen des Dokuments mit dem korrekten Benutzerpasswort (oder das Öffnen eines Dokuments, das kein Benutzerpasswort hat) ermöglicht zusätzliche Vorgänge, die gemäß den im Dokument\\u2019s Verschlüsselungswörterbuch angegebenen Benutzerzugriffsberechtigungen ausgeführt werden.

**Returns:**
java.lang.String - das Benutzerpasswort.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Setzt den Verschlüsselungsmodus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Verschlüsselungsmodus. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Setzt das Owner-Passwort.

--------------------

Das Öffnen des Dokuments mit dem korrekten Owner-Passwort (unter der Annahme, dass es nicht dasselbe wie das Benutzerpasswort ist) ermöglicht vollen (Owner-)Zugriff auf das Dokument. Dieser uneingeschränkte Zugriff beinhaltet die Möglichkeit, die Passwörter des Dokuments\\u2019s und die Zugriffsberechtigungen zu ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | das Eigentümerpasswort. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Setzt die Berechtigungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Berechtigungen. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Setzt das User-Passwort.

--------------------

Das Öffnen des Dokuments mit dem korrekten Benutzerpasswort (oder das Öffnen eines Dokuments, das kein Benutzerpasswort hat) ermöglicht zusätzliche Vorgänge, die gemäß den im Dokument\\u2019s Verschlüsselungswörterbuch angegebenen Benutzerzugriffsberechtigungen ausgeführt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | das Benutzerpasswort. |

