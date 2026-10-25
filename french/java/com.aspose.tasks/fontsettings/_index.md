---
title: "FontSettings"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Spécifie les paramètres de police utilisés lors du rendu de la vue des projets."
type: docs
weight: 101
url: /fr/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Spécifie les paramètres de police utilisés lors du rendu de la vue du projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Obtient la police par défaut (ou de secours) pour le rendu. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Obtient un rappel qui peut être utilisé pour personnaliser les polices résolues. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Obtient une valeur indiquant si la police par défaut doit être utilisée pour le rendu. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Définit la police par défaut (ou de secours) pour le rendu. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Définit les dossiers où Aspose.Tasks recherche les polices TrueType lors du rendu de la vue du projet. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Définit un rappel qui peut être utilisé pour personnaliser les polices résolues. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Définit une valeur indiquant si la police par défaut doit être utilisée pour le rendu. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Obtient la police par défaut (ou de secours) pour le rendu.

**Returns:**
java.lang.String - la police par défaut (ou de secours) pour le rendu.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Obtient un rappel qui peut être utilisé pour personnaliser les polices résolues.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Obtient une valeur indiquant si la police par défaut doit être utilisée pour le rendu.

--------------------

Lorsque la valeur est False et que DefaultFontName est spécifié, le moteur de rendu utilisera la police spécifiée par DefaultFontName comme police de secours. Sinon, les polices 'Arial' (si installée) ou 'Generic Sans Serif' sont utilisées comme police de secours. La police de secours est utilisée lors du rendu de la vue du projet lorsqu'un style de texte fait référence à une police qui n'est pas installée sur le système d'exploitation actuel. Pour un contrôle plus fin de la résolution des polices, vous pouvez utiliser `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Returns:**
booléen - une valeur indiquant si la police par défaut doit être utilisée pour le rendu.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Définit la police par défaut (ou de secours) pour le rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la police par défaut (ou de secours) pour le rendu. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Définit les dossiers où Aspose.Tasks recherche les polices TrueType lors du rendu de la vue du projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Un tableau de dossiers contenant des polices TrueType. |
| recursive | booléen | Si true, les dossiers spécifiés seront analysés de manière récursive. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Définit un rappel qui peut être utilisé pour personnaliser les polices résolues.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | un rappel qui peut être utilisé pour personnaliser les polices résolues. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Définit une valeur indiquant si la police par défaut doit être utilisée pour le rendu.

--------------------

Lorsque la valeur est False et que DefaultFontName est spécifié, le moteur de rendu utilisera la police spécifiée par DefaultFontName comme police de secours. Sinon, les polices 'Arial' (si installée) ou 'Generic Sans Serif' sont utilisées comme police de secours. La police de secours est utilisée lors du rendu de la vue du projet lorsqu'un style de texte fait référence à une police qui n'est pas installée sur le système d'exploitation actuel. Pour un contrôle plus fin de la résolution des polices, vous pouvez utiliser `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si la police par défaut doit être utilisée pour le rendu. |

