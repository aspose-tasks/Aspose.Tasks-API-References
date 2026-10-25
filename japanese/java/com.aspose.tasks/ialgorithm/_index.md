---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "T のオブジェクトのリストに適用できるアルゴリズムを表します。"
type: docs
weight: 375
url: /ja/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

`T` オブジェクトのリストに適用できるアルゴリズムを表します。

T : メソッドインターフェイスを適用するオブジェクトの型。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | リスト内のオブジェクトを処理します。 |
| [postAlg(T el, int index)](#postAlg-T-int-) | オブジェクトの処理後に呼び出されます。 |
| [preAlg(T el, int index)](#preAlg-T-int-) | オブジェクトの処理前に呼び出されます。 |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


リスト内のオブジェクトを処理します。 [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-) の後に呼び出されます;

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理されたオブジェクト。 |
| インデックス | int | オブジェクトのインデックス。 |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


オブジェクトの処理後に呼び出されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理されたオブジェクト。 |
| インデックス | int | オブジェクトのインデックス。 |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


オブジェクトの処理前に呼び出されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理されたオブジェクト。 |
| インデックス | int | オブジェクトのインデックス。 |

