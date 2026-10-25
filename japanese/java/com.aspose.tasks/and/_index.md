---
title: "および"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "指定された条件に論理 AND を適用します。"
type: docs
weight: 10
url: /ja/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

指定された条件に論理 AND を適用します。

T : メソッドインターフェイスを適用するオブジェクトの型。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | And&lt;T&gt; クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [check(T el)](#check-T-) | 指定されたオブジェクトが条件を満たす場合に true を返します。 |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


And&lt;T&gt; クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | 最初の条件。 |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | 2番目の条件。 |

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
