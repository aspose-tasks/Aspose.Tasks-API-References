---
title: "FontResolveEventArgs"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Proporciona argumentos para la devolución de llamada que se invoca cuando la fuente se resuelve."
type: docs
weight: 99
url: /es/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Proporciona argumentos para la devolución de llamada que se invoca cuando la fuente se resuelve.
## Métodos

| Método | Descripción |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Obtiene el nombre de la fuente solicitada. |
| [getResolvedFontName()](#getResolvedFontName--) | Obtiene el nombre de la fuente resuelta. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Establece el nombre de la fuente resuelta. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Obtiene el nombre de la fuente solicitada.

**Returns:**
java.lang.String - el nombre de la fuente solicitada.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Obtiene el nombre de la fuente resuelta. Puede establecerse para controlar las fuentes usadas al renderizar una vista.

**Returns:**
java.lang.String - Nombre de la fuente solicitada si se encuentra la fuente o nombre de la fuente de reserva o null si no se puede encontrar la fuente.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Establece el nombre de la fuente resuelta. Puede establecerse para controlar las fuentes usadas al renderizar una vista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el nombre de la fuente resuelta. |

