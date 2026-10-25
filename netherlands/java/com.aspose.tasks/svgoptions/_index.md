---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het renderen van projectpagina's naar SVG."
type: docs
weight: 283
url: /nl/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Staat toe extra opties op te geven bij het renderen van projectpagina's naar SVG.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Initialiseert een nieuw exemplaar van de [SvgOptions](../../com.aspose/tasks/svgoptions) klasse die kan worden gebruikt om een project op te slaan in SVG-formaat. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Haalt een door de gebruiker gedefinieerde implementatie‑callback op die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Bepaalt of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Stelt een door de gebruiker gedefinieerde implementatie‑callback in die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Bepaalt of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Initialiseert een nieuw exemplaar van de [SvgOptions](../../com.aspose/tasks/svgoptions) klasse die kan worden gebruikt om een project op te slaan in SVG-formaat.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Gereserveerd voor intern gebruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


Gereserveerd voor intern gebruik.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Haalt een door de gebruiker gedefinieerde implementatie‑callback op die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Bepaalt of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out.

--------------------

Het gebruik van een gradient‑kwast wordt momenteel niet ondersteund voor het renderen naar SVG.

**Returns:**
boolean - waarde die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Stelt een door de gebruiker gedefinieerde implementatie‑callback in die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | een door de gebruiker gedefinieerde implementatie‑callback die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Bepaalt of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out.

--------------------

Het gebruik van een gradient‑kwast wordt momenteel niet ondersteund voor het renderen naar SVG.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | waarde die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out. |

