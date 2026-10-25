---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リスト処理用のユーティリティクラスです。"
type: docs
weight: 147
url: /ja/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

リスト処理用のユーティリティクラスです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | 指定された位置から開始して、各リスト要素にアルゴリズムを適用します。 |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | 指定された条件でリスト要素をフィルタリングします。 |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | 指定された条件を満たすリスト要素の最初の出現を検索します。 |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


指定された位置から開始して、各リスト要素にアルゴリズムを適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 処理対象のリスト。 |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | 適用されたアルゴリズム。 |
| 開始インデックス | int | 開始要素の位置。 |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


指定された条件でリスト要素をフィルタリングします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 処理するリスト。 |
| cond | [ICondition](../../com.aspose.tasks/icondition) | 指定されたリストをフィルタリングするために使用される条件。 |

**Returns:**
java.util.List&lt;T&gt; - フィルタリングされたリスト。
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


指定された条件を満たすリスト要素の最初の出現を検索します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| list | java.util.List&lt;T&gt; | 処理するリスト。 |
| cond | [ICondition](../../com.aspose.tasks/icondition) | 指定されたリスト内の要素を検索するために使用される条件。 |
| clazz | java.lang.Class | 要素 T のクラス型。 |

**Returns:**
T - リスト要素または null。
