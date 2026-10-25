---
title: "PixelFormat"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Especifica el formato de los datos de color para cada píxel en la imagen."
type: docs
weight: 193
url: /es/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

Especifica el formato de los datos de color para cada píxel en la imagen.
## Campos

| Campo | Descripción |
| --- | --- |
| [Alpha](#Alpha) | Los datos de píxeles contienen valores alfa que no están premultiplicados. |
| [Canonical](#Canonical) | El formato de píxel predeterminado de 32 bits por píxel. |
| [DontCare](#DontCare) | No se especifica ningún formato de píxel. |
| [Extended](#Extended) | Reservado. |
| [Format16bppArgb1555](#Format16bppArgb1555) | El formato de píxel es de 16 bits por píxel. |
| [Format16bppGrayScale](#Format16bppGrayScale) | El formato de píxel es de 16 bits por píxel. |
| [Format16bppRgb555](#Format16bppRgb555) | Especifica que el formato es de 16 bits por píxel; se utilizan 5 bits para cada uno de los componentes rojo, verde y azul. |
| [Format16bppRgb565](#Format16bppRgb565) | Especifica que el formato es de 16 bits por píxel; se utilizan 5 bits para el componente rojo, 6 bits para el componente verde y 5 bits para el componente azul. |
| [Format1bppIndexed](#Format1bppIndexed) | Especifica que el formato de píxel es de 1 bit por píxel y que utiliza color indexado. |
| [Format24bppRgb](#Format24bppRgb) | Especifica que el formato es de 24 bits por píxel; se utilizan 8 bits para cada uno de los componentes rojo, verde y azul. |
| [Format32bppArgb](#Format32bppArgb) | Especifica que el formato es de 32 bits por píxel; se utilizan 8 bits para cada uno de los componentes alfa, rojo, verde y azul. |
| [Format32bppPArgb](#Format32bppPArgb) | Especifica que el formato es de 32 bits por píxel; se utilizan 8 bits para cada uno de los componentes alfa, rojo, verde y azul. |
| [Format32bppRgb](#Format32bppRgb) | Especifica que el formato es de 32 bits por píxel; se utilizan 8 bits para cada uno de los componentes rojo, verde y azul. |
| [Format48bppRgb](#Format48bppRgb) | Especifica que el formato es de 48 bits por píxel; se utilizan 16 bits para cada uno de los componentes rojo, verde y azul. |
| [Format4bppIndexed](#Format4bppIndexed) | Especifica que el formato es de 4 bits por píxel, indexado. |
| [Format64bppArgb](#Format64bppArgb) | Especifica que el formato es de 64 bits por píxel; se utilizan 16 bits para cada uno de los componentes alfa, rojo, verde y azul. |
| [Format64bppPArgb](#Format64bppPArgb) | Especifica que el formato es de 64 bits por píxel; se utilizan 16 bits para cada uno de los componentes alfa, rojo, verde y azul. |
| [Format8bppIndexed](#Format8bppIndexed) | Especifica que el formato es de 8 bits por píxel, indexado. |
| [Gdi](#Gdi) | Los datos de píxel contienen colores GDI. |
| [Indexed](#Indexed) | Los datos de píxel contienen valores indexados por color, lo que significa que los valores son un índice a los colores en la tabla de colores del sistema, en lugar de valores de color individuales. |
| [Max](#Max) | El valor máximo para esta enumeración. |
| [PAlpha](#PAlpha) | El formato de píxel contiene valores alfa premultiplicados. |
| [Undefined](#Undefined) | El formato de píxel no está definido. |
### Alpha {#Alpha}
```
public static final int Alpha
```


Los datos de píxeles contienen valores alfa que no están premultiplicados.

### Canonical {#Canonical}
```
public static final int Canonical
```


El formato de píxel predeterminado es de 32 bits por píxel. El formato especifica una profundidad de color de 24 bits y un canal alfa de 8 bits.

### DontCare {#DontCare}
```
public static final int DontCare
```


No se especifica ningún formato de píxel.

### Extended {#Extended}
```
public static final int Extended
```


Reservado.

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


El formato de píxel es de 16 bits por píxel. La información de color especifica 32.768 tonos de color, de los cuales 5 bits son rojo, 5 bits son verde, 5 bits son azul y 1 bit es alfa.

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


El formato de píxel es de 16 bits por píxel. La información de color especifica 65.536 tonos de gris.

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


Especifica que el formato es de 16 bits por píxel; se utilizan 5 bits para cada uno de los componentes rojo, verde y azul. El bit restante no se usa.

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


Especifica que el formato es de 16 bits por píxel; se utilizan 5 bits para el componente rojo, 6 bits para el componente verde y 5 bits para el componente azul.

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


Especifica que el formato de píxel es de 1 bit por píxel y que utiliza color indexado. Por lo tanto, la tabla de colores tiene dos colores.

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


Especifica que el formato es de 24 bits por píxel; se utilizan 8 bits para cada uno de los componentes rojo, verde y azul.

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


Especifica que el formato es de 32 bits por píxel; se utilizan 8 bits para cada uno de los componentes alfa, rojo, verde y azul.

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


Especifica que el formato es de 32 bits por píxel; se utilizan 8 bits para cada uno de los componentes alfa, rojo, verde y azul. Los componentes rojo, verde y azul están premultiplicados, según el componente alfa.

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


Especifica que el formato es de 32 bits por píxel; se utilizan 8 bits para cada uno de los componentes rojo, verde y azul. Los 8 bits restantes no se usan.

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


Especifica que el formato es de 48 bits por píxel; se utilizan 16 bits para cada uno de los componentes rojo, verde y azul.

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


Especifica que el formato es de 4 bits por píxel, indexado.

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


Especifica que el formato es de 64 bits por píxel; se utilizan 16 bits para cada uno de los componentes alfa, rojo, verde y azul.

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


Especifica que el formato es de 64 bits por píxel; 16 bits cada uno se utilizan para los componentes alfa, rojo, verde y azul. Los componentes rojo, verde y azul están premultiplicados según el componente alfa.

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


Especifica que el formato es de 8 bits por píxel, indexado. Por lo tanto, la tabla de colores contiene 256 colores.

### Gdi {#Gdi}
```
public static final int Gdi
```


Los datos de píxel contienen colores GDI.

### Indexed {#Indexed}
```
public static final int Indexed
```


Los datos de píxel contienen valores indexados por color, lo que significa que los valores son un índice a los colores en la tabla de colores del sistema, en lugar de valores de color individuales.

### Max {#Max}
```
public static final int Max
```


El valor máximo para esta enumeración.

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


El formato de píxel contiene valores alfa premultiplicados.

### Undefined {#Undefined}
```
public static final int Undefined
```


El formato de píxel no está definido.

