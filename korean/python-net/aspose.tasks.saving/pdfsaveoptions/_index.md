---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 90
url: /ko/python-net/aspose.tasks.saving/pdfsaveoptions/
---

## PdfSaveOptions class

프로젝트 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.

PdfSaveOptions 유형은 다음 멤버를 노출합니다:
## 생성자
| 이름 | 설명 |
| :- | :- |
| PdfSaveOptions() | 문서를 저장하는 데 사용할 수 있는 [PdfSaveOptions](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/) 클래스의 새 인스턴스를 초기화합니다 |
## 속성
| 이름 | 설명 |
| :- | :- |
| save_format |  |
| bar_styles | 프로젝트 뷰에 표시되는 [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) 클래스 인스턴스 목록을 가져오거나 설정합니다. |
| draw_non_working_time | 비작업 시간을 그릴지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 TRUE). |
| end_date | 렌더링을 종료할 날짜를 가져오거나 설정합니다. |
| timescale_fit_behavior | 시간축의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 가져오거나 설정합니다. |
| fit_content | 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 가져오거나 설정합니다. |
| gridlines | 프로젝트 뷰에 표시되는 [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) 목록을 가져오거나 설정합니다. |
| legend_drawing_options | 범례를 렌더링하는 방법을 정의하는 값을 가져오거나 설정합니다. 기본값은 LegendDrawingOptions.OnEveryPage입니다. |
| legend_items | 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져오거나 설정합니다.<br/>            null인 경우 기본 항목이 렌더링됩니다. |
| mark_critical_tasks | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 FALSE). |
| non_working_time_color | 비작업 시간 색상을 가져오거나 설정합니다. |
| page_count | 프로젝트의 페이지 수를 가져오거나 설정합니다. |
| page_size | 렌더링될 페이지 크기를 가져오거나 설정합니다 (기본값은 PageSize.A4). |
| is_portrait | 페이지 방향이 세로인지 여부를 나타내는 값을 가져오거나 설정합니다; 페이지 방향이 가로인 경우 false를 반환합니다. |
| presentation_format | 문서가 저장될 [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/)을 가져오거나 설정합니다. |
| roll_up_gantt_bars | 요약 작업 막대에 하위 작업이 표시될지 여부를 나타내는 값을 가져오거나 설정합니다.<br/>            하위 작업의 경우, Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 롤업될지 여부를 나타냅니다.<br/>            요약 작업의 경우, Rollup 필드는 요약 작업 막대가 롤업된 막대를 표시할지 여부를 나타냅니다.<br/>            하위 작업이 롤업되도록 하려면 요약 작업에 대한 Rollup 필드를 Yes로 설정해야 합니다. |
| start_date | 렌더링을 시작할 날짜를 가져오거나 설정합니다. |
| text_styles | 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져오거나 설정합니다. |
| timescale | 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(있는 경우)이 어떻게 렌더링되는지를 제어하는 데 사용되는 [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) 값을 가져오거나 설정합니다. |
| use_gradient_brush | Gantt 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| view | 렌더링할 뷰 열 목록을 가져오거나 설정합니다 ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            설정되지 않은 경우 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다.<br/>            View와 [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다. |
| view_settings | 렌더링할 뷰 ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/))를 가져오거나 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장될 뷰를 명시적으로 지정할 수 있습니다.<br/>            이 속성이 설정된 경우, 프로젝트 저장 시 [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) 속성이 무시됩니다.<br/>            뷰는 다음 화면 중 하나에서 선택해야 합니다 (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | 포인트 단위(1 포인트 = 1/72 인치)로 사용자 지정 페이지 크기를 가져오거나 설정합니다. |
| render_to_single_page | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링되어야 하는지 여부를 가져오거나 설정합니다.<br/>            페이지 크기가 변경되어 렌더링된 프로젝트가 한 페이지에 맞도록 합니다. |
| reduce_footer_gap | 마지막 작업과 푸터 사이의 간격을 줄여야 하는지 여부를 가져오거나 설정합니다. |
| compliance | 생성된 PDF 문서에 대한 원하는 호환성 수준을 가져오거나 설정합니다.<br/>            기본값은 [PDF15](/tasks/python-net/aspose.tasks.saving/pdfcompliance/)입니다. |
| encryption_details | 암호화 세부 정보를 가져오거나 설정합니다. 설정되지 않으면 암호화가 수행되지 않습니다. |
| text_compression | 이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 가져오거나 설정합니다.<br/>            기본값은 [FLATE](/tasks/python-net/aspose.tasks.saving/pdftextcompression/)입니다. |
| digital_signature_details | 디지털 서명 세부 정보를 가져오거나 설정합니다. 설정되지 않으면 서명이 수행되지 않습니다. |
| save_to_separate_files | 프로젝트 페이지를 별도의 파일로 저장할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| page_saving_callback | 각 렌더링된 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 콜백을 가져오거나 설정합니다.<br/>            [save_to_separate_files](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/) 옵션이 사용될 때 적용됩니다. |
| pages | 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. |
| font_settings | 프로젝트 보기 렌더링 시 사용되는 글꼴 설정을 지정합니다. |

### 또 보기

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

