---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projektsidor renderas till SVG."
type: docs
weight: 283
url: /sv/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Tillåter att ange ytterligare alternativ när projektsidor renderas till SVG.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Initierar en ny instans av klassen [SvgOptions](../../com.aspose.tasks/svgoptions) som kan användas för att spara projekt i SVG‑format. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Hämtar en användardefinierad implementeringsåteruppringning som används för att få en utström för varje renderad sida. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Bestämmer om en gradientpensel ska användas vid rendering av projektlayout. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ställer in en användardefinierad implementeringsåteruppringning som används för att få en utström för varje renderad sida. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Bestämmer om en gradientpensel ska användas vid rendering av projektlayout. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Initierar en ny instans av klassen [SvgOptions](../../com.aspose.tasks/svgoptions) som kan användas för att spara projekt i SVG‑format.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Reserverad för intern användning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


Reserverad för intern användning.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Hämtar en användardefinierad implementeringsåteruppringning som används för att få en utström för varje renderad sida.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Bestämmer om en gradientpensel ska användas vid rendering av projektlayout.

--------------------

För närvarande stöds inte användning av gradientpensel vid rendering till SVG.

**Returns:**
boolean – värde som indikerar om en gradientpensel ska användas vid rendering av projektlayout.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Ställer in en användardefinierad implementeringsåteruppringning som används för att få en utström för varje renderad sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | en användardefinierad implementationsåteruppringning som används för att hämta en utmatningsström för varje renderad sida. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Bestämmer om en gradientpensel ska användas vid rendering av projektlayout.

--------------------

För närvarande stöds inte användning av gradientpensel vid rendering till SVG.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | värde som indikerar om en gradientpensel ska användas vid rendering av projektlayout. |

