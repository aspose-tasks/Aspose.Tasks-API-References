---
title: "GlobalizationSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目的全球化设置。"
type: docs
weight: 114
url: /zh/java/com.aspose.tasks/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

表示项目的全球化设置。

推荐的做法是在整个项目中使用与文化无关的文字或格式。不过，如果项目使用特定文化的文字，则可以使用此类来帮助公式计算引擎解析这些文字。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFalseLiteral()](#getFalseLiteral--) | 获取公式中布尔值 'false' 文字的字符串。 |
| [getFormulaDateNA()](#getFormulaDateNA--) | 获取公式中用于日期字段的 "NA"（空值）文字。 |
| [getTrueLiteral()](#getTrueLiteral--) | 获取公式中布尔值 'true' 文字的字符串。 |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### getFalseLiteral() {#getFalseLiteral--}
```
public String getFalseLiteral()
```


获取公式中布尔值 'false' 文字的字符串。

**Returns:**
java.lang.String - 用于公式中布尔值 'false' 字面量的字符串。
### getFormulaDateNA() {#getFormulaDateNA--}
```
public String getFormulaDateNA()
```


获取公式中用于日期字段的 "NA"（空值）文字。

**Returns:**
java.lang.String - 在日期字段的公式中使用的 \"NA\"（空值）字面量。
### getTrueLiteral() {#getTrueLiteral--}
```
public String getTrueLiteral()
```


获取公式中布尔值 'true' 文字的字符串。

**Returns:**
java.lang.String - 用于公式中布尔值 'true' 字面量的字符串。
