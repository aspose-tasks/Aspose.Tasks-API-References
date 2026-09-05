---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "平準化順序の可能な値を定義します。"
type: docs
weight: 143
url: /ja/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

平準化順序の可能な値を定義します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [IdOnly](#IdOnly) | タスクは ID の昇順で遅延します。 |
| [PriorityThenStandard](#PriorityThenStandard) | 優先度が最初に考慮され、次に Standard と同じプロパティが適用されます。 |
| [Standard](#Standard) | 次のプロパティが考慮されます: 前任タスクとの関係、総余裕時間（総余裕時間が大きいタスクが先に遅延）、開始日、優先度。 |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


タスクは ID の昇順で遅延します。

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


優先度が最初に考慮され、次に Standard と同じプロパティが適用されます。

### Standard {#Standard}
```
public static final int Standard
```


次のプロパティが考慮されます: 前任タスクとの関係、総余裕時間（総余裕時間が大きいタスクが先に遅延）、開始日、優先度。これはデフォルト値です。

