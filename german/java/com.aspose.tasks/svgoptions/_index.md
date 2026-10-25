---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu SVG."
type: docs
weight: 283
url: /de/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu SVG.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Initialisiert eine neue Instanz der [SvgOptions](../../com.aspose/tasks/svgoptions)-Klasse, die zum Speichern des Projekts im SVG-Format verwendet werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Ruft einen benutzerdefinierten Implementierungs-Callback ab, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Bestimmt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Legt einen benutzerdefinierten Implementierungs-Callback fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Bestimmt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Initialisiert eine neue Instanz der [SvgOptions](../../com.aspose/tasks/svgoptions)-Klasse, die zum Speichern des Projekts im SVG-Format verwendet werden kann.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Für den internen Gebrauch reserviert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


Für den internen Gebrauch reserviert.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Ruft einen benutzerdefinierten Implementierungs-Callback ab, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Bestimmt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll.

--------------------

Die Verwendung eines Farbverlaufspinsels wird derzeit für das Rendern nach SVG nicht unterstützt.

**Returns:**
boolescher Wert – gibt an, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Legt einen benutzerdefinierten Implementierungs-Callback fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | ein benutzerdefinierter Implementierungs-Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Bestimmt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll.

--------------------

Die Verwendung eines Farbverlaufspinsels wird derzeit für das Rendern nach SVG nicht unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Wert, der angibt, ob beim Rendern des Projektlayouts ein Farbverlaufspinsel verwendet werden soll. |

