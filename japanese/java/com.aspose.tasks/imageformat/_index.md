---
title: "ImageFormat"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "画像のファイル形式を指定します。"
type: docs
weight: 133
url: /ja/java/com.aspose.tasks/imageformat/
---

**Inheritance:**
java.lang.Object
```
public final class ImageFormat
```

画像のファイル形式を指定します。拡張できません。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ImageFormat(String guid)](#ImageFormat-java.lang.String-) | 指定された Guid 文字列を使用して ImageFormat クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [equals(Object o)](#equals-java.lang.Object-) | 指定されたオブジェクトがこの ImageFormat オブジェクトと等価な ImageFormat オブジェクトかどうかを示す値を返します。 |
| [getBmp()](#getBmp--) | ビットマップ (BMP) 画像形式を取得します。 |
| [getEmf()](#getEmf--) | 拡張メタファイル (EMF) 画像形式を取得します。 |
| [getExif()](#getExif--) | 交換可能画像ファイル (Exif) 形式を取得します。 |
| [getGif()](#getGif--) | Graphics Interchange Format (GIF) 画像形式を取得します。 |
| [getGuid()](#getGuid--) | この ImageFormat オブジェクトを表す Guid 文字列を取得します。 |
| [getIcon()](#getIcon--) | Windows アイコン画像形式を取得します。 |
| [getJpeg()](#getJpeg--) | Joint Photographic Experts Group (JPEG) 画像形式を取得します。 |
| [getMemoryBmp()](#getMemoryBmp--) | メモリ内のビットマップの形式を取得します。 |
| [getPng()](#getPng--) | W3C Portable Network Graphics (PNG) 画像形式を取得します。 |
| [getTiff()](#getTiff--) | Tagged Image File Format (TIFF) 画像形式を取得します。 |
| [getWmf()](#getWmf--) | Windows メタファイル (WMF) 画像形式を取得します。 |
| [hashCode()](#hashCode--) | このオブジェクトを表すハッシュコード値を返します。 |
| [isBitmapType()](#isBitmapType--) | 画像形式がビットマップ型かどうかを判定します。 |
| [isMetafileType()](#isMetafileType--) | 画像形式がメタファイル型かどうかを判定します。 |
| [isUnknownType()](#isUnknownType--) | 画像形式が不明な型かどうかを判定します。 |
| [toString()](#toString--) | この ImageFormat オブジェクトを人間が読める文字列に変換します。 |
### ImageFormat(String guid) {#ImageFormat-java.lang.String-}
```
public ImageFormat(String guid)
```


指定された Guid 文字列を使用して ImageFormat クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| guid | java.lang.String | 特定の画像形式を指定する Guid 文字列です。 |

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


指定されたオブジェクトがこの ImageFormat オブジェクトと等価な ImageFormat オブジェクトかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object | テスト対象のオブジェクトです。 |

**Returns:**
boolean - o がこの ImageFormat オブジェクトと等価な ImageFormat オブジェクトである場合は true、そうでない場合は false。
### getBmp() {#getBmp--}
```
public static ImageFormat getBmp()
```


ビットマップ (BMP) 画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the bitmap image format.
### getEmf() {#getEmf--}
```
public static ImageFormat getEmf()
```


拡張メタファイル (EMF) 画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the enhanced metafile image format.
### getExif() {#getExif--}
```
public static ImageFormat getExif()
```


交換可能画像ファイル (Exif) 形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Exif format.
### getGif() {#getGif--}
```
public static ImageFormat getGif()
```


Graphics Interchange Format (GIF) 画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the GIF image format.
### getGuid() {#getGuid--}
```
public String getGuid()
```


この ImageFormat オブジェクトを表す Guid 文字列を取得します。

**Returns:**
java.lang.String - この ImageFormat オブジェクトを表す Guid 文字列。
### getIcon() {#getIcon--}
```
public static ImageFormat getIcon()
```


Windows アイコン画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows icon image format.
### getJpeg() {#getJpeg--}
```
public static ImageFormat getJpeg()
```


Joint Photographic Experts Group (JPEG) 画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the JPEG image format.
### getMemoryBmp() {#getMemoryBmp--}
```
public static ImageFormat getMemoryBmp()
```


メモリ内のビットマップの形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the format of a bitmap in memory.
### getPng() {#getPng--}
```
public static ImageFormat getPng()
```


W3C Portable Network Graphics (PNG) 画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the PNG image format.
### getTiff() {#getTiff--}
```
public static ImageFormat getTiff()
```


Tagged Image File Format (TIFF) 画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the TIFF image format.
### getWmf() {#getWmf--}
```
public static ImageFormat getWmf()
```


Windows メタファイル (WMF) 画像形式を取得します。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows metafile image format.
### hashCode() {#hashCode--}
```
public int hashCode()
```


このオブジェクトを表すハッシュコード値を返します。

**Returns:**
int - このオブジェクトを表すハッシュコード。
### isBitmapType() {#isBitmapType--}
```
public boolean isBitmapType()
```


画像形式がビットマップ型かどうかを判定します。

**Returns:**
boolean - 画像形式がビットマップタイプである場合は true、そうでない場合は false。
### isMetafileType() {#isMetafileType--}
```
public boolean isMetafileType()
```


画像形式がメタファイル型かどうかを判定します。

**Returns:**
boolean - 画像形式がメタファイルタイプである場合は true、そうでない場合は false。
### isUnknownType() {#isUnknownType--}
```
public boolean isUnknownType()
```


画像形式が不明な型かどうかを判定します。

**Returns:**
boolean - 画像形式が不明なタイプである場合は true、そうでない場合は false。
### toString() {#toString--}
```
public String toString()
```


この ImageFormat オブジェクトを人間が読める文字列に変換します。

**Returns:**
java.lang.String - この ImageFormat オブジェクトを表す文字列。
