---
title: "PixelFormat"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "画像内の各ピクセルのカラー データ形式を指定します。"
type: docs
weight: 193
url: /ja/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

画像内の各ピクセルのカラー データ形式を指定します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [Alpha](#Alpha) | ピクセルデータには、事前乗算されていないアルファ値が含まれています。 |
| [Canonical](#Canonical) | 1 ピクセルあたり 32 ビットのデフォルトピクセルフォーマット。 |
| [DontCare](#DontCare) | ピクセルフォーマットは指定されていません。 |
| [Extended](#Extended) | 予約済み。 |
| [Format16bppArgb1555](#Format16bppArgb1555) | ピクセルフォーマットは 1 ピクセルあたり 16 ビットです。 |
| [Format16bppGrayScale](#Format16bppGrayScale) | ピクセルフォーマットは 1 ピクセルあたり 16 ビットです。 |
| [Format16bppRgb555](#Format16bppRgb555) | フォーマットが 1 ピクセルあたり 16 ビットであることを指定します。赤、緑、青の各コンポーネントに 5 ビットずつ使用されます。 |
| [Format16bppRgb565](#Format16bppRgb565) | フォーマットが 1 ピクセルあたり 16 ビットであることを指定します。赤コンポーネントに 5 ビット、緑コンポーネントに 6 ビット、青コンポーネントに 5 ビットが使用されます。 |
| [Format1bppIndexed](#Format1bppIndexed) | ピクセルフォーマットが 1 ピクセルあたり 1 ビットで、インデックスカラーを使用することを指定します。 |
| [Format24bppRgb](#Format24bppRgb) | フォーマットが 1 ピクセルあたり 24 ビットであることを指定します。赤、緑、青の各コンポーネントに 8 ビットずつ使用されます。 |
| [Format32bppArgb](#Format32bppArgb) | フォーマットが 1 ピクセルあたり 32 ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに 8 ビットずつ使用されます。 |
| [Format32bppPArgb](#Format32bppPArgb) | フォーマットが 1 ピクセルあたり 32 ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに 8 ビットずつ使用されます。 |
| [Format32bppRgb](#Format32bppRgb) | フォーマットが 1 ピクセルあたり 32 ビットであることを指定します。赤、緑、青の各コンポーネントに 8 ビットずつ使用されます。 |
| [Format48bppRgb](#Format48bppRgb) | フォーマットがピクセルあたり48ビットであることを指定します。赤、緑、青の各コンポーネントに16ビットずつ使用されます。 |
| [Format4bppIndexed](#Format4bppIndexed) | フォーマットがピクセルあたり4ビットで、インデックス方式であることを指定します。 |
| [Format64bppArgb](#Format64bppArgb) | フォーマットがピクセルあたり64ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに16ビットずつ使用されます。 |
| [Format64bppPArgb](#Format64bppPArgb) | フォーマットがピクセルあたり64ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに16ビットずつ使用されます。 |
| [Format8bppIndexed](#Format8bppIndexed) | フォーマットがピクセルあたり8ビットで、インデックス方式であることを指定します。 |
| [Gdi](#Gdi) | ピクセルデータにはGDIカラーが含まれています。 |
| [Indexed](#Indexed) | ピクセルデータにはカラーインデックス値が含まれます。これは、個々のカラー値ではなく、システムカラー表の色へのインデックスであることを意味します。 |
| [Max](#Max) | この列挙体の最大値です。 |
| [PAlpha](#PAlpha) | ピクセルフォーマットには事前乗算されたアルファ値が含まれています。 |
| [Undefined](#Undefined) | ピクセルフォーマットは未定義です。 |
### Alpha {#Alpha}
```
public static final int Alpha
```


ピクセルデータには、事前乗算されていないアルファ値が含まれています。

### Canonical {#Canonical}
```
public static final int Canonical
```


デフォルトのピクセルフォーマットはピクセルあたり32ビットです。このフォーマットは24ビットのカラー深度と8ビットのアルファチャンネルを指定します。

### DontCare {#DontCare}
```
public static final int DontCare
```


ピクセルフォーマットは指定されていません。

### Extended {#Extended}
```
public static final int Extended
```


予約済み。

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


ピクセルフォーマットはピクセルあたり16ビットです。カラー情報は32,768色の階調を指定し、そのうち5ビットが赤、5ビットが緑、5ビットが青、1ビットがアルファです。

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


ピクセルフォーマットはピクセルあたり16ビットです。カラー情報は65,536階調のグレイを指定します。

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


フォーマットがピクセルあたり16ビットであることを指定します。赤、緑、青の各コンポーネントに5ビットずつ使用され、残りの1ビットは使用されません。

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


フォーマットが 1 ピクセルあたり 16 ビットであることを指定します。赤コンポーネントに 5 ビット、緑コンポーネントに 6 ビット、青コンポーネントに 5 ビットが使用されます。

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


ピクセルフォーマットがピクセルあたり1ビットで、インデックスカラーを使用することを指定します。そのため、カラーテーブルには2色が含まれます。

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


フォーマットが 1 ピクセルあたり 24 ビットであることを指定します。赤、緑、青の各コンポーネントに 8 ビットずつ使用されます。

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


フォーマットが 1 ピクセルあたり 32 ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに 8 ビットずつ使用されます。

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


フォーマットがピクセルあたり32ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに8ビットずつ使用され、赤、緑、青のコンポーネントはアルファコンポーネントに従って事前乗算されます。

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


フォーマットがピクセルあたり32ビットであることを指定します。赤、緑、青の各コンポーネントに8ビットずつ使用され、残りの8ビットは使用されません。

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


フォーマットがピクセルあたり48ビットであることを指定します。赤、緑、青の各コンポーネントに16ビットずつ使用されます。

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


フォーマットがピクセルあたり4ビットで、インデックス方式であることを指定します。

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


フォーマットがピクセルあたり64ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに16ビットずつ使用されます。

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


フォーマットがピクセルあたり64ビットであることを指定します。アルファ、赤、緑、青の各コンポーネントに16ビットずつ使用され、赤、緑、青のコンポーネントはアルファコンポーネントに従って事前乗算されます。

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


フォーマットがピクセルあたり8ビットで、インデックス方式であることを指定します。そのため、カラーテーブルには256色が含まれます。

### Gdi {#Gdi}
```
public static final int Gdi
```


ピクセルデータにはGDIカラーが含まれています。

### Indexed {#Indexed}
```
public static final int Indexed
```


ピクセルデータにはカラーインデックス値が含まれます。これは、個々のカラー値ではなく、システムカラー表の色へのインデックスであることを意味します。

### Max {#Max}
```
public static final int Max
```


この列挙体の最大値です。

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


ピクセルフォーマットには事前乗算されたアルファ値が含まれています。

### Undefined {#Undefined}
```
public static final int Undefined
```


ピクセルフォーマットは未定義です。

