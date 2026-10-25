---
title: "FontResolveEventArgs"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Fournit des arguments pour le rappel qui est invoqué lorsque la police est résolue."
type: docs
weight: 99
url: /fr/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Fournit des arguments pour le rappel qui est invoqué lorsque la police est résolue.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Obtient le nom de la police demandée. |
| [getResolvedFontName()](#getResolvedFontName--) | Obtient le nom de la police résolue. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Définit le nom de la police résolue. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Obtient le nom de la police demandée.

**Returns:**
java.lang.String - le nom de la police demandée.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Obtient le nom de la police résolue. Peut être défini pour contrôler les polices utilisées pour rendre une vue.

**Returns:**
java.lang.String - Nom de la police demandée si la police est trouvée ou nom de la police de secours ou null si la police ne peut pas être trouvée.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Définit le nom de la police résolue. Peut être défini pour contrôler les polices utilisées pour rendre une vue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le nom de la police résolue. |

