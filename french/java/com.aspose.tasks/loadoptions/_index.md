---
title: "LoadOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des paramètres de chargement supplémentaires lors du chargement d'un projet depuis un fichier ou un flux."
type: docs
weight: 148
url: /fr/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Permet de spécifier des paramètres de chargement supplémentaires lors du chargement d'un projet depuis un fichier ou un flux.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initialise une nouvelle instance de la classe [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Obtient un jeton qui peut être utilisé pour annuler une opération de chargement de projet. |
| [getEncoding()](#getEncoding--) | Obtient l'encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. |
| [getErrorHandler()](#getErrorHandler--) | Obtient une méthode de rappel pour gérer les erreurs d'analyse XML. |
| [getPassword()](#getPassword--) | Obtient un mot de passe de protection. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Obtient une instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera (Primavera P6 XER ou Primavera P6 Xml). |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Définit un jeton qui peut être utilisé pour annuler une opération de chargement de projet. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Définit l'encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Définit une méthode de rappel pour gérer les erreurs d'analyse XML. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Définit un mot de passe de protection. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Définit une instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera (Primavera P6 XER ou Primavera P6 Xml). |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialise une nouvelle instance de la classe [LoadOptions](../../com.aspose.tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Obtient un jeton qui peut être utilisé pour annuler une opération de chargement de projet.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtient l'encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. L'encodage par défaut est UTF8.

**Returns:**
java.nio.charset.Charset - encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Obtient une méthode de rappel pour gérer les erreurs d'analyse XML.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Obtient un mot de passe de protection.

**Returns:**
java.lang.String - un mot de passe de protection.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Obtient une instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera (Primavera P6 XER ou Primavera P6 Xml).

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Définit un jeton qui peut être utilisé pour annuler une opération de chargement de projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | un jeton qui peut être utilisé pour annuler une opération de chargement de projet. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Définit l'encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. L'encodage par défaut est UTF8.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.nio.charset.Charset | encodage utilisé pour lire un projet à partir des formats HTML, MPX, XER et Primavera XML. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Définit une méthode de rappel pour gérer les erreurs d'analyse XML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | une méthode de rappel pour gérer les erreurs d'analyse xml. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Définit un mot de passe de protection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | un mot de passe de protection. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Définit une instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera (Primavera P6 XER ou Primavera P6 Xml).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | une instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) qui peut être utilisée pour personnaliser le comportement du chargement des formats Primavera (Primavera P6 XER ou Primavera P6 Xml). |

