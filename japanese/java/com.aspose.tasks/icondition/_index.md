---
title: "ICondition"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "フィルタや検索メソッドで使用できる条件を表します。"
type: docs
weight: 377
url: /ja/java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

フィルタや検索メソッドで使用できる条件を表します。

T : メソッドインターフェイスを適用するオブジェクトの型。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [check(T el)](#check-T-) | 指定されたオブジェクトが条件を満たす場合に true を返します。 |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


指定されたオブジェクトが条件を満たす場合に true を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| el | T | チェックするオブジェクト。 |

**Returns:**
boolean - オブジェクトが条件を満たす場合は True
