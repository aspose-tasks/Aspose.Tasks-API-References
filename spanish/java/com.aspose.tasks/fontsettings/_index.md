---
title: "FontSettings"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Especifica la configuración de fuentes utilizada al renderizar la vista de proyectos."
type: docs
weight: 101
url: /es/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Obtiene la fuente predeterminada (o de respaldo) para el renderizado. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Obtiene una devolución de llamada que puede usarse para personalizar las fuentes resueltas. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Obtiene un valor que indica si se debe usar la fuente predeterminada para el renderizado. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Establece la fuente predeterminada (o de respaldo) para el renderizado. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Establece las carpetas donde Aspose.Tasks busca fuentes TrueType al renderizar la vista del proyecto. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Establece una devolución de llamada que puede usarse para personalizar las fuentes resueltas. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Establece un valor que indica si se debe usar la fuente predeterminada para el renderizado. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Obtiene la fuente predeterminada (o de respaldo) para el renderizado.

**Returns:**
java.lang.String - la fuente predeterminada (o de respaldo) para el renderizado.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Obtiene una devolución de llamada que puede usarse para personalizar las fuentes resueltas.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Obtiene un valor que indica si se debe usar la fuente predeterminada para el renderizado.

--------------------

Cuando el valor es False y se especifica DefaultFontName, el motor de renderizado utilizará la fuente especificada por DefaultFontName como fuente de respaldo. De lo contrario, se usan 'Arial' (si está instalada) o fuentes 'Generic Sans Serif' como fuente de respaldo. La fuente de respaldo se utiliza durante el renderizado de la vista del proyecto cuando un estilo de texto hace referencia a una fuente que no está instalada en el sistema operativo actual. Para un mayor control sobre la resolución de fuentes, puede usar la devolución de llamada `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)).

**Returns:**
boolean - un valor que indica si la fuente predeterminada debe usarse para el renderizado.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Establece la fuente predeterminada (o de respaldo) para el renderizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la fuente predeterminada (o de respaldo) para el renderizado. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Establece las carpetas donde Aspose.Tasks busca fuentes TrueType al renderizar la vista del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Una matriz de carpetas que contienen fuentes TrueType. |
| recursive | boolean | Si es true, las carpetas especificadas se escanearán de forma recursiva. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Establece una devolución de llamada que puede usarse para personalizar las fuentes resueltas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | una devolución de llamada que puede usarse para personalizar las fuentes resueltas. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Establece un valor que indica si se debe usar la fuente predeterminada para el renderizado.

--------------------

Cuando el valor es False y se especifica DefaultFontName, el motor de renderizado utilizará la fuente especificada por DefaultFontName como fuente de respaldo. De lo contrario, se usan 'Arial' (si está instalada) o fuentes 'Generic Sans Serif' como fuente de respaldo. La fuente de respaldo se utiliza durante el renderizado de la vista del proyecto cuando un estilo de texto hace referencia a una fuente que no está instalada en el sistema operativo actual. Para un mayor control sobre la resolución de fuentes, puede usar la devolución de llamada `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si la fuente predeterminada debe usarse para el renderizado. |

