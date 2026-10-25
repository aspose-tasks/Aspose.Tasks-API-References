---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden."
type: docs
weight: 101
url: /de/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Gibt die Standard‑ (oder Ersatz‑)Schrift für das Rendern zurück. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Gibt einen Callback zurück, der verwendet werden kann, um aufgelöste Schriften anzupassen. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Gibt einen Wert zurück, der angibt, ob die Standardschrift für das Rendern verwendet werden muss. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Legt die Standard‑ (oder Ersatz‑)Schrift für das Rendern fest. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Legt die Ordner fest, in denen Aspose.Tasks nach TrueType‑Schriften sucht, wenn die Projektansicht gerendert wird. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Legt einen Callback fest, der verwendet werden kann, um aufgelöste Schriften anzupassen. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Legt einen Wert fest, der angibt, ob die Standardschrift für das Rendern verwendet werden muss. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Gibt die Standard‑ (oder Ersatz‑)Schrift für das Rendern zurück.

**Returns:**
java.lang.String – die Standard‑ (oder Ersatz‑)Schrift für das Rendern.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Gibt einen Callback zurück, der verwendet werden kann, um aufgelöste Schriften anzupassen.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Gibt einen Wert zurück, der angibt, ob die Standardschrift für das Rendern verwendet werden muss.

--------------------

Wenn der Wert False ist und DefaultFontName angegeben ist, verwendet die Rendering‑Engine die durch DefaultFontName angegebene Schrift als Ersatzschrift. Andernfalls werden 'Arial' (falls installiert) oder 'Generic Sans Serif' als Ersatzschrift verwendet. Die Ersatzschrift wird beim Rendern der Projektansicht verwendet, wenn ein Textstil eine Schrift referenziert, die im aktuellen Betriebssystem nicht installiert ist. Für mehr Kontrolle über die Schriftauflösung können Sie den `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-))‑Callback verwenden.

**Returns:**
boolean – ein Wert, der angibt, ob die Standardschrift für das Rendern verwendet werden muss.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Legt die Standard‑ (oder Ersatz‑)Schrift für das Rendern fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Standard‑ (oder Ersatz‑)Schrift für das Rendern. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Legt die Ordner fest, in denen Aspose.Tasks nach TrueType‑Schriften sucht, wenn die Projektansicht gerendert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Ein Array von Ordnern, die TrueType‑Schriften enthalten. |
| recursive | boolean | Wenn true, werden die angegebenen Ordner rekursiv durchsucht. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Legt einen Callback fest, der verwendet werden kann, um aufgelöste Schriften anzupassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | Ein Callback, der verwendet werden kann, um aufgelöste Schriften anzupassen. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Legt einen Wert fest, der angibt, ob die Standardschrift für das Rendern verwendet werden muss.

--------------------

Wenn der Wert False ist und DefaultFontName angegeben ist, verwendet die Rendering‑Engine die durch DefaultFontName angegebene Schrift als Ersatzschrift. Andernfalls werden 'Arial' (falls installiert) oder 'Generic Sans Serif' als Ersatzschrift verwendet. Die Ersatzschrift wird beim Rendern der Projektansicht verwendet, wenn ein Textstil eine Schrift referenziert, die im aktuellen Betriebssystem nicht installiert ist. Für mehr Kontrolle über die Schriftauflösung können Sie den `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-))‑Callback verwenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Standardschriftart für die Darstellung verwendet werden muss. |

