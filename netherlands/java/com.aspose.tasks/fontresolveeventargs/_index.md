---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Biedt argumenten voor de callback die wordt aangeroepen wanneer het lettertype is opgelost."
type: docs
weight: 99
url: /nl/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Biedt argumenten voor de callback die wordt aangeroepen wanneer het lettertype is opgelost.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Haalt de naam van het aangevraagde lettertype op. |
| [getResolvedFontName()](#getResolvedFontName--) | Haalt de naam van het opgeloste lettertype op. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Stelt de naam van het opgeloste lettertype in. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Haalt de naam van het aangevraagde lettertype op.

**Returns:**
java.lang.String - de naam van het aangevraagde lettertype.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Haalt de naam van het opgeloste lettertype op. Kan worden ingesteld om de lettertypen te regelen die worden gebruikt om een weergave te renderen.

**Returns:**
java.lang.String - Naam van het aangevraagde lettertype als het lettertype wordt gevonden of naam van het fallback-lettertype of null als het lettertype niet kan worden gevonden.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Stelt de naam van het opgeloste lettertype in. Kan worden ingesteld om de lettertypen te regelen die worden gebruikt om een weergave te renderen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de naam van het opgeloste lettertype. |

