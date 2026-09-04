---
title: "PdfEncryptionDetails"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Contient les détails d'un chiffrement PDF."
type: docs
weight: 189
url: /fr/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Contient les détails d'un chiffrement PDF.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Initialise une nouvelle instance de la classe [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Obtient le mode de chiffrement. |
| [getOwnerPassword()](#getOwnerPassword--) | Obtient le mot de passe Owner. |
| [getPermissions()](#getPermissions--) | Obtient les autorisations. |
| [getUserPassword()](#getUserPassword--) | Obtient le mot de passe User. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Définit le mode de chiffrement. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Définit le mot de passe Owner. |
| [setPermissions(int value)](#setPermissions-int-) | Définit les autorisations. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Définit le mot de passe User. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Initialise une nouvelle instance de la classe [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| userPassword | java.lang.String | Le mot de passe user permettant d'ouvrir les documents protégés. |
| ownerPassword | java.lang.String | Le mot de passe owner permettant d'ouvrir les documents protégés. |
| encryptionAlgorithm | int | L'instance [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) qui indique l'algorithme de chiffrement. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Obtient le mode de chiffrement.

**Returns:**
int - le mode de chiffrement.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Obtient le mot de passe Owner.

--------------------

L'ouverture du document avec le mot de passe owner correct (en supposant qu'il ne soit pas identique au mot de passe user) permet un accès complet (owner) au document. Cet accès illimité comprend la capacité de changer les mots de passe du document\\\\u2019s et les autorisations d'accès.

**Returns:**
java.lang.String - le mot de passe Owner.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Obtient les autorisations.

**Returns:**
int - les autorisations.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Obtient le mot de passe User.

--------------------

L'ouverture du document avec le mot de passe user correct (ou l'ouverture d'un document qui n'a pas de mot de passe user) permet d'exécuter des opérations supplémentaires conformément aux autorisations d'accès user spécifiées dans le dictionnaire de chiffrement du document\\\\u2019s.

**Returns:**
java.lang.String - le mot de passe utilisateur.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Définit le mode de chiffrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le mode de chiffrement. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Définit le mot de passe Owner.

--------------------

L'ouverture du document avec le mot de passe owner correct (en supposant qu'il ne soit pas identique au mot de passe user) permet un accès complet (owner) au document. Cet accès illimité comprend la capacité de changer les mots de passe du document\\\\u2019s et les autorisations d'accès.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le mot de passe du propriétaire. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Définit les autorisations.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | les autorisations. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Définit le mot de passe User.

--------------------

L'ouverture du document avec le mot de passe user correct (ou l'ouverture d'un document qui n'a pas de mot de passe user) permet d'exécuter des opérations supplémentaires conformément aux autorisations d'accès user spécifiées dans le dictionnaire de chiffrement du document\\\\u2019s.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le mot de passe utilisateur. |

