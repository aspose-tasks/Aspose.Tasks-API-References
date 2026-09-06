---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillhandahåller argument för återuppringningen som anropas när teckensnittet har lösts."
type: docs
weight: 99
url: /sv/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Tillhandahåller argument för återuppringningen som anropas när teckensnittet har lösts.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Hämtar namnet på det begärda teckensnittet. |
| [getResolvedFontName()](#getResolvedFontName--) | Hämtar namnet på det upplösta teckensnittet. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Ställer in namnet på det upplösta teckensnittet. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Hämtar namnet på det begärda teckensnittet.

**Returns:**
java.lang.String - namnet på det begärda teckensnittet.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Hämtar namnet på det upplösta teckensnittet. Kan ställas in för att kontrollera vilka teckensnitt som används för att rendera en vy.

**Returns:**
java.lang.String - Namnet på det begärda teckensnittet om teckensnittet hittas eller namnet på reservteckensnittet, eller null om teckensnittet inte kan hittas.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Ställer in namnet på det upplösta teckensnittet. Kan ställas in för att kontrollera vilka teckensnitt som används för att rendera en vy.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | namnet på det upplösta teckensnittet. |

