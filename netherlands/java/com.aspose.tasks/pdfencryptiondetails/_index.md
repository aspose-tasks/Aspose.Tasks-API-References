---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Bevat details voor een PDF-encryptie."
type: docs
weight: 189
url: /nl/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Bevat details voor een PDF-encryptie.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Initialiseert een nieuw exemplaar van de [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Haalt de encryptiemodus op. |
| [getOwnerPassword()](#getOwnerPassword--) | Haalt het Owner-wachtwoord op. |
| [getPermissions()](#getPermissions--) | Haalt de permissies op. |
| [getUserPassword()](#getUserPassword--) | Haalt het User-wachtwoord op. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Stelt de encryptiemodus in. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Stelt het Owner-wachtwoord in. |
| [setPermissions(int value)](#setPermissions-int-) | Stelt de permissies in. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Stelt het User-wachtwoord in. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Initialiseert een nieuw exemplaar van de [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| userPassword | java.lang.String | Het user-wachtwoord dat het openen van beveiligde documenten mogelijk maakt. |
| ownerPassword | java.lang.String | Het owner-wachtwoord dat het openen van beveiligde documenten mogelijk maakt. |
| encryptionAlgorithm | int | De [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) instantie die het encryptie-algoritme aangeeft. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Haalt de encryptiemodus op.

**Returns:**
int - de encryptiemodus.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Haalt het Owner-wachtwoord op.

--------------------

Het openen van het document met het juiste owner-wachtwoord (ervan uitgaande dat dit niet hetzelfde is als het user-wachtwoord) geeft volledige (owner) toegang tot het document. Deze onbeperkte toegang omvat de mogelijkheid om de wachtwoorden van het document\\u2019s te wijzigen en de toegangspermissies aan te passen.

**Returns:**
java.lang.String - het Owner-wachtwoord.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Haalt de permissies op.

**Returns:**
int - de permissies.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Haalt het User-wachtwoord op.

--------------------

Het openen van het document met het juiste user-wachtwoord (of het openen van een document dat geen user-wachtwoord heeft) maakt extra bewerkingen mogelijk die worden uitgevoerd volgens de gebruikers-toegangspermissies die in de encryptiewoordenboek van het document\\u2019s zijn gespecificeerd.

**Returns:**
java.lang.String - het gebruikerswachtwoord.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Stelt de encryptiemodus in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de encryptiemodus. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Stelt het Owner-wachtwoord in.

--------------------

Het openen van het document met het juiste owner-wachtwoord (ervan uitgaande dat dit niet hetzelfde is als het user-wachtwoord) geeft volledige (owner) toegang tot het document. Deze onbeperkte toegang omvat de mogelijkheid om de wachtwoorden van het document\\u2019s te wijzigen en de toegangspermissies aan te passen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | het eigenaarswachtwoord. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Stelt de permissies in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de machtigingen. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Stelt het User-wachtwoord in.

--------------------

Het openen van het document met het juiste user-wachtwoord (of het openen van een document dat geen user-wachtwoord heeft) maakt extra bewerkingen mogelijk die worden uitgevoerd volgens de gebruikers-toegangspermissies die in de encryptiewoordenboek van het document\\u2019s zijn gespecificeerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | het gebruikerswachtwoord. |

