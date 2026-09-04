---
title: "ResourceSavingArgs"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Cette classe représente un ensemble de données liées à l'enregistrement de fichiers de ressources externes qui se produit lors de la conversion au format HTML."
type: docs
weight: 254
url: /fr/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Cette classe représente un ensemble de données liées à l'enregistrement du fichier de ressources externe qui se produit lors de la conversion au format HTML.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Fermez le flux si KeepStreamOpen est faux, sinon videz-le. |
| [getFileName()](#getFileName--) | Obtient le nom de fichier supposé qui passe du convertisseur au code de la méthode personnalisée. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Obtient une valeur indiquant si le flux restera ouvert après la fin de l'enregistrement des ressources. |
| [getStream()](#getStream--) | Obtient le contenu binaire du fichier enregistré. |
| [getUri()](#getUri--) | Obtient l'URI de la ressource. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Définit le nom de fichier supposé qui passe du convertisseur au code de la méthode personnalisée. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Définit une valeur indiquant si le flux restera ouvert après la fin de l'enregistrement des ressources. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Définit le contenu binaire du fichier enregistré. |
| [setUri(String value)](#setUri-java.lang.String-) | Définit l'URI de la ressource. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Fermez le flux si KeepStreamOpen est faux, sinon videz-le.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtient le nom de fichier supposé qui passe du convertisseur au code de la méthode personnalisée. Peut être utilisé dans le code personnalisé pour décider comment le traiter ou où enregistrer ce fichier.

**Returns:**
java.lang.String - le nom de fichier supposé qui passe du convertisseur au code de la méthode personnalisée.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Obtient une valeur indiquant si le flux restera ouvert après la fin de l'enregistrement des ressources.

**Returns:**
boolean - une valeur indiquant si le flux restera ouvert après la fin de l'enregistrement des ressources.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Obtient le contenu binaire du fichier enregistré.

**Returns:**
java.io.OutputStream - le contenu binaire du fichier enregistré.
### getUri() {#getUri--}
```
public final String getUri()
```


Obtient l'URI de la ressource.

**Returns:**
java.lang.String - l'URI de la ressource.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Définit le nom de fichier supposé qui passe du convertisseur au code de la méthode personnalisée. Peut être utilisé dans le code personnalisé pour décider comment le traiter ou où enregistrer ce fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le nom de fichier supposé qui passe du convertisseur au code de la méthode personnalisée. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Définit une valeur indiquant si le flux restera ouvert après la fin de l'enregistrement des ressources.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si le flux restera ouvert après la fin de l'enregistrement des ressources. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Définit le contenu binaire du fichier enregistré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.io.OutputStream | le contenu binaire du fichier enregistré. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Définit l'URI de la ressource.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | l'URI de la ressource. |

