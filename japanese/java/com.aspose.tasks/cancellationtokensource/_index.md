---
title: "CancellationTokenSource"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "CancellationToken にキャンセルすべきであることをシグナルします。"
type: docs
weight: 47
url: /ja/java/com.aspose.tasks/cancellationtokensource/
---

**Inheritance:**
java.lang.Object
```
public class CancellationTokenSource
```

`CancellationToken` にキャンセルすべきであることを通知します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [CancellationTokenSource()](#CancellationTokenSource--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [cancel()](#cancel--) | キャンセル要求を伝えます。 |
| [getToken()](#getToken--) | この `CancellationTokenSource` に関連付けられた新しい `CancellationToken` を作成します。 |
| [isCancellationRequested()](#isCancellationRequested--) | この CancellationTokenSource に対してキャンセルが要求されたかどうかを取得します。 |
### CancellationTokenSource() {#CancellationTokenSource--}
```
public CancellationTokenSource()
```


### cancel() {#cancel--}
```
public void cancel()
```


キャンセル要求を伝えます。

### getToken() {#getToken--}
```
public CancellationToken getToken()
```


この `CancellationTokenSource` に関連付けられた新しい `CancellationToken` を作成します。

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token associated with this `CancellationTokenSource`.
### isCancellationRequested() {#isCancellationRequested--}
```
public boolean isCancellationRequested()
```


この CancellationTokenSource に対してキャンセルが要求されたかどうかを取得します。

**Returns:**
boolean - キャンセルが要求された場合は true、そうでない場合は false。
