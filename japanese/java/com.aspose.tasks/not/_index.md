---
title: "Not"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "指定された条件に論理 NOT を適用します。"
type: docs
weight: 162
url: /ja/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

指定された条件に論理 NOT を適用します。

T : メソッドインターフェイスを適用するオブジェクトの型。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Not&lt;T&gt; クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [check(T el)](#check-T-) | 指定されたオブジェクトが条件を満たす場合に true を返します。 |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Not&lt;T&gt; クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | 指定された条件。 |

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
boolean - オブジェクトが条件を満たす場合は True。
