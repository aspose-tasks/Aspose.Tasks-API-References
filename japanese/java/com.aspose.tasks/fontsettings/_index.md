---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトビューをレンダリングする際に使用されるフォント設定を指定します。"
type: docs
weight: 101
url: /ja/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | レンダリングに使用されるデフォルト（またはフォールバック）フォントを取得します。 |
| [getFontResolveCallback()](#getFontResolveCallback--) | 解決されたフォントをカスタマイズできるコールバックを取得します。 |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | レンダリングにデフォルトフォントを使用すべきかどうかを示す値を取得します。 |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | レンダリングに使用するデフォルト（またはフォールバック）フォントを設定します。 |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | プロジェクトのビューをレンダリングする際に Aspose.Tasks が TrueType フォントを検索するフォルダーを設定します。 |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | 解決されたフォントをカスタマイズできるコールバックを設定します。 |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | レンダリングにデフォルトフォントを使用すべきかどうかを示す値を設定します。 |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


レンダリングに使用されるデフォルト（またはフォールバック）フォントを取得します。

**Returns:**
java.lang.String - レンダリングに使用されるデフォルト（またはフォールバック）フォントです。
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


解決されたフォントをカスタマイズできるコールバックを取得します。

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


レンダリングにデフォルトフォントを使用すべきかどうかを示す値を取得します。

--------------------

値が False で DefaultFontName が指定されている場合、レンダリングエンジンは DefaultFontName で指定されたフォントをフォールバックフォントとして使用します。そうでない場合は、'Arial'（インストールされている場合）または 'Generic Sans Serif' フォントがフォールバックフォントとして使用されます。フォールバックフォントは、テキストスタイルが現在のオペレーティングシステムにインストールされていないフォントを参照している場合に、プロジェクトビューのレンダリング中に使用されます。フォント解決をより細かく制御するには、`FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) コールバックを使用できます。

**Returns:**
boolean - レンダリングにデフォルトフォントを使用すべきかどうかを示す値です。
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


レンダリングに使用するデフォルト（またはフォールバック）フォントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | レンダリングに使用されるデフォルト（またはフォールバック）フォントです。 |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


プロジェクトのビューをレンダリングする際に Aspose.Tasks が TrueType フォントを検索するフォルダーを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType フォントを含むフォルダーの配列です。 |
| recursive | boolean | true の場合、指定されたフォルダーは再帰的にスキャンされます。 |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


解決されたフォントをカスタマイズできるコールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | 解決されたフォントをカスタマイズできるコールバックです。 |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


レンダリングにデフォルトフォントを使用すべきかどうかを示す値を設定します。

--------------------

値が False で DefaultFontName が指定されている場合、レンダリングエンジンは DefaultFontName で指定されたフォントをフォールバックフォントとして使用します。そうでない場合は、'Arial'（インストールされている場合）または 'Generic Sans Serif' フォントがフォールバックフォントとして使用されます。フォールバックフォントは、テキストスタイルが現在のオペレーティングシステムにインストールされていないフォントを参照している場合に、プロジェクトビューのレンダリング中に使用されます。フォント解決をより細かく制御するには、`FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) コールバックを使用できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | デフォルトフォントをレンダリングに使用すべきかどうかを示す値。 |

