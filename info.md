# Healthcare Information Management and Information Models  
## การจัดการสารสนเทศสุขภาพและแบบจำลองสารสนเทศด้านสุขภาพ

## ภาพรวมรายวิชา

รายวิชานี้มุ่งให้นักศึกษาวิทยาศาสตร์สุขภาพดิจิทัลเข้าใจการจัดการข้อมูลและสารสนเทศสุขภาพในมุมขององค์กร กระบวนการทำงาน มาตรฐานข้อมูล การกำกับดูแลข้อมูล และการบริหารโครงการสุขภาพดิจิทัล โดยเน้นการเรียนรู้แบบปฏิบัติ เพื่อให้นักศึกษาสามารถวิเคราะห์ workflow ออกแบบ information model เบื้องต้น เข้าใจมาตรฐานข้อมูลสุขภาพ และวางแผนโครงการสุขภาพดิจิทัลในระดับหน้างานได้

รายวิชานี้ไม่เน้น SQL, database หรือ data analytics เชิงลึก เนื่องจากมีรายวิชาเฉพาะแยกต่างหากแล้ว แต่เน้นการเชื่อมโยงระหว่างระบบสุขภาพ กระบวนการทำงาน ข้อมูล มาตรฐาน การจัดการโครงการ และการนำระบบไปใช้จริง

---

## Learning Outcomes

เมื่อสิ้นสุดรายวิชา นักศึกษาสามารถ

1. อธิบายบทบาทของข้อมูลและสารสนเทศสุขภาพในองค์กรสุขภาพได้
2. วิเคราะห์ workflow ของงานสุขภาพและระบุจุดที่เกิดข้อมูล จุดใช้ข้อมูล และจุดเสี่ยงของข้อมูลได้
3. วาด diagram พื้นฐานสำหรับสื่อสารงานสุขภาพดิจิทัล เช่น workflow, swimlane, BPMN, system context diagram และ application map ได้
4. อธิบายแนวคิด information model, clinical information model และ health data standards ได้
5. อธิบายแนวคิด EHR, EMR, HIS, HIE, HL7, FHIR, DICOM และ API ในระดับพื้นฐานได้
6. ออกแบบแนวทาง data governance, data stewardship, privacy และ security สำหรับโครงการข้อมูลสุขภาพขนาดเล็กได้
7. วางแผนโครงการสุขภาพดิจิทัลเบื้องต้น โดยใช้ project charter, RACI, WBS, Gantt chart, Kanban และ risk register ได้
8. นำเสนอแผนโครงการจัดการข้อมูลสุขภาพดิจิทัลได้อย่างเป็นระบบ

---

## โครงสร้างรายวิชา 14 ครั้ง

---

# ครั้งที่ 1  
## Introduction to Healthcare Information Management

### เนื้อหา

- ความหมายของ health data, health information และ health knowledge
- ข้อมูลสุขภาพคืออะไร
- ทำไมข้อมูลสุขภาพไม่ได้เป็นแค่ “ตาราง”
- ความสัมพันธ์ระหว่าง service workflow, data, decision, quality และ policy
- บทบาทของ health data manager / digital health practitioner
- ตัวอย่างปัญหาข้อมูลสุขภาพในหน่วยงานจริง

### Workshop

ให้นักศึกษาเลือก 1 งานสุขภาพ เช่น

- คลินิกเบาหวาน
- ER
- งานเภสัชกรรม
- งานคุ้มครองผู้บริโภค
- งานติดตามผู้ป่วยหลังจำหน่าย
- งานนัดหมายวัคซีน

แล้วตอบคำถาม

- งานนี้ใช้ข้อมูลอะไร
- ข้อมูลนี้ใช้เพื่อใคร
- ข้อมูลนี้ใช้ตัดสินใจอะไร
- ถ้าข้อมูลผิดหรือไม่ครบ จะเกิดผลกระทบอะไร

### Output

- Problem statement 1 หน้า

---

# ครั้งที่ 2  
## Health Service Workflow & Data Lifecycle

### เนื้อหา

- Health data lifecycle
  - Collect
  - Validate
  - Store
  - Use
  - Share
  - Archive
  - Destroy
