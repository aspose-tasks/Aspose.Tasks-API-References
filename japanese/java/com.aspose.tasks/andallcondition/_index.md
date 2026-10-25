---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "すべての条件に論理 AND を適用します。"
type: docs
weight: 11
url: /ja/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

すべての条件に論理 AND を適用します。例: cond1 AND cond2 AND cond3...

T : メソッドインターフェイスを適用するオブジェクトの型。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | AndAllCondition&lt;T&gt; クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [check(T el)](#check-T-) | 指定されたオブジェクトが条件を満たす場合に true を返します。 |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


AndAllCondition&lt;T&gt; クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 条件 | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | 条件のリストです。 |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


指定されたオブジェクトが条件を満たす場合に true を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | チェックするオブジェクト。 |

**Returns:**
boolean - オブジェクトが条件を満たす場合は True
