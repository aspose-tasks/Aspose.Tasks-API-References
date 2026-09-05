---
title: "DailyRepetitionBase"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "毎日繰り返しパターンの繰り返しのための基底クラスを表します。"
type: docs
weight: 65
url: /ja/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

毎日繰り返しパターンの繰り返しのための基底クラスを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | 発生間隔を日数で表す日数を取得します。 |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | 発生間隔を日数で表す日数を設定します。 |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


繰り返しを計算するために使用される計算機を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


発生間隔を日数で表す日数を取得します。

**Returns:**
int - 発生間隔を日数で表す日数。
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


再発パターンのバリデータを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


発生間隔を日数で表す日数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 発生間隔を日数で表す日数。 |

