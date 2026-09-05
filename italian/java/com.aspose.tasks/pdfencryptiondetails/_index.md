---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API Reference"
description: "Contiene i dettagli per una crittografia PDF."
type: docs
weight: 189
url: /it/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Contiene i dettagli per una crittografia PDF.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Inizializza una nuova istanza della classe [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Restituisce la modalità di crittografia. |
| [getOwnerPassword()](#getOwnerPassword--) | Restituisce la password Owner. |
| [getPermissions()](#getPermissions--) | Restituisce le autorizzazioni. |
| [getUserPassword()](#getUserPassword--) | Restituisce la password User. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Imposta la modalità di crittografia. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Imposta la password Owner. |
| [setPermissions(int value)](#setPermissions-int-) | Imposta le autorizzazioni. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Imposta la password User. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Inizializza una nuova istanza della classe [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| userPassword | java.lang.String | La password utente che consente di aprire documenti protetti. |
| ownerPassword | java.lang.String | La password owner che consente di aprire documenti protetti. |
| encryptionAlgorithm | int | L'istanza di [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) che indica l'algoritmo di crittografia. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Restituisce la modalità di crittografia.

**Returns:**
int - la modalità di crittografia.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Restituisce la password Owner.

--------------------

Aprire il documento con la password owner corretta (presumendo che non sia la stessa della password user) consente l'accesso completo (owner) al documento. Questo accesso illimitato include la possibilità di modificare le password del documento\\u2019s e le autorizzazioni di accesso.

**Returns:**
java.lang.String - la password Owner.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Restituisce le autorizzazioni.

**Returns:**
int - le autorizzazioni.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Restituisce la password User.

--------------------

Aprire il documento con la password user corretta (o aprire un documento che non possiede una password user) consente di eseguire operazioni aggiuntive in base alle autorizzazioni di accesso user specificate nel dizionario di crittografia del documento\\u2019s.

**Returns:**
java.lang.String - la password utente.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Imposta la modalità di crittografia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | la modalità di crittografia. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Imposta la password Owner.

--------------------

Aprire il documento con la password owner corretta (presumendo che non sia la stessa della password user) consente l'accesso completo (owner) al documento. Questo accesso illimitato include la possibilità di modificare le password del documento\\u2019s e le autorizzazioni di accesso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la password del proprietario. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Imposta le autorizzazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | le autorizzazioni. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Imposta la password User.

--------------------

Aprire il documento con la password user corretta (o aprire un documento che non possiede una password user) consente di eseguire operazioni aggiuntive in base alle autorizzazioni di accesso user specificate nel dizionario di crittografia del documento\\u2019s.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la password utente. |

