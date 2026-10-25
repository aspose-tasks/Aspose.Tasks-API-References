---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Specificeert lettertype-instellingen die worden gebruikt bij het renderen van de projectweergave."
type: docs
weight: 101
url: /nl/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Haalt het standaard (of fallback) lettertype op voor rendering. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Haalt een callback op die kan worden gebruikt om opgeloste lettertypen aan te passen. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Haalt een waarde op die aangeeft of het standaardlettertype moet worden gebruikt voor rendering. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Stelt het standaard (of fallback) lettertype in voor rendering. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Stelt de mappen in waar Aspose.Tasks zoekt naar TrueType-lettertypen bij het renderen van de projectweergave. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Stelt een callback in die kan worden gebruikt om opgeloste lettertypen aan te passen. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Stelt een waarde in die aangeeft of het standaardlettertype moet worden gebruikt voor rendering. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Haalt het standaard (of fallback) lettertype op voor rendering.

**Returns:**
java.lang.String - het standaard (of fallback) lettertype voor rendering.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Haalt een callback op die kan worden gebruikt om opgeloste lettertypen aan te passen.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Haalt een waarde op die aangeeft of het standaardlettertype moet worden gebruikt voor rendering.

--------------------

Wanneer de waarde False is en DefaultFontName is opgegeven, zal de renderengine het lettertype gebruiken dat door DefaultFontName is gespecificeerd als fallback-lettertype. Anders worden 'Arial' (indien geïnstalleerd) of 'Generic Sans Serif' lettertypen gebruikt als fallback-lettertype. Het fallback-lettertype wordt gebruikt tijdens het renderen van de projectweergave wanneer een tekststijl verwijst naar een lettertype dat niet op het huidige besturingssysteem is geïnstalleerd. Voor meer controle over lettertype‑resolutie kun je de `FontResolveCallback`([getFontResolveCallback](../../com.aspose/tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose/tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback gebruiken.

**Returns:**
boolean - een waarde die aangeeft of het standaardlettertype moet worden gebruikt voor het renderen.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Stelt het standaard (of fallback) lettertype in voor rendering.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | het standaard (of fallback) lettertype voor het renderen. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Stelt de mappen in waar Aspose.Tasks zoekt naar TrueType-lettertypen bij het renderen van de projectweergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Een array van mappen die TrueType-lettertypen bevatten. |
| recursive | boolean | Als true worden de opgegeven mappen recursief gescand. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Stelt een callback in die kan worden gebruikt om opgeloste lettertypen aan te passen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | een callback die kan worden gebruikt om opgeloste lettertypen aan te passen. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Stelt een waarde in die aangeeft of het standaardlettertype moet worden gebruikt voor rendering.

--------------------

Wanneer de waarde False is en DefaultFontName is opgegeven, zal de renderengine het lettertype gebruiken dat door DefaultFontName is gespecificeerd als fallback-lettertype. Anders worden 'Arial' (indien geïnstalleerd) of 'Generic Sans Serif' lettertypen gebruikt als fallback-lettertype. Het fallback-lettertype wordt gebruikt tijdens het renderen van de projectweergave wanneer een tekststijl verwijst naar een lettertype dat niet op het huidige besturingssysteem is geïnstalleerd. Voor meer controle over lettertype‑resolutie kun je de `FontResolveCallback`([getFontResolveCallback](../../com.aspose/tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose/tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback gebruiken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of het standaardlettertype moet worden gebruikt voor het renderen. |

