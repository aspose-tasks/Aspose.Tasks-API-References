---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "サマリ行のカスタム属性値の計算タイプを指定します。"
type: docs
weight: 282
url: /ja/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

集計行のカスタム属性値の計算タイプを指定します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [None](#None) | 概要行のカスタム属性の値が計算されないことを意味します。 |
| [Rollup](#Rollup) | 概要行のカスタム属性の値が、`ExtendedAttributeDefinition.RollupType`で定義されたロールアップ関数を使用して計算されることを意味します（[ExtendedAttributeDefinition.getRollupType()](../../com.aspose/tasks/extendedattributedefinition\\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose/tasks/extendedattributedefinition\\#setRollupType-int-))。 |
| [UseFormula](#UseFormula) | 概要行のカスタム属性の値が、`ExtendedAttributeDefinition.Formula`で定義された数式を使用して計算されることを意味します（[ExtendedAttributeDefinition.getFormula()](../../com.aspose/tasks/extendedattributedefinition\\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose/tasks/extendedattributedefinition\\#setFormula-String-))。 |
### None {#None}
```
public static final int None
```


概要行のカスタム属性の値が計算されないことを意味します。

### Rollup {#Rollup}
```
public static final int Rollup
```


概要行のカスタム属性の値が、`ExtendedAttributeDefinition.RollupType`で定義されたロールアップ関数を使用して計算されることを意味します（[ExtendedAttributeDefinition.getRollupType()](../../com.aspose/tasks/extendedattributedefinition\\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose/tasks/extendedattributedefinition\\#setRollupType-int-))。

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


概要行のカスタム属性の値が、`ExtendedAttributeDefinition.Formula`で定義された数式を使用して計算されることを意味します（[ExtendedAttributeDefinition.getFormula()](../../com.aspose/tasks/extendedattributedefinition\\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose/tasks/extendedattributedefinition\\#setFormula-String-))。

--------------------

この設定を有効にするには、`ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose/tasks/extendedattributedefinition\\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose/tasks/extendedattributedefinition\\#setCalculationType-int-)) を\"Formula\"に設定する必要があります。

