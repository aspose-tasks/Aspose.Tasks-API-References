---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API Reference"
description: "PDF 암호화에 대한 세부 정보를 포함합니다."
type: docs
weight: 189
url: /ko/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

PDF 암호화에 대한 세부 정보를 포함합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | 새로운 [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | 암호화 모드를 가져옵니다. |
| [getOwnerPassword()](#getOwnerPassword--) | Owner 비밀번호를 가져옵니다. |
| [getPermissions()](#getPermissions--) | 권한을 가져옵니다. |
| [getUserPassword()](#getUserPassword--) | User 비밀번호를 가져옵니다. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | 암호화 모드를 설정합니다. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Owner 비밀번호를 설정합니다. |
| [setPermissions(int value)](#setPermissions-int-) | 권한을 설정합니다. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | User 비밀번호를 설정합니다. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


새로운 [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| userPassword | java.lang.String | 보호된 문서를 열 수 있게 하는 사용자 비밀번호. |
| ownerPassword | java.lang.String | 보호된 문서를 열 수 있게 하는 소유자 비밀번호. |
| encryptionAlgorithm | int | 암호화 알고리즘을 나타내는 [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) 인스턴스. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


암호화 모드를 가져옵니다.

**Returns:**
int - 암호화 모드.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Owner 비밀번호를 가져옵니다.

--------------------

올바른 소유자 비밀번호로 문서를 열면(사용자 비밀번호와 동일하지 않다고 가정) 문서에 대한 전체(소유자) 접근이 허용됩니다. 이 무제한 접근에는 문서\\u2019s 비밀번호와 접근 권한을 변경할 수 있는 기능이 포함됩니다.

**Returns:**
java.lang.String - Owner 비밀번호.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


권한을 가져옵니다.

**Returns:**
int - 권한.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


User 비밀번호를 가져옵니다.

--------------------

올바른 사용자 비밀번호로 문서를 열거나(사용자 비밀번호가 없는 문서를 열 경우) 문서에 지정된 사용자 접근 권한에 따라 추가 작업을 수행할 수 있습니다. 이 권한은 문서\\u2019s 암호화 사전에서 지정됩니다.

**Returns:**
java.lang.String - 사용자 비밀번호.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


암호화 모드를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 암호화 모드. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Owner 비밀번호를 설정합니다.

--------------------

올바른 소유자 비밀번호로 문서를 열면(사용자 비밀번호와 동일하지 않다고 가정) 문서에 대한 전체(소유자) 접근이 허용됩니다. 이 무제한 접근에는 문서\\u2019s 비밀번호와 접근 권한을 변경할 수 있는 기능이 포함됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 소유자 비밀번호. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


권한을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 권한. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


User 비밀번호를 설정합니다.

--------------------

올바른 사용자 비밀번호로 문서를 열거나(사용자 비밀번호가 없는 문서를 열 경우) 문서에 지정된 사용자 접근 권한에 따라 추가 작업을 수행할 수 있습니다. 이 권한은 문서\\u2019s 암호화 사전에서 지정됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 사용자 비밀번호. |

