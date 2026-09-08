---
title: "TableTextStyle.TableTextStyle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TableTextStyle 생성자. TableTextStyle 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

`[`TableTextStyle`](../)` 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TableTextStyle(int rowUid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | Int32 | 지정된 행 고유 ID입니다. |

## 예제

프로젝트에서 다양한 텍스트 항목을 스타일링하는 데 사용되는 테이블 텍스트 스타일을 사용자 지정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// 첫 번째 작업 이름 텍스트 스타일을 설정합니다
var style1 = new TableTextStyle(1);
// 스타일을 적용할 필드를 설정합니다.
style1.Field = Field.TaskName;
// 텍스트 스타일의 <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" />을 설정합니다.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// 텍스트 스타일 글꼴의 크기를 포인트 단위로 설정합니다.

// 두 번째 작업 기간 텍스트 스타일을 설정합니다
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // 뷰 데이터를 기록해야 함을 나타내는 플래그를 설정합니다
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### 또 보기

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

지정된 폰트를 사용하여 [`TableTextStyle`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | Int32 | 지정된 행 고유 ID입니다. |
| font | FontDescriptor | 텍스트 스타일이 기반하는 폰트입니다. |

### 또 보기

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

지정된 폰트 크기와 폰트 스타일을 사용하여 [`TableTextStyle`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | Int32 | 지정된 행 고유 ID입니다. |
| fontSize | Single | 텍스트 스타일이 기반하는 폰트의 크기입니다. |
| fontStyle | FontStyles | 텍스트 스타일이 기반하는 폰트의 스타일입니다. |

### 또 보기

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

기본 폰트 설정과 지정된 폰트 스타일을 사용하여 [`TableTextStyle`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | Int32 | 지정된 행 고유 ID입니다. |
| fontStyle | FontStyles | 텍스트 스타일이 기반하는 폰트의 스타일입니다. |

### 또 보기

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


