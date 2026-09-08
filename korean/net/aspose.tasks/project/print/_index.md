---
title: "Project.Print"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 표준 UI 없는 인쇄 컨트롤러를 사용하여 기본 프린터 설정으로 프로젝트를 기본 프린터에 인쇄합니다."
type: docs
weight: 1140
url: /ko/net/aspose.tasks/project/print/
---
## Print() {#print}

표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 기본 프린터와 기본 프린터 설정으로 프로젝트를 인쇄합니다.

```csharp
public void Print()
```

## 예제

프로젝트를 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 기본 프린터와 기본 프린터 설정 및 사용자 지정 저장 옵션으로 프로젝트를 인쇄합니다.

```csharp
public void Print(PrintOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| options | PrintOptions | 지정된 [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) 클래스의 인스턴스. |

## 예제

인쇄 옵션을 사용하여 프로젝트를 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.ThirdsOfMonths
};
if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
{
    project.Print(options);
}
```

### 또 보기

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터와 기본 프린터 설정으로 프로젝트를 인쇄합니다.

```csharp
public void Print(string printerName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| printerName | 문자열 | 지정된 프린터 이름. |

## 예제

선택한 프린터에서 프로젝트를 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

foreach (string printer in PrinterSettings.InstalledPrinters)
{
    if (!printer.ToUpperInvariant().Contains("Microsoft Print to PDF".ToUpperInvariant()))
    {
        continue;
    }

    project.Print(printer);
    break;
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다.

```csharp
public void Print(PrinterSettings printerSettings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings 클래스의 지정된 인스턴스. |

## 예제

프린터 설정을 사용하여 프로젝트를 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 첫 두 페이지 인쇄
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정에 따라 프로젝트를 인쇄합니다.

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings 클래스의 지정된 인스턴스. |
| documentName | 문자열 | 표시할 문서 이름(예: 인쇄 상태 대화 상자 또는 프린터 대기열에 표시). |

## 예제

프린터 설정과 문서 이름을 사용하여 프로젝트를 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 첫 두 페이지 인쇄
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정 및 사용자 지정 저장 옵션에 따라 프로젝트를 인쇄합니다.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings 클래스의 지정된 인스턴스. |
| options | PrintOptions | 지정된 [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) 클래스의 인스턴스. |

## 예제

프린터 옵션 및 설정을 사용하여 프로젝트를 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// 첫 두 페이지 인쇄
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### 또 보기

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

표준(사용자 인터페이스 없음) 인쇄 컨트롤러를 사용하여 지정된 프린터 설정, 사용자 지정 저장 옵션 및 지정된 문서 이름에 따라 프로젝트를 인쇄합니다.

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| printerSettings | PrinterSettings | PrinterSettings 클래스의 지정된 인스턴스. |
| options | PrintOptions | 지정된 [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) 클래스의 인스턴스. |
| documentName | 문자열 | 표시할 문서 이름(예: 인쇄 상태 대화 상자 또는 프린터 대기열에 표시). |

## 예제

프린터 옵션, 프린터 설정 및 문서 이름을 사용하여 프로젝트를 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// 첫 두 페이지 인쇄
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### 또 보기

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


