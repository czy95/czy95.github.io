## 复习老板的BIM课
[Canvas链接](https://access.ust.hk/cas/login?client_name=Student+%2F+Staff+%2F+Project&ticket=ST-296501-1xlfQ2m10wn7DnedfkE2mekFL-scas1) 

### 10.2课
- All major public project exceeding HKD 30M should use BIM from 1/1/2018
- ***Current Adoption***
  - 建筑结构设计
  - virtual mock-ups ( digital stell fabrication, visualization on site)
  - [例如](/static/img/10271.JPG)
  - constructability
  - clash detection
  - engineering analysis(plugin for structural, lighting, mechanical, energy..)
    - Dynamo+Formlt (computational design), robot structural, LEED, civil 3d, CFD(for natural ventilation)
* ***What is BIM***
  - 3D,consistency check, project/product,(cost, schedule, lighting, analysis..)
  - It is object-based info(geometry) 和sketchup不同，每个物体都是一个对象
  - nD (time, cost, sus, facility mgt, safety..)
  - BIM Can have differenr modes
    - open/closed, little/big –> open big BIM
* ***LoD***
  - Level of development,level of detail.
  - LoD-G,graphical details，LoD-I, information richness
* ***Standards***
  - 降低沟通成本。BIM is not only about people: people, tech, process.
  - Project level: BIM Project Execution Plan (BEP)
    - 包含terminology, background, LoD…
  - Organization/Corporate level: CIC, HK housing authority
    - naming, color convention, LOD respon matrix
  - regional/national level:
    - GB, singapore BIM guide, National BIM Standards(USA)
* ***Products: BIM Model***
  - Data exchange standards
  - Industry Foundation Classes(IFC), 最新版IFC4 (766 Entities, 391 types)
    - open and neutral data formate to describe, exchange and share information in AEC and FM
    - by buildingSMART International (International Alliance for Interoperability [IAI] before 2005)
    - **IFC data model is object-oriented (elements, shapes, processes etc..)**
    - registered by ISO
    - 在GIS和Green Building的基础上，保留/修改/增加了一些
  - Practical Design using IFC
    - DMS: document management system, IFC Model Server
    - skecthing, HVAC, FM, Structual, Electrical…
  - IFC Schema Format
    - **IFC-EXPRESS, ifcXML**. both are ISO
    - Two types of attribute: (1) element ID; (2) values (string,numerical, enumeration, empty)
    - Free Softwarehttp://www.ifcwiki.org/index.php/Freeware, FZK Viewer, BIM Vision, Solibri
