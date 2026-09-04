---
title: "PrinterSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定文档的打印方式信息，包括使用的打印机。"
type: docs
weight: 215
url: /zh/java/com.aspose.tasks/printersettings/
---

**Inheritance:**
java.lang.Object
```
public class PrinterSettings
```

指定有关文档打印方式的信息，包括执行打印的打印机。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PrinterSettings()](#PrinterSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCollate()](#getCollate--) | 获取一个值，指示打印的文档是否已分页装订。 |
| [getCopies()](#getCopies--) | 获取要打印的文档副本数。 |
| [getFromPage()](#getFromPage--) | 获取要打印的第一页的页码。 |
| [getPrintFileName()](#getPrintFileName--) | 获取打印到文件时的文件名。 |
| [getPrinterName()](#getPrinterName--) | 获取要使用的打印机名称。 |
| [getSupportsColor()](#getSupportsColor--) | 获取指示此打印机是否支持彩色打印的值。 |
| [getToPage()](#getToPage--) | 获取要打印的最后一页的页码。 |
| [isDefaultPrinter()](#isDefaultPrinter--) | 获取指示 PrinterName 属性是否指定默认打印机的值，除非用户显式设置 PrinterName。 |
| [setCollate(boolean value)](#setCollate-boolean-) | 设置指示打印文档是否已排序的值。 |
| [setCopies(short value)](#setCopies-short-) | 设置要打印的文档副本数量。 |
| [setFromPage(int value)](#setFromPage-int-) | 设置要打印的第一页的页码。 |
| [setPrintFileName(String value)](#setPrintFileName-java.lang.String-) | 设置打印到文件时的文件名。 |
| [setPrinterName(String value)](#setPrinterName-java.lang.String-) | 设置要使用的打印机名称。 |
| [setToPage(int value)](#setToPage-int-) | 设置要打印的最后一页的页码。 |
| [toString()](#toString--) | 以字符串形式提供有关 PrinterSettings 的信息。 |
### PrinterSettings() {#PrinterSettings--}
```
public PrinterSettings()
```


### getCollate() {#getCollate--}
```
public boolean getCollate()
```


获取一个值，指示打印的文档是否已分页装订。

**Returns:**
boolean - 指示打印文档是否已排序的值。
### getCopies() {#getCopies--}
```
public short getCopies()
```


获取要打印的文档副本数。

**Returns:**
short - 要打印的文档副本数量。
### getFromPage() {#getFromPage--}
```
public int getFromPage()
```


获取要打印的第一页的页码。

**Returns:**
int - 要打印的第一页的页码。
### getPrintFileName() {#getPrintFileName--}
```
public String getPrintFileName()
```


获取打印到文件时的文件名。

**Returns:**
java.lang.String - 打印到文件时的文件名。
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```


获取要使用的打印机名称。

**Returns:**
java.lang.String - 要使用的打印机名称。
### getSupportsColor() {#getSupportsColor--}
```
public boolean getSupportsColor()
```


获取指示此打印机是否支持彩色打印的值。

**Returns:**
boolean - 指示此打印机是否支持彩色打印的值。
### getToPage() {#getToPage--}
```
public int getToPage()
```


获取要打印的最后一页的页码。

**Returns:**
int - 要打印的最后一页的页码。
### isDefaultPrinter() {#isDefaultPrinter--}
```
public boolean isDefaultPrinter()
```


获取指示 PrinterName 属性是否指定默认打印机的值，除非用户显式设置 PrinterName。

**Returns:**
boolean - 指示 PrinterName 属性是否指定默认打印机的值。
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


设置指示打印文档是否已排序的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示打印文档是否已排序的值。 |

### setCopies(short value) {#setCopies-short-}
```
public void setCopies(short value)
```


设置要打印的文档副本数量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | short | 要打印的文档副本数量。 |

### setFromPage(int value) {#setFromPage-int-}
```
public void setFromPage(int value)
```


设置要打印的第一页的页码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要打印的第一页的页码。 |

### setPrintFileName(String value) {#setPrintFileName-java.lang.String-}
```
public void setPrintFileName(String value)
```


设置打印到文件时的文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 打印到文件时的文件名。 |

### setPrinterName(String value) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String value)
```


设置要使用的打印机名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 要使用的打印机名称。 |

### setToPage(int value) {#setToPage-int-}
```
public void setToPage(int value)
```


设置要打印的最后一页的页码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要打印的最后一页页码。 |

### toString() {#toString--}
```
public String toString()
```


以字符串形式提供有关 PrinterSettings 的信息。

**Returns:**
java.lang.String - 关于 PrinterSettings 的字符串形式信息。
