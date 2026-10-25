---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ファイルまたはストリームからプロジェクトをロードする際に追加のロードパラメータを指定できます。"
type: docs
weight: 148
url: /ja/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

ファイルまたはストリームからプロジェクトをロードする際に追加のロードパラメータを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | 新しい [LoadOptions](../../com.aspose/tasks/loadoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | プロジェクトのロード操作をキャンセルするために使用できるトークンを取得します。 |
| [getEncoding()](#getEncoding--) | HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み取る際に使用されるエンコーディングを取得します。 |
| [getErrorHandler()](#getErrorHandler--) | XML パースエラーを処理するコールバックメソッドを取得します。 |
| [getPassword()](#getPassword--) | 保護パスワードを取得します。 |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Primavera 形式（Primavera P6 XER または Primavera P6 Xml）のロード動作をカスタマイズできる、[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスの指定インスタンスを取得します。 |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | プロジェクトのロード操作をキャンセルするために使用できるトークンを設定します。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み取る際に使用されるエンコーディングを設定します。 |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | XML パースエラーを処理するコールバックメソッドを設定します。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 保護パスワードを設定します。 |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Primavera 形式（Primavera P6 XER または Primavera P6 Xml）のロード動作をカスタマイズできる、[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスの指定インスタンスを設定します。 |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


新しい [LoadOptions](../../com.aspose/tasks/loadoptions) クラスのインスタンスを初期化します。

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


プロジェクトのロード操作をキャンセルするために使用できるトークンを取得します。

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み取る際に使用されるエンコーディングを取得します。デフォルトのエンコーディングは UTF8 です。

**Returns:**
java.nio.charset.Charset - HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み取る際に使用されるエンコーディングです。
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


XML パースエラーを処理するコールバックメソッドを取得します。

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


保護パスワードを取得します。

**Returns:**
java.lang.String - 保護パスワードです。
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Primavera 形式（Primavera P6 XER または Primavera P6 Xml）のロード動作をカスタマイズできる、[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスの指定インスタンスを取得します。

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


プロジェクトのロード操作をキャンセルするために使用できるトークンを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | プロジェクトのロード操作をキャンセルするために使用できるトークンです。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み取る際に使用されるエンコーディングを設定します。デフォルトのエンコーディングは UTF8 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.nio.charset.Charset | HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み取る際に使用されるエンコーディング。 |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


XML パースエラーを処理するコールバックメソッドを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML パースエラーを処理するコールバックメソッドです。 |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


保護パスワードを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 保護パスワードです。 |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Primavera 形式（Primavera P6 XER または Primavera P6 Xml）のロード動作をカスタマイズできる、[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスの指定インスタンスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスの指定インスタンスで、Primavera 形式（Primavera P6 XER または Primavera P6 Xml）のロード動作をカスタマイズできます。 |

