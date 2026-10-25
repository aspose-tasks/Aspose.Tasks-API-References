---
title: "열거형 DateFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.DateFormat 열거형. 날짜 형식을 지정합니다."
type: docs
weight: 430
url: /ko/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

날짜 형식을 지정합니다.

```csharp
public enum DateFormat
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | 예시: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | 예시: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | 예시: September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | 예시: September 30, 2002 |
| DateMmmDdHhMmAM | `4` | 예시: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | 예시: Sep 30, '02 |
| DateMmmmDd | `6` | 예시: September 30 |
| DateMmmDd | `7` | 예시: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | 예시: Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | 예시: Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | 예시: Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | 예시: Tue 13:00 PM |
| DateMmDd | `12` | 예시: 9/30 |
| DateDd | `13` | 예시: 30 |
| DateHhMmAm | `14` | 예시: 13:00 PM |
| DateDddMmmDd | `15` | 예시: Tue Sep 30 |
| DateDddMmDd | `16` | 예시: Tue 9/30 |
| DateDddDd | `17` | 예시: Tue 30 |
| DateWwwDd | `18` | 예시: W41/2 |
| DateWwwDdYyHhMmAm | `19` | 예시: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | 예시: 9/30/2002 |
| Custom | `21` | DateTime 값은 프로젝트의 [`CustomDateFormat`](../prj/customdateformat/) 속성에 설정된 형식 문자열을 사용하여 포맷됩니다. |
| DateDdMmYyyy | `256` | 예시: 19/07/2016 |
| Default | `255` | 예시: 기본 날짜 형식. |

## 예제

프로젝트에서 내보낼 모든 날짜의 날짜 형식을 사용자 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// 기본적으로 project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) DateFormat을 사용자 지정합니다 (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// 날짜 형식 19/07/2016으로 내보내기
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