- จุดเกิดข้อมูลในระบบบริการสุขภาพ
- จุดใช้ข้อมูลในระบบบริการสุขภาพ
- ปัญหาที่พบบ่อย
  - ข้อมูลซ้ำ
  - ข้อมูลไม่ครบ
  - ข้อมูลไม่ตรงกัน
  - ไม่มีเจ้าของข้อมูล
  - ข้อมูลไม่ได้ถูกนำไปใช้จริง

### Workshop

- วาด workflow งานสุขภาพแบบง่าย
- ระบุจุดที่เกิดข้อมูลในแต่ละขั้นตอน
- ระบุว่าใครเป็นผู้บันทึก ใครเป็นผู้ใช้ และข้อมูลถูกส่งต่อไปที่ใด

### Output

- Workflow diagram version 1
- Health data lifecycle map

---

# ครั้งที่ 3  
## Value Chain, Value Stream & Stakeholder Analysis

### เนื้อหา

- Value chain คืออะไร
- Value stream คืออะไร
- การมองข้อมูลสุขภาพในฐานะส่วนหนึ่งของการสร้างคุณค่า
- ความแตกต่างระหว่าง “ทำระบบ” กับ “ส่งมอบคุณค่า”
- Stakeholder ในโครงการสุขภาพดิจิทัล
  - Sponsor
  - User
  - Data owner
  - Data steward
  - IT
  - Admin
  - Clinician
  - Patient
  - Project manager

### ตัวอย่าง Value Stream

