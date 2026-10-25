---
title: "PrinterSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "문서를 인쇄하는 방법에 대한 정보와 인쇄기를 포함하여 지정합니다."
type: docs
weight: 215
url: /ko/java/com.aspose.tasks/printersettings/
---

**Inheritance:**
java.lang.Object
```
public class PrinterSettings
```

문서가 인쇄되는 방식에 대한 정보(인쇄하는 프린터 포함)를 지정합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PrinterSettings()](#PrinterSettings--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCollate()](#getCollate--) | 인쇄된 문서가 정렬되는지 여부를 나타내는 값을 가져옵니다. |
| [getCopies()](#getCopies--) | 인쇄할 문서 복사본 수를 가져옵니다. |
| [getFromPage()](#getFromPage--) | 인쇄할 첫 페이지의 페이지 번호를 가져옵니다. |
| [getPrintFileName()](#getPrintFileName--) | 파일에 인쇄할 때 파일 이름을 가져옵니다. |
| [getPrinterName()](#getPrinterName--) | 사용할 프린터의 이름을 가져옵니다. |
| [getSupportsColor()](#getSupportsColor--) | 이 프린터가 컬러 인쇄를 지원하는지 여부를 나타내는 값을 가져옵니다. |
| [getToPage()](#getToPage--) | 인쇄할 마지막 페이지의 번호를 가져옵니다. |
| [isDefaultPrinter()](#isDefaultPrinter--) | 사용자가 PrinterName을 명시적으로 설정한 경우를 제외하고, PrinterName 속성이 기본 프린터를 지정하는지 여부를 나타내는 값을 가져옵니다. |
| [setCollate(boolean value)](#setCollate-boolean-) | 인쇄된 문서가 정렬되는지 여부를 나타내는 값을 설정합니다. |
| [setCopies(short value)](#setCopies-short-) | 인쇄할 문서 사본 수를 설정합니다. |
| [setFromPage(int value)](#setFromPage-int-) | 인쇄할 첫 페이지의 페이지 번호를 설정합니다. |
| [setPrintFileName(String value)](#setPrintFileName-java.lang.String-) | 파일에 인쇄할 때 파일 이름을 설정합니다. |
| [setPrinterName(String value)](#setPrinterName-java.lang.String-) | 사용할 프린터의 이름을 설정합니다. |
| [setToPage(int value)](#setToPage-int-) | 인쇄할 마지막 페이지의 번호를 설정합니다. |
| [toString()](#toString--) | PrinterSettings에 대한 정보를 문자열 형태로 제공합니다. |
### PrinterSettings() {#PrinterSettings--}
```
public PrinterSettings()
```


### getCollate() {#getCollate--}
```
public boolean getCollate()
```


인쇄된 문서가 정렬되는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 인쇄된 문서가 정렬되는지 여부를 나타내는 값.
### getCopies() {#getCopies--}
```
public short getCopies()
```


인쇄할 문서 복사본 수를 가져옵니다.

**Returns:**
short - 인쇄할 문서 사본 수.
### getFromPage() {#getFromPage--}
```
public int getFromPage()
```


인쇄할 첫 페이지의 페이지 번호를 가져옵니다.

**Returns:**
int - 인쇄할 첫 페이지의 페이지 번호.
### getPrintFileName() {#getPrintFileName--}
```
public String getPrintFileName()
```


파일에 인쇄할 때 파일 이름을 가져옵니다.

**Returns:**
java.lang.String - 파일에 인쇄할 때 파일 이름.
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```


사용할 프린터의 이름을 가져옵니다.

**Returns:**
java.lang.String - 사용할 프린터의 이름.
### getSupportsColor() {#getSupportsColor--}
```
public boolean getSupportsColor()
```


이 프린터가 컬러 인쇄를 지원하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 이 프린터가 컬러 인쇄를 지원하는지 여부를 나타내는 값.
### getToPage() {#getToPage--}
```
public int getToPage()
```


인쇄할 마지막 페이지의 번호를 가져옵니다.

**Returns:**
int - 인쇄할 마지막 페이지의 번호.
### isDefaultPrinter() {#isDefaultPrinter--}
```
public boolean isDefaultPrinter()
```


사용자가 PrinterName을 명시적으로 설정한 경우를 제외하고, PrinterName 속성이 기본 프린터를 지정하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - PrinterName 속성이 기본 프린터를 지정하는지 여부를 나타내는 값.
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


인쇄된 문서가 정렬되는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 인쇄된 문서가 정렬되는지 여부를 나타내는 값. |

### setCopies(short value) {#setCopies-short-}
```
public void setCopies(short value)
```


인쇄할 문서 사본 수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | short | 인쇄할 문서 사본 수. |

### setFromPage(int value) {#setFromPage-int-}
```
public void setFromPage(int value)
```


인쇄할 첫 페이지의 페이지 번호를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 인쇄할 첫 페이지의 페이지 번호. |

### setPrintFileName(String value) {#setPrintFileName-java.lang.String-}
```
public void setPrintFileName(String value)
```


파일에 인쇄할 때 파일 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 파일에 인쇄할 때 파일 이름. |

### setPrinterName(String value) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String value)
```


사용할 프린터의 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 사용할 프린터의 이름. |

### setToPage(int value) {#setToPage-int-}
```
public void setToPage(int value)
```


인쇄할 마지막 페이지의 번호를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 인쇄할 마지막 페이지 번호. |

### toString() {#toString--}
```
public String toString()
```


PrinterSettings에 대한 정보를 문자열 형태로 제공합니다.

**Returns:**
java.lang.String - 문자열 형태의 PrinterSettings에 대한 정보.
