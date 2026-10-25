---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "未定義の制約を持つタスクを処理するために使用される動作を指定します。"
type: docs
weight: 329
url: /ja/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

未定義の制約を持つタスクを処理するために使用される動作を指定します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [None](#None) | XER 形式からロードする際のデフォルト動作です。 |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | タイプが 'ConstraintType.StartNoEarlierThan' で日付が Start の制約が、'Undefined' 制約を持つタスクに追加されます。 |
### None {#None}
```
public static final int None
```


XER 形式からロードする際のデフォルト動作です。何も実行されません。タスクの制約タイプは 'ConstraintType.Undefined' に設定されます。

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


タイプが 'ConstraintType.StartNoEarlierThan' で日付が Start の制約が、'Undefined' 制約を持つタスクに追加されます。

