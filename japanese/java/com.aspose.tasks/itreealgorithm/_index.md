---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクト T のツリーに適用できるアルゴリズムを表します。"
type: docs
weight: 384
url: /ja/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

`T` オブジェクトのツリーに適用できるアルゴリズムを表します。

T : メソッドインターフェイスを適用するオブジェクトの型。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | ツリーのノードを処理します。 |
| [postAlg(T el, int level)](#postAlg-T-int-) | ツリーのノードを処理した後に呼び出されます。 |
| [preAlg(T el, int level)](#preAlg-T-int-) | ツリーのノードを処理する前に呼び出されます。 |
### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


ツリーのノードを処理します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理するノード。 |
| レベル | int | ツリーノードのレベル。 |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int level)
```


ツリーのノードを処理した後に呼び出されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理するノード。 |
| レベル | int | ツリーノードのレベル。 |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


ツリーのノードを処理する前に呼び出されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理するノード。 |
| レベル | int | ツリーノードのレベル。 |

