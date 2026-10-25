---
title: "클래스 PdfEncryptionDetails"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfEncryptionDetails 클래스. PDF 암호화에 대한 세부 정보를 포함합니다"
type: docs
weight: 2110
url: /ko/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

PDF 암호화에 대한 세부 정보를 포함합니다.

```csharp
public class PdfEncryptionDetails
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | `PdfEncryptionDetails` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | 암호화 모드를 가져오거나 설정합니다. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | 소유자 비밀번호를 가져오거나 설정합니다. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | 권한을 가져오거나 설정합니다. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | 사용자 비밀번호를 가져오거나 설정합니다. |

## 예제

프로젝트를 PDF 파일로 저장할 때 PDF 암호화 세부 정보를 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// 암호화 세부 정보를 지정해 보세요
var encryptionDetails = new PdfEncryptionDetails(
    // 사용자 비밀번호 지정
    "userPassword", 
    // 소유자 비밀번호 지정
    "ownerPassword", 
    // 암호화 알고리즘 지정
    PdfEncryptionAlgorithm.RC4_128);

// 권한 지정
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// 사용자 및 소유자 비밀번호 표시
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// 암호화 모드 표시: RC4_40 또는 RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// 지정된 암호화 세부 정보를 사용하여 프로젝트를 저장합니다
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


