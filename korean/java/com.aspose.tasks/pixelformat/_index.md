---
title: "PixelFormat"
second_title: "Aspose.Tasks for Java API Reference"
description: "이미지의 각 픽셀에 대한 색상 데이터 형식을 지정합니다."
type: docs
weight: 193
url: /ko/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

이미지의 각 픽셀에 대한 색상 데이터 형식을 지정합니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [Alpha](#Alpha) | 픽셀 데이터에 사전 곱셈되지 않은 알파 값이 포함되어 있습니다. |
| [Canonical](#Canonical) | 픽셀당 32비트의 기본 픽셀 형식입니다. |
| [DontCare](#DontCare) | 픽셀 형식이 지정되지 않았습니다. |
| [Extended](#Extended) | 예약됨. |
| [Format16bppArgb1555](#Format16bppArgb1555) | 픽셀당 16비트의 픽셀 형식입니다. |
| [Format16bppGrayScale](#Format16bppGrayScale) | 픽셀당 16비트의 픽셀 형식입니다. |
| [Format16bppRgb555](#Format16bppRgb555) | 형식이 픽셀당 16비트이며, 빨강, 초록, 파랑 구성 요소 각각에 5비트가 사용된다고 지정합니다. |
| [Format16bppRgb565](#Format16bppRgb565) | 형식이 픽셀당 16비트이며, 빨강 구성 요소에 5비트, 초록 구성 요소에 6비트, 파랑 구성 요소에 5비트가 사용된다고 지정합니다. |
| [Format1bppIndexed](#Format1bppIndexed) | 픽셀당 1비트의 픽셀 형식이며 인덱스 색상을 사용한다고 지정합니다. |
| [Format24bppRgb](#Format24bppRgb) | 형식이 픽셀당 24비트이며, 빨강, 초록, 파랑 구성 요소 각각에 8비트가 사용된다고 지정합니다. |
| [Format32bppArgb](#Format32bppArgb) | 형식이 픽셀당 32비트이며, 알파, 빨강, 초록, 파랑 구성 요소 각각에 8비트가 사용된다고 지정합니다. |
| [Format32bppPArgb](#Format32bppPArgb) | 형식이 픽셀당 32비트이며, 알파, 빨강, 초록, 파랑 구성 요소 각각에 8비트가 사용된다고 지정합니다. |
| [Format32bppRgb](#Format32bppRgb) | 형식이 픽셀당 32비트이며, 빨강, 초록, 파랑 구성 요소 각각에 8비트가 사용된다고 지정합니다. |
| [Format48bppRgb](#Format48bppRgb) | 포맷이 픽셀당 48비트임을 지정합니다; 각각 16비트가 빨강, 초록 및 파랑 구성 요소에 사용됩니다. |
| [Format4bppIndexed](#Format4bppIndexed) | 포맷이 픽셀당 4비트이며 인덱스됨을 지정합니다. |
| [Format64bppArgb](#Format64bppArgb) | 포맷이 픽셀당 64비트임을 지정합니다; 각각 16비트가 알파, 빨강, 초록 및 파랑 구성 요소에 사용됩니다. |
| [Format64bppPArgb](#Format64bppPArgb) | 포맷이 픽셀당 64비트임을 지정합니다; 각각 16비트가 알파, 빨강, 초록 및 파랑 구성 요소에 사용됩니다. |
| [Format8bppIndexed](#Format8bppIndexed) | 포맷이 픽셀당 8비트이며 인덱스됨을 지정합니다. |
| [Gdi](#Gdi) | 픽셀 데이터에 GDI 색상이 포함되어 있습니다. |
| [Indexed](#Indexed) | 픽셀 데이터에 색상 인덱스 값이 포함되어 있으며, 이는 값이 개별 색상 값이 아니라 시스템 색상 테이블의 색상에 대한 인덱스임을 의미합니다. |
| [Max](#Max) | 이 열거형의 최대값입니다. |
| [PAlpha](#PAlpha) | 픽셀 포맷에 사전 곱해진 알파 값이 포함되어 있습니다. |
| [Undefined](#Undefined) | 픽셀 포맷이 정의되지 않았습니다. |
### Alpha {#Alpha}
```
public static final int Alpha
```


픽셀 데이터에 사전 곱셈되지 않은 알파 값이 포함되어 있습니다.

### Canonical {#Canonical}
```
public static final int Canonical
```


픽셀당 32비트인 기본 픽셀 포맷입니다. 이 포맷은 24비트 색상 깊이와 8비트 알파 채널을 지정합니다.

### DontCare {#DontCare}
```
public static final int DontCare
```


픽셀 형식이 지정되지 않았습니다.

### Extended {#Extended}
```
public static final int Extended
```


예약됨.

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


픽셀 포맷은 픽셀당 16비트입니다. 색상 정보는 32,768가지 색조를 지정하며, 그 중 5비트는 빨강, 5비트는 초록, 5비트는 파랑, 1비트는 알파입니다.

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


픽셀 포맷은 픽셀당 16비트이며, 색상 정보는 65,536가지 회색 음영을 지정합니다.

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


포맷이 픽셀당 16비트이며, 각각 5비트가 빨강, 초록 및 파랑 구성 요소에 사용됩니다. 남은 1비트는 사용되지 않습니다.

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


형식이 픽셀당 16비트이며, 빨강 구성 요소에 5비트, 초록 구성 요소에 6비트, 파랑 구성 요소에 5비트가 사용된다고 지정합니다.

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


픽셀 포맷이 픽셀당 1비트이며 인덱스 색상을 사용함을 지정합니다. 따라서 색상 테이블에는 두 가지 색상이 포함됩니다.

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


형식이 픽셀당 24비트이며, 빨강, 초록, 파랑 구성 요소 각각에 8비트가 사용된다고 지정합니다.

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


형식이 픽셀당 32비트이며, 알파, 빨강, 초록, 파랑 구성 요소 각각에 8비트가 사용된다고 지정합니다.

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


포맷이 픽셀당 32비트이며, 각각 8비트가 알파, 빨강, 초록 및 파랑 구성 요소에 사용됩니다. 빨강, 초록, 파랑 구성 요소는 알파 구성 요소에 따라 사전 곱해집니다.

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


포맷이 픽셀당 32비트이며, 각각 8비트가 빨강, 초록 및 파랑 구성 요소에 사용됩니다. 남은 8비트는 사용되지 않습니다.

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


포맷이 픽셀당 48비트임을 지정합니다; 각각 16비트가 빨강, 초록 및 파랑 구성 요소에 사용됩니다.

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


포맷이 픽셀당 4비트이며 인덱스됨을 지정합니다.

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


포맷이 픽셀당 64비트임을 지정합니다; 각각 16비트가 알파, 빨강, 초록 및 파랑 구성 요소에 사용됩니다.

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


포맷이 픽셀당 64비트이며, 각각 16비트가 알파, 빨강, 초록 및 파랑 구성 요소에 사용됩니다. 빨강, 초록, 파랑 구성 요소는 알파 구성 요소에 따라 사전 곱해집니다.

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


포맷이 픽셀당 8비트이며 인덱스됨을 지정합니다. 따라서 색상 테이블에는 256가지 색상이 포함됩니다.

### Gdi {#Gdi}
```
public static final int Gdi
```


픽셀 데이터에 GDI 색상이 포함되어 있습니다.

### Indexed {#Indexed}
```
public static final int Indexed
```


픽셀 데이터에 색상 인덱스 값이 포함되어 있으며, 이는 값이 개별 색상 값이 아니라 시스템 색상 테이블의 색상에 대한 인덱스임을 의미합니다.

### Max {#Max}
```
public static final int Max
```


이 열거형의 최대값입니다.

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


픽셀 포맷에 사전 곱해진 알파 값이 포함되어 있습니다.

### Undefined {#Undefined}
```
public static final int Undefined
```


픽셀 포맷이 정의되지 않았습니다.

