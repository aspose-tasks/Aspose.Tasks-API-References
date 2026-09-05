---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 191
url: /ko/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

프로젝트 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | 문서를 [SaveFileFormat](../../com.aspose.tasks/savefileformat) 형식으로 저장하는 데 사용할 수 있는 [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | 생성된 PDF 문서에 대한 원하는 준수 수준을 가져옵니다. |
| [getEncryptionDetails()](#getEncryptionDetails--) | 암호화 세부 정보를 가져옵니다. |
| [getFontSettings()](#getFontSettings--) | 프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다. |
| [getPageSavingCallback()](#getPageSavingCallback--) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 가져옵니다. |
| [getPages()](#getPages--) | 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져옵니다. |
| [getReduceFooterGap()](#getReduceFooterGap--) | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져옵니다. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | 프로젝트 페이지를 별도 파일로 저장할지 여부를 나타내는 값을 가져옵니다. |
| [getTextCompression()](#getTextCompression--) | 이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 가져옵니다. |
| [setCompliance(int value)](#setCompliance-int-) | 생성된 PDF 문서에 대한 원하는 준수 수준을 설정합니다. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | 암호화 세부 정보를 설정합니다. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백을 설정합니다. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 설정합니다. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정합니다. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | 프로젝트 페이지를 별도 파일로 저장할지 여부를 나타내는 값을 설정합니다. |
| [setTextCompression(int value)](#setTextCompression-int-) | 이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 설정합니다. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


문서를 [SaveFileFormat](../../com.aspose.tasks/savefileformat) 형식으로 저장하는 데 사용할 수 있는 [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) 클래스의 새 인스턴스를 초기화합니다.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


내부 사용을 위해 예약됨.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


내부 사용을 위해 예약됨.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


생성된 PDF 문서에 대한 원하는 준수 수준을 가져옵니다. 기본값은 [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15)입니다.

**Returns:**
int - 생성된 PDF 문서에 대한 원하는 준수 수준.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


암호화 세부 정보를 가져옵니다. 설정되지 않은 경우 암호화가 수행되지 않습니다.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


프로젝트 뷰를 렌더링할 때 사용되는 글꼴 설정을 지정합니다.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


각 렌더링된 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 콜백을 가져옵니다. `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) 옵션이 사용될 때 적용됩니다.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져옵니다.

--------------------

이 목록이 비어 있으면 모든 페이지가 저장됩니다.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


프로젝트 페이지를 별도 파일로 저장할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 프로젝트 페이지를 별도 파일로 저장할지 여부를 나타내는 값.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 가져옵니다. 기본값은 [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate)입니다.

**Returns:**
int - 이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


생성된 PDF 문서에 대한 원하는 준수 수준을 설정합니다. 기본값은 [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15)입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 생성된 PDF 문서에 대한 원하는 준수 수준. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


암호화 세부 정보를 설정합니다. 설정되지 않은 경우 암호화가 수행되지 않습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | 암호화 세부 정보. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


각 렌더링된 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 콜백을 설정합니다. `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) 옵션이 사용될 때 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 각 렌더링된 페이지에 대한 출력 스트림을 얻기 위해 사용되는 사용자 정의 콜백. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 설정합니다.

--------------------

이 목록이 비어 있으면 모든 페이지가 저장됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.List&lt;java.lang.Integer&gt; | 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 나타내는 값. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


프로젝트 페이지를 별도 파일로 저장할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트 페이지를 별도의 파일에 저장할지 여부를 나타내는 값입니다. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 설정합니다. 기본값은 [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\\#Flate)입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형입니다. |

