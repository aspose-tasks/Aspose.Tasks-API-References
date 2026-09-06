---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API-referens"
description: "Anger teckensnittsinställningar som används vid rendering av projektvyn."
type: docs
weight: 101
url: /sv/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Anger teckensnittsinställningar som används när projektets vy renderas.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Hämtar standard (eller reserv) teckensnittet för rendering. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Hämtar en återuppringning som kan användas för att anpassa upplösta teckensnitt. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Hämtar ett värde som indikerar om standardteckensnittet måste användas för rendering. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Ställer in standard (eller reserv) teckensnittet för rendering. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Ställer in mapparna där Aspose.Tasks söker efter TrueType‑teckensnitt när projektets vy renderas. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Ställer in en återuppringning som kan användas för att anpassa upplösta teckensnitt. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Ställer in ett värde som indikerar om standardteckensnittet måste användas för rendering. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Hämtar standard (eller reserv) teckensnittet för rendering.

**Returns:**
java.lang.String – standard (eller reserv) teckensnittet för rendering.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Hämtar en återuppringning som kan användas för att anpassa upplösta teckensnitt.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Hämtar ett värde som indikerar om standardteckensnittet måste användas för rendering.

--------------------

Om värdet är False och DefaultFontName är angivet, kommer renderingsmotorn att använda det teckensnitt som anges av DefaultFontName som reservteckensnitt. Annars används 'Arial' (om installerat) eller 'Generic Sans Serif' som reservteckensnitt. Reservteckensnittet används under rendering av projektvyn när en textstil refererar till ett teckensnitt som inte är installerat på det aktuella operativsystemet. För större kontroll över teckensnittsupplösning kan du använda `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-))‑återuppringning.

**Returns:**
boolean – ett värde som indikerar om standardteckensnittet måste användas för rendering.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Ställer in standard (eller reserv) teckensnittet för rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | standard (eller reserv) teckensnittet för rendering. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Ställer in mapparna där Aspose.Tasks söker efter TrueType‑teckensnitt när projektets vy renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolders | java.lang.String[] | En array av mappar som innehåller TrueType‑teckensnitt. |
| rekursiv | boolean | Om true kommer de angivna mapparna att skannas rekursivt. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Ställer in en återuppringning som kan användas för att anpassa upplösta teckensnitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | en återuppringning som kan användas för att anpassa upplösta teckensnitt. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Ställer in ett värde som indikerar om standardteckensnittet måste användas för rendering.

--------------------

Om värdet är False och DefaultFontName är angivet, kommer renderingsmotorn att använda det teckensnitt som anges av DefaultFontName som reservteckensnitt. Annars används 'Arial' (om installerat) eller 'Generic Sans Serif' som reservteckensnitt. Reservteckensnittet används under rendering av projektvyn när en textstil refererar till ett teckensnitt som inte är installerat på det aktuella operativsystemet. För större kontroll över teckensnittsupplösning kan du använda `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-))‑återuppringning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om standardteckensnittet måste användas för rendering. |

