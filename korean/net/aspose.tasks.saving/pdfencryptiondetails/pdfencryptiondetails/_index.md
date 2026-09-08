---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfEncryptionDetails 생성자. PdfEncryptionDetails 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

새 인스턴스를 초기화합니다. [`PdfEncryptionDetails`](../) 클래스.

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| userPassword | 문자열 | 보호된 문서를 열 수 있는 사용자 비밀번호입니다. |
| ownerPassword | 문자열 | 보호된 문서를 열 수 있는 소유자 비밀번호입니다. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | 암호화 알고리즘을 나타내는 [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) 인스턴스입니다. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


