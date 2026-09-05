---
title: "PdfEncryptionDetails"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "PDF 暗号化の詳細を含みます。"
type: docs
weight: 189
url: /ja/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

PDF 暗号化の詳細を含みます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | 暗号化モードを取得します。 |
| [getOwnerPassword()](#getOwnerPassword--) | 所有者パスワードを取得します。 |
| [getPermissions()](#getPermissions--) | アクセス許可を取得します。 |
| [getUserPassword()](#getUserPassword--) | ユーザーパスワードを取得します。 |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | 暗号化モードを設定します。 |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | 所有者パスワードを設定します。 |
| [setPermissions(int value)](#setPermissions-int-) | アクセス許可を設定します。 |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | ユーザーパスワードを設定します。 |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| userPassword | java.lang.String | 保護されたドキュメントを開くためのユーザーパスワード。 |
| ownerPassword | java.lang.String | 保護されたドキュメントを開くための所有者パスワード。 |
| encryptionAlgorithm | int | 暗号化アルゴリズムを示す [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) インスタンス。 |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


暗号化モードを取得します。

**Returns:**
int - 暗号化モード。
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


所有者パスワードを取得します。

--------------------

正しい所有者パスワードでドキュメントを開くと（ユーザーパスワードと同じでないと仮定して）、ドキュメントへの完全な（所有者）アクセスが可能になります。この無制限のアクセスには、ドキュメント\\u2019s のパスワードとアクセス許可を変更する機能が含まれます。

**Returns:**
java.lang.String - 所有者パスワード。
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


アクセス許可を取得します。

**Returns:**
int - アクセス許可。
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


ユーザーパスワードを取得します。

--------------------

正しいユーザーパスワードでドキュメントを開く（またはユーザーパスワードが設定されていないドキュメントを開く）と、ドキュメント\\u2019s の暗号化辞書に指定されたユーザーアクセス許可に従って追加の操作を実行できます。

**Returns:**
java.lang.String - ユーザーパスワード。
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


暗号化モードを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 暗号化モード。 |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


所有者パスワードを設定します。

--------------------

正しい所有者パスワードでドキュメントを開くと（ユーザーパスワードと同じでないと仮定して）、ドキュメントへの完全な（所有者）アクセスが可能になります。この無制限のアクセスには、ドキュメント\\u2019s のパスワードとアクセス許可を変更する機能が含まれます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 所有者パスワード。 |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


アクセス許可を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 権限。 |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


ユーザーパスワードを設定します。

--------------------

正しいユーザーパスワードでドキュメントを開く（またはユーザーパスワードが設定されていないドキュメントを開く）と、ドキュメント\\u2019s の暗号化辞書に指定されたユーザーアクセス許可に従って追加の操作を実行できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | ユーザーパスワード。 |

