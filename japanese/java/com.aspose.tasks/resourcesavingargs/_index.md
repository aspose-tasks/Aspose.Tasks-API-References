---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "このクラスは、HTML 形式への変換中に発生する外部リソースファイルの保存に関連するデータのセットを表します。"
type: docs
weight: 254
url: /ja/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

このクラスは、HTML 形式への変換中に発生する外部リソースファイルの保存に関連するデータの集合を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | KeepStreamOpen が false の場合はストリームを閉じ、そうでなければフラッシュします。 |
| [getFileName()](#getFileName--) | コンバータからカスタムメソッドのコードへ渡されると想定されるファイル名を取得します。 |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | リソースの保存が完了した後にストリームが開いたままになるかどうかを示す値を取得します。 |
| [getStream()](#getStream--) | 保存されたファイルのバイナリ コンテンツを取得します。 |
| [getUri()](#getUri--) | リソース URI を取得します。 |
| [setFileName(String value)](#setFileName-java.lang.String-) | コンバータからカスタム メソッドのコードへ渡される想定ファイル名を設定します。 |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | リソースの保存が完了した後にストリームを開いたままにするかどうかを示す値を設定します。 |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | 保存されたファイルのバイナリ コンテンツを設定します。 |
| [setUri(String value)](#setUri-java.lang.String-) | リソース URI を設定します。 |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


KeepStreamOpen が false の場合はストリームを閉じ、そうでなければフラッシュします。

### getFileName() {#getFileName--}
```
public final String getFileName()
```


コンバータからカスタム メソッドのコードへ渡される想定ファイル名を取得します。カスタム コードでこのファイルの処理方法や保存場所を決定する際に使用できます。

**Returns:**
java.lang.String - コンバータからカスタム メソッドのコードへ渡される想定ファイル名。
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


リソースの保存が完了した後にストリームが開いたままになるかどうかを示す値を取得します。

**Returns:**
boolean - リソースの保存が完了した後にストリームを開いたままにするかどうかを示す値。
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


保存されたファイルのバイナリ コンテンツを取得します。

**Returns:**
java.io.OutputStream - 保存されたファイルのバイナリ コンテンツ。
### getUri() {#getUri--}
```
public final String getUri()
```


リソース URI を取得します。

**Returns:**
java.lang.String - リソース URI。
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


コンバータからカスタム メソッドのコードへ渡される想定ファイル名を設定します。カスタム コードでこのファイルの処理方法や保存場所を決定する際に使用できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | コンバータからカスタム メソッドのコードへ渡される想定ファイル名。 |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


リソースの保存が完了した後にストリームを開いたままにするかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | リソースの保存が完了した後にストリームを開いたままにするかどうかを示す値。 |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


保存されたファイルのバイナリ コンテンツを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.io.OutputStream | 保存されたファイルのバイナリ コンテンツ。 |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


リソース URI を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | リソース URI。 |

