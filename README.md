# 🎓 Internship Aggregator Platform

[![GitHub Issues](https://img.shields.io/github/issues/EngMohamedElabsy/Project?color=blue)](https://github.com/EngMohamedElabsy/Project/issues)
[![GitHub PRs](https://img.shields.io/github/issues-pr/EngMohamedElabsy/Project?color=green)](https://github.com/EngMohamedElabsy/Project/pulls)
[![Project Board](https://img.shields.io/badge/Board-Project%20Kanban-orange)](https://github.com/users/EngMohamedElabsy/projects/3)

منصة مركزية ذكية لربط الطلاب بالفرص التدريبية والتدريب الصيفي لدى الشركات، مبنية باتباع أفضل ممارسات هندسة البرمجيات (Software Engineering Best Practices) ومعايير إدارة المتطلبات Agile / Scrum.

---

## 📌 عن المشروع (Problem & Solution)

### ❓ المشكلة:
يعاني طلاب الجامعات سنوياً من تشتت فرص التدريب العملي بين منصات متعددة، ومجموعات التواصل الاجتماعي، وصعوبة متابعة حالة طلبات التقديم، بينما تواجه الشركات صعوبة في فرز وإدارة طلبات المتقدمين في مكان واحد منظم.

### 💡 الحل:
منصة موحدة تجمع كل الأطراف وتتيح:
1. **للطلاب:** استكشاف التدريبات المناسبة لمهاراتهم، التقديم بنقرة واحدة باستخدام السيرة الذاتية، ومتابعة فورية لحالة الطلب.
2. **للشركات / أصحاب العمل:** نشر إعلانات التدريب، استقبال وفرز المرشحين، واتخاذ قرارات القبول/الرفض بسهولة.
3. **للإدارة:** مراقبة جودة التدريبات وإحصائيات المنصة وحماية الطلاب من الحسابات والتدريبات الوهمية.

---

## 👥 أدوار النظام (User Roles)

* 👨‍🎓 **الطالب (Student):** إنشاء الحساب، تعديل الملف الشخصي، البحث عن التدريبات والتقديم عليها ومتابعة حالتها.
* 🏢 **صاحب العمل (Employer):** نشر فرص التدريب، مراجعة طلبات التقديم وسير المتقدمين، وتحديث قرارات القبول والرفض.
* 🛡️ **مسؤول النظام (Admin):** إدارة الحسابات، تعطيل الحسابات المخالفة/المزعجة، ومتابعة تقارير نمو المنصة.

---

## 📋 مصفوفة المتطلبات وقصص المستخدم (User Stories Matrix)

تم توثيق وهندسة المتطلبات بالكامل وفقاً لمنهجية **MoSCoW Prioritization**:

| الكود | قصة المستخدم (User Story) | الأولوية | الـ Issue على GitHub |
|:---:|:---|:---:|:---:|
| **US-01** | تسجيل حساب طالب جديد | **Should** | [#1](https://github.com/EngMohamedElabsy/Project/issues/1) |
| **US-02** | تعديل وإدارة الملف الشخصي | **Could** | [#2](https://github.com/EngMohamedElabsy/Project/issues/2) |
| **US-03** | استعادة وتعيين كلمة المرور | **Must (MVP)** | [#3](https://github.com/EngMohamedElabsy/Project/issues/3) |
| **US-04** | تسجيل الدخول للوحة التحكم | **Must (MVP)** | [#5](https://github.com/EngMohamedElabsy/Project/issues/5) |
| **US-05** | البحث المتقدم عن التدريبات بالاسم والشركة | **Must (MVP)** | [#6](https://github.com/EngMohamedElabsy/Project/issues/6) |
| **US-06** | التقديم على فرصة تدريب بالسيرة الذاتية | **Must (MVP)** | [#7](https://github.com/EngMohamedElabsy/Project/issues/7) |
| **US-07** | نشر فرصة تدريب جديدة بواسطة الشركة | **Must (MVP)** | [#8](https://github.com/EngMohamedElabsy/Project/issues/8) |
| **US-08** | مراجعة قائمة المتقدمين للتدريب | **Should** | [#9](https://github.com/EngMohamedElabsy/Project/issues/9) |
| **US-09** | تغيير حالة الطلب (قبول / رفض) | **Must (MVP)** | [#10](https://github.com/EngMohamedElabsy/Project/issues/10) |
| **US-10** | تتبع حالة الطلبات المقدمة للطلاب | **Should** | [#11](https://github.com/EngMohamedElabsy/Project/issues/11) |
| **US-11** | إيقاف حسابات الشركات المخالفة | **Should** | [#12](https://github.com/EngMohamedElabsy/Project/issues/12) |
| **US-12** | تقارير إحصائية للتدريبات النشطة | **Could** | [#13](https://github.com/EngMohamedElabsy/Project/issues/13) |

---

## 🚀 نطاق النسخة الأولية (MVP Scope)

تشمل النسخة الأولى الأساسية العمليات الضرورية لتشغيل المنصة بنجاح:
* **نطاق الـ MVP المعتمد:** `US-03`, `US-04`, `US-05`, `US-06`, `US-07`, `US-09`.
* **المتطلب غير الوظيفي الإلزامي:** `NFR-02` (تشفير وتجزئة كلمات المرور باستخدام bcrypt).
* باقي القصص (`Should` و `Could`) تظل في الـ Backlog للتطوير في المراحل القادمة.

---

## ⚙️ معايير الجودة والقبول (Acceptance Criteria & DoD)

* كل قصة مستخدم موثقة ومربوطة بسيناريوهات **Gherkin BDD** (`Given / When / Then`).
* تم تحديد المتطلبات غير الوظيفية (**NFRs**) مثل الأداء والحماية ومعدل الجاهزية.
* التوثيق الشامل متاح بالكامل في: [`docs/requirements.md`](docs/requirements.md).

---

## 📊 لوحة إدارة المشروع (Project Kanban Board)

لمتابعة سير العمل والتطوير خطوة بخطوة:
👉 [**Internship Platform Board**](https://github.com/users/EngMohamedElabsy/projects/3)
* 🔵 **To Do:** قائمة المهام والقصص قيد الانتظار.
* 🟡 **To Program:** المهام التي يجري تطويرها حالياً.
* 🟢 **Done:** الميزات المكتملة والمختبرة.

---

## 👨‍💻 المساهمون والمطورون
* **Mohamed Elabsy** - [@EngMohamedElabsy](https://github.com/EngMohamedElabsy)
