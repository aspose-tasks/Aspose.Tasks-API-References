---
title: "Rsc"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل الخصائص المدعومة لكائن Resource."
type: docs
weight: 271
url: /ar/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

يمثل الخصائص المدعومة لكائن `Resource`.
## الحقول

| حقل | الوصف |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | يحدد كيف ومتى يتم تحميل أو تراكم تكاليف الموارد القياسية والوقت الإضافي إلى تكلفة المهمة. |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | معرف Active Directory (Guid) للموارد. |
| [ACTUAL_COST](#ACTUAL-COST) | التكاليف المتكبدة للعمل الذي أُنجز بالفعل من قبل الموارد على مهامهم، بالإضافة إلى أي تكاليف مسجلة أخرى مرتبطة بالمهمة. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | التكاليف المتكبدة للعمل الإضافي الذي تم إنجازه بالفعل على المهام بواسطة الموارد المعينة. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | الكمية الفعلية للعمل الإضافي الذي تم إنجازه بالفعل بواسطة المورد المعين للمهام. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | كمية العمل التي يتم من خلالها حماية العمل الإضافي الفعلي. |
| [ACTUAL_WORK](#ACTUAL-WORK) | كمية العمل التي تم إنجازها بالفعل بواسطة المورد المعين للمهام. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | كمية العمل التي يتم من خلالها حماية العمل الفعلي. |
| [ACWP](#ACWP) | التكلفة الفعلية للعمل الذي قام به مورد للمشروع حتى الآن. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | اسم مالك التعيين. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | معرف GUID لمالك التعيين. |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | تاريخ البدء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية. |
| [AVAILABLE_TO](#AVAILABLE-TO) | تاريخ الانتهاء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية. |
| [BCWP](#BCWP) | التكلفة المتوقعة للعمل الذي قام به مورد للمشروع حتى الآن. |
| [BCWS](#BCWS) | تكلفة الميزانية للعمل المجدول لمورد. |
| [BOOKING_TYPE](#BOOKING-TYPE) | نوع الحجز للمورد. |
| [BUDGET_COST](#BUDGET-COST) | تكاليف الميزانية للموارد ذات تكلفة الميزانية. |
| [BUDGET_WORK](#BUDGET-WORK) | عمل الميزانية للموارد المادية وموارد عمل الميزانية. |
| [CALENDAR](#CALENDAR) | تقويم المورد. |
| [CAN_LEVEL](#CAN-LEVEL) | يحدد ما إذا كان يمكن إجراء تسوية الموارد على مورد. |
| [CODE](#CODE) | الرمز أو معلومات أخرى حول المورد. |
| [COST](#COST) | التكلفة الإجمالية المجدولة أو المتوقعة لمورد، استنادًا إلى التكاليف المتكبدة بالفعل للعمل الذي قام به الموارد المعينة للمهام، بالإضافة إلى التكاليف المخطط لها للعمل المتبقي. |
| [COST_CENTER](#COST-CENTER) | يحدد أي مركز تكلفة يجب تحميل التكاليف المتراكمة للمورد إليه. |
| [COST_PER_USE](#COST-PER-USE) | التكلفة التي تتراكم في كل مرة يتم فيها استخدام المورد. |
| [COST_VARIANCE](#COST-VARIANCE) | الفرق بين تكلفة الأساس والتكلفة الإجمالية لمورد. |
| [CREATED](#CREATED) | التاريخ والوقت الذي تم فيه إضافة المورد إلى المشروع. |
| [CV](#CV) | انحراف تكلفة القيمة المكتسبة حتى تاريخ حالة المشروع. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | عنوان البريد الإلكتروني للمورد. |
| [FINISH](#FINISH) | التاريخ الذي من المقرر أن يُكمل فيه المورد العمل على جميع المهام المعيَّنة. |
| [GROUP](#GROUP) | المجموعة التي ينتمي إليها المورد. |
| [GUID](#GUID) | يحتوي على رمز التعريف الفريد المُولَّد للمورد. |
| [HYPERLINK](#HYPERLINK) | العنوان أو النص التوضيحي للرابط المرتبط بالمورد. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | العنوان الخاص بالرابط المرتبط بالمورد. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | الموقع المحدد في المستند داخل الرابط المرتبط بالمهمة. |
| [ID](#ID) | معرّف الموضع للمورد داخل قائمة الموارد. |
| [INACTIVE](#INACTIVE) | يحدد ما إذا كان المورد قد تم جعله غير نشط بواسطة مستخدم يمتلك صلاحيات إدارية. |
| [INITIALS](#INITIALS) | الأحرف الأولى للمورد. |
| [IS_BUDGET](#IS-BUDGET) | يحدد ما إذا كان مورد العمل أو المادة أو التكلفة هو مورد ميزانية. |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | يحدد ما إذا كان المورد هو مورد تكلفة. |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | يظهر ما إذا كان المورد من مجموعة موارد المؤسسة (صحيح) أو من مجموعة الموارد المحلية (خطأ). |
| [IS_GENERIC](#IS-GENERIC) | يحدد ما إذا كان المورد عامًا أم لا. |
| [IS_NULL](#IS-NULL) | يحدد ما إذا كان المورد فارغًا. |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | يظهر ما إذا كان المورد الحالي مورد فريق. |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | وحدة القياس للمورد المادي. |
| [MAX_UNITS](#MAX-UNITS) | الحد الأقصى لعدد الوحدات التي تمثل السعة القصوى التي يتوفر فيها المورد لإنجاز أي مهام خلال الفترة الزمنية الحالية. |
| [NAME](#NAME) | اسم المورد. |
| [NOTES_RTF](#NOTES-RTF) | ملاحظات النص بتنسيق RTF. |
| [NOTES_TEXT](#NOTES-TEXT) | النص العادي للملاحظات المستخرج من بيانات RTF. |
| [OVERALLOCATED](#OVERALLOCATED) | يشير إلى ما إذا كان المورد مُعيَّنًا لعمل أكثر على مهمة محددة أو جميع المهام مما يمكن إكماله ضمن السعة العمل العادية. |
| [OVERTIME_COST](#OVERTIME-COST) | إجمالي تكلفة العمل الإضافي للمورد على جميع المهام المعيَّنة. |
| [OVERTIME_RATE](#OVERTIME-RATE) | معدل الأجر للعمل الإضافي الذي يؤديه المورد. |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي. |
| [OVERTIME_WORK](#OVERTIME-WORK) | كمية العمل الإضافي المجدولة التي سيؤديها المورد على مهمة ويتم احتسابها وفق معدلات العمل الإضافي للموارد المشاركة. |
| [PEAK_UNITS](#PEAK-UNITS) | الحد الأقصى لوحدة التعيين لمورد في أي لحظة زمنية لجميع المهام التي تم تعيين المورد لها. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | نسبة العمل المكتمل عبر جميع المهام. |
| [PHONETICS](#PHONETICS) | التهجئة الصوتية لاسم المورد. |
| [REGULAR_WORK](#REGULAR-WORK) | إجمالي كمية العمل غير الإضافي المجدول الذي سيؤدى بواسطة المورد. |
| [REMAINING_COST](#REMAINING-COST) | المصروف المجدول المتبقي الذي سيتكبد عند إكمال العمل المجدول المتبقي. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | المصروف الإضافي المجدول المتبقي لمورد. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | كمية العمل الإضافي المجدول المتبقية. |
| [REMAINING_WORK](#REMAINING-WORK) | الوقت المتبقي المطلوب لإكمال مهمة أو مجموعة مهام. |
| [STANDARD_RATE](#STANDARD-RATE) | معدل الأجر للعمل العادي غير الإضافي الذي يؤديه المورد. |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | الوحدات المستخدمة في Microsoft Project لعرض المعدل القياسي. |
| [START](#START) | التاريخ الذي يُجدول فيه بدء عمل المورد المعين على مهمة. |
| [SV](#SV) | انحراف جدول القيمة المكتسبة، حتى تاريخ حالة المشروع. |
| [TYPE](#TYPE) | نوع المورد. |
| [UID](#UID) | المعرّف الفريد للمورد. |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | حساب NT المرتبط بالمورد. |
| [WORK](#WORK) | إجمالي الوقت المجدول للمورد على مهمة. |
| [WORKGROUP](#WORKGROUP) | نوع مجموعة العمل التي ينتمي إليها المورد. |
| [WORK_VARIANCE](#WORK-VARIANCE) | الفرق بين عمل الخط الأساسي للمورد والعمل المجدول الحالي. |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


يحدد كيف ومتى يتم تحميل أو تراكم تكاليف الموارد القياسية والوقت الإضافي إلى تكلفة المهمة.

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


معرف Active Directory (Guid) للموارد.

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


التكاليف المتكبدة للعمل الذي أُنجز بالفعل من قبل الموارد على مهامهم، بالإضافة إلى أي تكاليف مسجلة أخرى مرتبطة بالمهمة.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


التكاليف المتكبدة للعمل الإضافي الذي تم إنجازه بالفعل على المهام بواسطة الموارد المعينة.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


الكمية الفعلية للعمل الإضافي الذي تم إنجازه بالفعل بواسطة المورد المعين للمهام.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


كمية العمل التي يتم من خلالها حماية العمل الإضافي الفعلي.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


كمية العمل التي تم إنجازها بالفعل بواسطة المورد المعين للمهام.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


كمية العمل التي يتم من خلالها حماية العمل الفعلي.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


التكلفة الفعلية للعمل الذي قام به مورد للمشروع حتى الآن.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


اسم مالك التعيين.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


معرف GUID لمالك التعيين.

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


تاريخ البدء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية.

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


تاريخ الانتهاء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


التكلفة المتوقعة للعمل الذي قام به مورد للمشروع حتى الآن.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


تكلفة الميزانية للعمل المجدول لمورد.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


نوع الحجز للمورد.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


تكاليف الميزانية للموارد ذات تكلفة الميزانية. تُعيّن موارد الميزانية فقط إلى مهمة ملخص المشروع.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


عمل الميزانية للموارد ذات عمل الميزانية والموارد المادية. تُعيّن موارد الميزانية فقط إلى مهمة ملخص المشروع.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


تقويم المورد.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


يحدد ما إذا كان يمكن إجراء تسوية الموارد على مورد.

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


الرمز أو معلومات أخرى حول المورد.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


التكلفة الإجمالية المجدولة أو المتوقعة لمورد، استنادًا إلى التكاليف المتكبدة بالفعل للعمل الذي قام به الموارد المعينة للمهام، بالإضافة إلى التكاليف المخطط لها للعمل المتبقي.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


يحدد أي مركز تكلفة يجب تحميل التكاليف المتراكمة للمورد إليه.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


التكلفة التي تتراكم في كل مرة يتم فيها استخدام المورد.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


الفرق بين تكلفة الأساس والتكلفة الإجمالية لمورد.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


التاريخ والوقت الذي تم فيه إضافة المورد إلى المشروع.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


انحراف تكلفة القيمة المكتسبة، حتى تاريخ حالة المشروع. CV هو الفرق بين BCWP (تكلفة العمل المنفذ وفق الميزانية) و ACWP (التكلفة الفعلية للعمل المنفذ).

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


عنوان البريد الإلكتروني للمورد.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


التاريخ الذي من المقرر أن يُكمل فيه المورد العمل على جميع المهام المعيَّنة.

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


المجموعة التي ينتمي إليها المورد.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


يحتوي على رمز التعريف الفريد المُولَّد للمورد.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


العنوان أو النص التوضيحي للرابط المرتبط بالمورد.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


العنوان الخاص بالرابط المرتبط بالمورد.

--------------------

العنوان الكامل (Hyperlink Href في Microsoft Project) للارتباط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


الموقع المحدد في المستند داخل الرابط المرتبط بالمهمة.

--------------------

العنوان الكامل (Hyperlink Href في Microsoft Project) للارتباط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


معرّف الموضع للمورد داخل قائمة الموارد.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


يحدد ما إذا كان المورد قد تم جعله غير نشط بواسطة مستخدم يمتلك صلاحيات إدارية.

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


الأحرف الأولى للمورد.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


يحدد ما إذا كان مورد العمل أو المادة أو التكلفة هو مورد ميزانية.

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


يحدد ما إذا كان المورد هو مورد تكلفة.

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


يظهر ما إذا كان المورد من مجموعة موارد المؤسسة (صحيح) أو من مجموعة الموارد المحلية (خطأ).

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


يحدد ما إذا كان المورد عامًا أم لا.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


يحدد ما إذا كان المورد فارغًا.

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


يظهر ما إذا كان المورد الحالي مورد فريق.

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


وحدة القياس للمورد المادي.

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


الحد الأقصى لعدد الوحدات التي تمثل السعة القصوى التي يتوفر فيها المورد لإنجاز أي مهام خلال الفترة الزمنية الحالية.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


اسم المورد.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


ملاحظات النص بتنسيق RTF.

--------------------

مدعوم لتنسيقات MPP فقط.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


النص العادي للملاحظات المستخرج من بيانات RTF.

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Byte> OVERALLOCATED
```


يشير إلى ما إذا كان المورد مُعيَّنًا لعمل أكثر على مهمة محددة أو جميع المهام مما يمكن إكماله ضمن السعة العمل العادية.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


إجمالي تكلفة العمل الإضافي للمورد على جميع المهام المعيَّنة.

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


معدل الأجر للعمل الإضافي الذي يؤديه المورد.

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


كمية العمل الإضافي المجدولة التي سيؤديها المورد على مهمة ويتم احتسابها وفق معدلات العمل الإضافي للموارد المشاركة.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


الحد الأقصى لوحدة التعيين لمورد في أي لحظة زمنية لجميع المهام التي تم تعيين المورد لها.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


نسبة العمل المكتمل عبر جميع المهام.

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


التهجئة الصوتية لاسم المورد. للاستخدام مع اليابانية فقط.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


إجمالي كمية العمل غير الإضافي المجدول الذي سيؤدى بواسطة المورد.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


المصروف المجدول المتبقي الذي سيتكبد عند إكمال العمل المجدول المتبقي.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


المصروف الإضافي المجدول المتبقي لمورد.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


كمية العمل الإضافي المجدول المتبقية.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


الوقت المتبقي المطلوب لإكمال مهمة أو مجموعة مهام.

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


معدل الأجر للعمل العادي غير الإضافي الذي يؤديه المورد.

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


الوحدات المستخدمة في Microsoft Project لعرض المعدل القياسي.

### START {#START}
```
public static final Key<Date,Byte> START
```


التاريخ الذي يُجدول فيه بدء عمل المورد المعين على مهمة.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


انحراف جدول القيمة المكتسبة، حتى تاريخ حالة المشروع. SV هو الفرق بين BCWP (تكلفة العمل المنفذ وفق الميزانية) و BCWS (تكلفة العمل المجدول وفق الميزانية).

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


نوع المورد.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


المعرّف الفريد للمورد.

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


حساب NT المرتبط بالمورد.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


إجمالي الوقت المجدول للمورد على مهمة.

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


نوع مجموعة العمل التي ينتمي إليها المورد.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


الفرق بين عمل الخط الأساسي للمورد والعمل المجدول الحالي.

