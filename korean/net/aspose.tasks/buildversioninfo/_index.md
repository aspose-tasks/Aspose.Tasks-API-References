---
title: "클래스 BuildVersionInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.BuildVersionInfo 클래스. 빌드 버전 및 제품 정보를 포함합니다."
type: docs
weight: 160
url: /ko/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

빌드 버전 및 제품 정보를 포함합니다.

```csharp
public static class BuildVersionInfo
```

## 필드

| 이름 | 설명 |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | 어셈블리의 정보 버전 번호입니다. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | 어셈블리 버전. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | 파일 버전. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | 제품 이름. |

## 예제

Aspose.Tasks의 빌드 버전 정보를 읽는 방법을 보여줍니다.

```csharp
// 현재 Aspose.Tasks 버전에 대한 일반 정보를 읽습니다
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