```text
ผู้ป่วยมารับบริการ 
→ คัดกรอง 
→ ตรวจรักษา 
→ สั่งยา/ตรวจแล็บ 
→ ให้คำแนะนำ 
→ ติดตามผล

Workshop
วาด value chain หรือ value stream ของงานสุขภาพ
ทำ stakeholder map ของ mini project
ระบุว่าแต่ละขั้นตอนต้องใช้ข้อมูลอะไร ใครเป็นเจ้าของข้อมูล และข้อมูลถูกส่งต่อไปไหน
Output
Health value chain map
Stakeholder map
ครั้งที่ 4: Diagram Skills for Digital Health Work
หัวข้อ

Diagram ที่คนทำงานสุขภาพดิจิทัลควรวาดเป็น

Flowchart
Swimlane diagram
Data flow diagram
System context diagram
User journey
Basic architecture diagram
Application map
เครื่องมือที่ใช้ได้
diagrams.net / draw.io
FigJam
Miro free
Canva whiteboard
Google Slides
Workshop

จาก workflow เดิม ให้นักศึกษาแปลงเป็น swimlane diagram โดยระบุ

ใครทำงานตรงไหน
ระบบอะไรเกี่ยวข้อง
ข้อมูลเกิดขึ้นที่ขั้นตอนไหน
ข้อมูลถูกส่งต่อระหว่างใครกับใคร
Output
Swimlane diagram
Initial system context diagram
ครั้งที่ 5: BPMN for Healthcare Workflow
หัวข้อ
BPMN คืออะไร
เหตุผลที่ควรใช้ BPMN ในงานสุขภาพดิจิทัล
BPMN สำหรับการสื่อสารกับทีม IT และทีมหน้างาน
BPMN core symbols
Start event
End event
Task
Gateway
Sequence flow
Pool
Lane
Message flow
Data object
ข้อจำกัดของ BPMN ในงานสุขภาพจริง
ขอบเขตการสอน

สอนเฉพาะระดับที่นักศึกษาสามารถ

อ่าน BPMN ออก
วาด process พื้นฐานได้
ใช้สื่อสาร workflow กับทีมสุขภาพและทีม IT ได้

ไม่จำเป็นต้องสอนลึกถึง

BPMN execution engine
Token simulation
Event หลายชนิด
Subprocess ซับซ้อน
Camunda หรือ automation engine
Workshop
แปลง workflow หรือ swimlane diagram จากครั้งก่อนให้เป็น BPMN แบบง่าย
Output
BPMN diagram ของงานสุขภาพ
ครั้งที่ 6: Enterprise Architecture & Health Information Models
หัวข้อ
Enterprise Architecture เบื้องต้น
การมององค์กรแบบเชื่อมโยง
Strategy
Business
Data
Application
Technology
Business capability ในองค์กรสุขภาพ
ลงทะเบียน
คัดกรอง
ตรวจรักษา
สั่งยา
ตรวจแล็บ
ติดตามผล
รายงาน
Information model คืออะไร
Conceptual model, logical model, physical model
Clinical information model
Common information model
Reference model
ตัวอย่าง entity สำคัญในข้อมูลสุขภาพ
Patient
Encounter
Diagnosis
Medication
Laboratory result
Observation
Provider
Workshop
วาด capability map ของหน่วยงานสุขภาพ
วาด conceptual information model ของงานที่เลือก
Output
Capability map
Conceptual information model
ครั้งที่ 7: EHR, EMR, HIS and Health Information Exchange
หัวข้อ
EMR คืออะไร
EHR คืออะไร
HIS คืออะไร
ความแตกต่างระหว่าง EMR, EHR และ HIS
ระบบย่อยในโรงพยาบาล
OPD
IPD
Pharmacy system
LIS
RIS
PACS
Finance
Appointment system
Health Information Exchange หรือ HIE
ปัญหาข้อมูลไม่เชื่อมกัน
แนวคิด interoperability ในระบบสุขภาพ
Workshop
วาด system context diagram ของโรงพยาบาลหรือหน่วยงานสุขภาพ
ระบุระบบที่ต้องแลกเปลี่ยนข้อมูล
ระบุข้อมูลที่ไหลระหว่างระบบ
Output
System context diagram
Healthcare application map
ครั้งที่ 8: Health Data Standards & Interoperability
หัวข้อ
ทำไมต้องมีมาตรฐานข้อมูลสุขภาพ
ระดับของ interoperability
Technical interoperability
Syntactic interoperability
Semantic interoperability
Organizational interoperability
ตัวอย่างมาตรฐานและรหัสข้อมูลสุขภาพ
ICD
ATC
LOINC
SNOMED CT
HL7
CDA
FHIR
DICOM
IHE
API และ JSON ในภาษาง่าย ๆ
ตัวอย่าง FHIR resource
Patient
Encounter
Observation
MedicationRequest
ขอบเขตการสอน

ไม่จำเป็นต้องให้นักศึกษาเขียน FHIR เอง แต่ควรให้นักศึกษา

อ่านตัวอย่าง FHIR/JSON ได้
เข้าใจว่ามาตรฐานใช้แก้ปัญหาอะไร
คุยกับทีมเทคนิคได้รู้เรื่อง
เข้าใจว่าทำไมระบบสุขภาพต้องใช้รหัสและมาตรฐานร่วมกัน
Workshop
อ่านตัวอย่างข้อมูลผู้ป่วยหรือผลแล็บแบบ JSON
ทำตาราง mapping ว่าข้อมูลแต่ละชนิดควรเกี่ยวข้องกับมาตรฐานใด
Output
Data standard mapping table
FHIR reading worksheet
ครั้งที่ 9: Data Governance, Data Stewardship & Data Quality
หัวข้อ
Data governance คืออะไร
Data stewardship คืออะไร
ความแตกต่างระหว่าง governance และ stewardship
บทบาทสำคัญ
Data owner
Data steward
Data custodian
Data user
Data policy
Data access control
Metadata
Data lineage แบบง่าย
Data quality dimensions
Completeness
Accuracy
Consistency
Timeliness
Validity
Uniqueness
Data quality responsibility
Workshop
ออกแบบ data governance เบื้องต้นของ mini project
ระบุว่าใครมีสิทธิ์ดู เพิ่ม แก้ไข ลบ และนำข้อมูลไปใช้
ตรวจตัวอย่างข้อมูลเพื่อหาปัญหา missing, duplicate และ invalid value
Output
Data governance canvas
Data quality checklist
ครั้งที่ 10: Privacy, Security, PDPA and Ethical Use of Health Data
หัวข้อ
ข้อมูลสุขภาพเป็นข้อมูลอ่อนไหว
หลักการใช้ข้อมูลเท่าที่จำเป็น
Consent
Minimum necessary data
De-identification
Data masking
Access control
Audit trail
Backup
Cyber hygiene สำหรับคนทำงานสุขภาพ
ความเสี่ยงจากการใช้เครื่องมือทั่วไปกับข้อมูลสุขภาพ
Google Sheet
LINE
Email
AI tools
Public link
Ethical use of health data
Unintended consequences ของระบบข้อมูลสุขภาพ
Workshop
วิเคราะห์ case ว่าข้อมูลใดควรเก็บหรือไม่ควรเก็บ
วิเคราะห์ความเสี่ยงจากการใช้ Google Sheet/LINE/AI กับข้อมูลผู้ป่วย
ทำ privacy and security checklist
Output
Privacy & security checklist
Ethical risk note
ครั้งที่ 11: Digital Health Project Management: Charter, RACI and WBS
หัวข้อ
Project vs operation
โครงการสุขภาพดิจิทัลมีลักษณะเฉพาะอย่างไร
Scope, time, cost, quality, risk
Traditional project management
Agile project management
Hybrid project management
Project charter
Work Breakdown Structure หรือ WBS
Milestone
RACI matrix
Responsible
Accountable
Consulted
Informed
Workshop
เขียน project charter ของ mini project
แตกงานเป็น WBS
ทำ RACI matrix
Output
Project charter
WBS
RACI matrix
ตัวอย่าง RACI Matrix
งาน	แพทย์	พยาบาล	เภสัชกร	IT	ผู้จัดการโครงการ
กำหนดข้อมูลที่ต้องเก็บ	C	R	C	C	A
สร้างแบบฟอร์ม	C	C	C	R	A
ตรวจคุณภาพข้อมูล	C	R	C	C	A
ครั้งที่ 12: Gantt Chart, Timeline, Kanban and Modern PM
หัวข้อ
Gantt chart ใช้เมื่อไหร่
Milestone คืออะไร
Dependency
Critical task แบบเข้าใจง่าย
การวางแผนโครงการสุขภาพดิจิทัล 8–12 สัปดาห์
Agile mindset
Kanban board
To do
Doing
Review
Done
WIP limit
Backlog
User story
Sprint แบบเข้าใจง่าย
Hybrid PM
ใช้ Gantt วางภาพรวม
ใช้ Kanban ติดตามงานรายวัน
เครื่องมือฟรี/ง่าย
Google Sheets
Trello
Notion
ClickUp free
Canva table/timeline
GitHub Projects
Workshop
ทำ Gantt chart จาก WBS
สร้าง Kanban board ของโครงการ
เขียน user story อย่างน้อย 5 เรื่อง
Output
Gantt chart
Kanban board
Backlog
User stories
ตัวอย่าง User Story
ในฐานะพยาบาลคลินิก NCD
ฉันต้องการเห็นรายชื่อผู้ป่วยที่ HbA1c สูง
เพื่อให้สามารถติดตามผู้ป่วยกลุ่มเสี่ยงได้เร็วขึ้น
ครั้งที่ 13: Risk Management, Change Management, UX and Implementation
หัวข้อ
ความเสี่ยงของโครงการสุขภาพดิจิทัล
Risk register
Resistance to change
Change management
Training plan
Communication plan
Pilot test
Evaluation
User adoption
Workflow fit
Human-centered design
UX สำหรับระบบข้อมูลสุขภาพ
การลดภาระการกรอกข้อมูล
Form design ที่ดี
Dashboard usability เบื้องต้น
PM ยุคใหม่ต้องบริหาร adoption ไม่ใช่แค่ส่งมอบระบบ
Workshop
ทำ risk register
ทำ change and communication plan
วิเคราะห์ว่า prototype หรือแนวคิดระบบของตนเองเพิ่มภาระผู้ใช้หรือไม่
Output
Risk register
Change & communication plan
Implementation plan
ตัวอย่าง Risk Register
Risk	Impact	Likelihood	Mitigation
ผู้ใช้ไม่กรอกข้อมูลครบ	High	High	ลดจำนวน field และทำ validation
ข้อมูลซ้ำ	Medium	High	ใช้รหัสผู้ป่วยหรือ visit ID
ไม่มีคนดูแลระบบหลังจบโครงการ	High	Medium	กำหนด owner และคู่มือการใช้งาน
ผู้ใช้ไม่ยอมใช้ระบบใหม่	High	Medium	ทำ pilot test และอบรมผู้ใช้ก่อนใช้งานจริง
ครั้งที่ 14: Responsible AI, Data Product Thinking and Final Presentation
หัวข้อ
Data product thinking
Dashboard, registry, alert system และ report ในฐานะ data product
คำถามสำคัญของ data product
ใครคือผู้ใช้
ใช้ตัดสินใจอะไร
ข้อมูลมาจากไหน
refresh บ่อยแค่ไหน
ใครดูแล
success metric คืออะไร
AI-ready data
Responsible AI in health
AI governance
Human-in-the-loop
Bias, fairness, explainability
Model monitoring แบบ concept
การใช้ GenAI กับข้อมูลสุขภาพอย่างปลอดภัย
Final project presentation
Workshop / Final Presentation

นักศึกษานำเสนอ final portfolio ของโครงการ

Final Output

Digital Health Information Management Portfolio ประกอบด้วย

Problem statement
Health data lifecycle map
Workflow diagram
Value chain map
Stakeholder map
Swimlane diagram
BPMN diagram
Capability map
Conceptual information model
System context diagram
Application map
Data standard mapping table
Data governance canvas
Data quality checklist
Privacy & security checklist
Project charter
WBS
RACI matrix
Gantt chart
Kanban board
User stories
Risk register
Implementation plan
Data product concept
Responsible AI consideration
การประเมินผล
รายการ	คะแนน
การมีส่วนร่วมในชั้นเรียน	10
Workshop รายสัปดาห์	25
Diagram assignment: workflow, swimlane, BPMN, context diagram	15
Information model + standards mapping	15
Governance, privacy, security และ data quality assignment	15
Final project portfolio + presentation	20
รวม	100
ชิ้นงานหลักของรายวิชา
Digital Health Information Management Portfolio

ให้นักศึกษาเลือก 1 ปัญหาหน้างานสุขภาพ แล้วจัดทำ portfolio เพื่อแสดงว่าสามารถวิเคราะห์และออกแบบการจัดการสารสนเทศสุขภาพได้อย่างเป็นระบบ

องค์ประกอบของ Portfolio
Problem statement
Stakeholder analysis
Workflow diagram
Swimlane diagram
BPMN diagram
Value chain map
Capability map
Conceptual information model
System context diagram
Application map
Standards mapping
Data governance canvas
Data quality checklist
Privacy/security checklist
Project charter
WBS
RACI matrix
Gantt chart
Kanban board
Risk register
Implementation plan
Responsible AI consideration
เครื่องมือแนะนำสำหรับรายวิชา
งาน	เครื่องมือ
เขียนเอกสารโครงการ	Google Docs, Notion
ทำตาราง RACI / Risk / Gantt	Google Sheets
วาด workflow / BPMN / system diagram	diagrams.net, FigJam, Miro free
ทำ Kanban	Trello, Notion, ClickUp free, GitHub Projects
ทำ mockup / presentation	Canva, Figma, Google Slides
จัดเก็บ portfolio	Google Drive, Notion, Google Sites
ตัวอย่างโจทย์ Mini Project
ระบบติดตามผู้ป่วยเบาหวานในคลินิก NCD
ระบบติดตามการนัดหมายวัคซีน
ระบบจัดการข้อร้องเรียนผลิตภัณฑ์สุขภาพ
ระบบบันทึก medication error
ระบบติดตามผู้ป่วยหลังจำหน่าย
ระบบจัดการข้อมูลเยี่ยมบ้าน
ระบบติดตามการใช้ยาปฏิชีวนะ
ระบบติดตามผลตรวจแล็บผิดปกติ
ระบบติดตามผู้ป่วยกลุ่มเสี่ยงในชุมชน
ระบบข้อมูลสำหรับงานคุ้มครองผู้บริโภค
สรุปแนวคิดของรายวิชา

รายวิชานี้เชื่อมระหว่าง

ระบบสุขภาพ
→ กระบวนการทำงาน
→ ข้อมูล
→ แบบจำลองสารสนเทศ
→ มาตรฐาน
→ การกำกับดูแลข้อมูล
→ การบริหารโครงการ
→ การนำไปใช้จริง

จุดเน้นไม่ใช่การเขียนฐานข้อมูลหรือวิเคราะห์ข้อมูลเชิงสถิติ แต่คือการทำให้นักศึกษาสามารถเข้าใจและจัดการงานข้อมูลสุขภาพในระดับองค์กรและโครงการได้
