---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Argumente für den Callback bereit, der aufgerufen wird, wenn die Schrift aufgelöst wird."
type: docs
weight: 99
url: /de/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Stellt Argumente für den Callback bereit, der aufgerufen wird, wenn die Schrift aufgelöst wird.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Ermittelt den Namen der angeforderten Schriftart. |
| [getResolvedFontName()](#getResolvedFontName--) | Ruft den Namen der aufgelösten Schriftart ab. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Legt den Namen der aufgelösten Schriftart fest. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Ermittelt den Namen der angeforderten Schriftart.

**Returns:**
java.lang.String - der Name der angeforderten Schriftart.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Ruft den Namen der aufgelösten Schriftart ab. Kann festgelegt werden, um die zum Rendern einer Ansicht verwendeten Schriftarten zu steuern.

**Returns:**
java.lang.String - Name der angeforderten Schriftart, falls die Schriftart gefunden wird, oder Name der Ersatzschriftart bzw. null, wenn die Schriftart nicht gefunden werden kann.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Legt den Namen der aufgelösten Schriftart fest. Kann festgelegt werden, um die zum Rendern einer Ansicht verwendeten Schriftarten zu steuern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der Name der aufgelösten Schriftart. |

