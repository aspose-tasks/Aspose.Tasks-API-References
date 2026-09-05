---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Specifica le impostazioni del carattere utilizzate durante il rendering della vista dei progetti."
type: docs
weight: 101
url: /it/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Specifica le impostazioni del carattere usate durante il rendering della vista del progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Ottiene il carattere predefinito (o di fallback) per il rendering. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Ottiene una callback che può essere usata per personalizzare i caratteri risolti. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Ottiene un valore che indica se il carattere predefinito deve essere usato per il rendering. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Imposta il carattere predefinito (o di fallback) per il rendering. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Imposta le cartelle in cui Aspose.Tasks cerca i font TrueType durante il rendering della vista del progetto. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Imposta una callback che può essere usata per personalizzare i caratteri risolti. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Imposta un valore che indica se il carattere predefinito deve essere usato per il rendering. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Ottiene il carattere predefinito (o di fallback) per il rendering.

**Returns:**
java.lang.String - il carattere predefinito (o di fallback) per il rendering.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Ottiene una callback che può essere usata per personalizzare i caratteri risolti.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Ottiene un valore che indica se il carattere predefinito deve essere usato per il rendering.

--------------------

Quando il valore è False e DefaultFontName è specificato, il motore di rendering utilizzerà il carattere specificato da DefaultFontName come carattere di riserva. Altrimenti vengono utilizzati i caratteri 'Arial' (se installato) o 'Generic Sans Serif' come carattere di riserva. Il carattere di riserva viene utilizzato durante il rendering della vista del progetto quando uno stile di testo fa riferimento a un carattere non installato sul sistema operativo corrente. Per un maggiore controllo sulla risoluzione dei caratteri è possibile utilizzare il callback `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Returns:**
boolean - un valore che indica se il carattere predefinito deve essere utilizzato per il rendering.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Imposta il carattere predefinito (o di fallback) per il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il carattere predefinito (o di riserva) per il rendering. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Imposta le cartelle in cui Aspose.Tasks cerca i font TrueType durante il rendering della vista del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Un array di cartelle che contengono caratteri TrueType. |
| recursive | boolean | Se true le cartelle specificate verranno scansionate ricorsivamente. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Imposta una callback che può essere usata per personalizzare i caratteri risolti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | un callback che può essere utilizzato per personalizzare i caratteri risolti. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Imposta un valore che indica se il carattere predefinito deve essere usato per il rendering.

--------------------

Quando il valore è False e DefaultFontName è specificato, il motore di rendering utilizzerà il carattere specificato da DefaultFontName come carattere di riserva. Altrimenti vengono utilizzati i caratteri 'Arial' (se installato) o 'Generic Sans Serif' come carattere di riserva. Il carattere di riserva viene utilizzato durante il rendering della vista del progetto quando uno stile di testo fa riferimento a un carattere non installato sul sistema operativo corrente. Per un maggiore controllo sulla risoluzione dei caratteri è possibile utilizzare il callback `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se il carattere predefinito deve essere utilizzato per il rendering. |

