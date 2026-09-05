---
title: "ArrayUtils"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ArrayList 処理用ユーティリティクラスです。"
type: docs
weight: 14
url: /ja/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

ArrayList 処理用ユーティリティクラスです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | 指定された位置から開始して、各 List 要素にアルゴリズムを適用します。 |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | 指定された条件で ArrayList 要素をフィルタリングします。 |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | 指定された条件を満たすArrayList要素の最初の出現を検索します。 |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| 配列 | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


指定された位置から開始して、各 List 要素にアルゴリズムを適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 配列 | java.util.List | 処理対象のArrayList。 |
| アルゴリズム | com.aspose.tasks.IAlgorithm | 適用されたアルゴリズム。 |
| 開始インデックス | int | 開始要素の位置。 |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


指定された条件で ArrayList 要素をフィルタリングします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 配列 | java.util.List | 処理対象のリスト。 |
| cond | com.aspose.tasks.ICondition | リストをフィルタリングするために使用される条件。 |

**Returns:**
java.util.List - フィルタ済みリスト。
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


指定された条件を満たすArrayList要素の最初の出現を検索します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 配列 | java.util.List | 処理対象のArrayList。 |
| cond | com.aspose.tasks.ICondition | ArrayList要素を検索するために使用される条件。 |

**Returns:**
java.lang.Object - リスト要素またはnull。
