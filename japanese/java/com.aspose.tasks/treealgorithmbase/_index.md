---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ITreeAlgorithmltTgt の実装のための基底クラス。"
type: docs
weight: 327
url: /ja/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

ITreeAlgorithm&lt;T&gt; の実装のための基底クラスです。

T : 要素の型。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | ツリーのノードを処理します。 |
| [postAlg(T el, int level)](#postAlg-T-int-) | ツリーのノードを処理した後に呼び出されます。 |
| [preAlg(T el, int level)](#preAlg-T-int-) | ツリーのノードを処理する前に呼び出されます。 |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


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
public void postAlg(T el, int level)
```


ツリーのノードを処理した後に呼び出されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理するノード。 |
| レベル | int | ツリーノードのレベル。 |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


ツリーのノードを処理する前に呼び出されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | 処理するノード。 |
| レベル | int | ツリーノードのレベル。 |

