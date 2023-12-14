---
layout: default
title: XML S1000D Docs
parent: XML S1000D
nav_order: 1
---

# XML S1000D Docs
{: .fw-600 }
{: .no_toc }

This section aims to present my extensive experience in producing XML S1000D manuals for aircraft systems in Simplified Technical English (STE).
{: .fs-6 .fw-300 }

---

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

{: .important }
> Although I have worked on a wide range of technical documentation in a variety of projects, some examples of content from previous projects **cannot be made publicly available** due to corporate intellectual property, non-disclosure agreements, and export control restrictions. If you would like to discuss specific past projects and deliverables in more detail, please contact me at the [Resume contact section](https://franmaral.github.io/resume/resume.html).

## Introduction

With over 16 years of experience in end-to-end S1000D technical writing with civil and military aerospace OEMs, I have extensively applied the concepts of information management, information sets, data modules, publication modules, technical content optimisation and common information repositories to aircraft system manuals and IETMs.

<img src="/portfolio/assets/images/IETM_webscreen.jpeg" alt="XML arbortext editor" width="350" height="350">

For example, I have authored onboard system software test and troubleshooting procedures for flight control units, created standard test equipment maintenance guides describing diagnostic suite interfaces and fault logging methodology, and developed XML authoring practices aligned with business rules and customisations for change integration.

## XML Technical Writer Career

Throughout my years as an XML technical writer, I have been fortunate to progress through roles covering aviation quality assurance, project coordination or managing teams working on aircraft systems documentation.

<img src="/portfolio/assets/images/S1000D-descript.png" alt="XML arbortext editor" width="500" height="500">

Though deeply technical, my collaborative yet empathetic nature has allowed me to thrive not only through individual contributions, but also by enabling those around me to excel. I remain curious and have continued to seek both formal and informal learning on everything from digital mockup visualisation to coding or team management.

### Roles

Through increasingly challenging roles, I have honed a multi-faceted skill set that includes advanced XML documentation, quality control processes, project coordination and team mentoring. See below for a summary of my roles:

```
    2007 - 2008     Technical Illustrator
    2008 - 2009     Technical Author
    2009 - 2014     Incoming Inspector
    2014 - 2022     Manual Manager and RFC Lead
    2023 - Present  TID Support
```

### Project Details

| Projects        | Tools                            | Description |
|-----------------|----------------------------------|-------------|
| Illustration    | cgm, 3D, PView, Isoview, Illustrator | Created complex equipment diagrams, schematics, and 3D models using technical illustration software to visually represent aviation components and systems. |
| Catalogue         | Stilo, Sprint, Airn@v              | Organised extensive parts catalogue spanning thousands of aircraft hardware SKUs ensuring data integrity, simplification, and searchability across items. |
| Repair          | SGML, Arbortext, IDS, Sprint, Airn@v | Led team authoring detailed aviation maintenance and repair manuals while ensuring precise representation of fault limits, tolerances procedures for technicians. |
| Maintenance     | SGML, Arbortext, IDS, Sprint, PDF    | Managed group producing onboard system software descriptions, diagnostic test procedures, and maintenance guides for avionics units and flight control systems. |
| Fault Isolation | XML, Arbortext, IDS, Sprint, IETM    | Provided ongoing publication support through continuous stakeholder collaboration, in-depth analysis, strategic planning, and communication facilitation to aid documentation decisions. |

For more information, visit my [Resume](https://franmaral.github.io/resume/resume.html).

## Technical Publications

My responsibilities as an XML Technical Writer were the end-to-end creation and management of aircraft maintenance documentation in accordance with technical publication guidelines. Key tasks included the following:

- Planning publications based on data and SME input
- Interacting with engineers and operators to gather specifications
- Analysing aircraft interface control documentation
- Writing configuration control
- Structuring content through information modelling
- Launch illustration and author work orders
- Authoring modules using S1000D standards
- Enforcing Simplified Technical English checks
- Performing quality validation on QA tools
- Publish and distribute system manuals on PDFs and IETMs
- Preparing training material on best practice in technical writing.

## XML S1000D

My technical writing expertise lies in designing the required information architecture, creating a modular XML structure using elements such as topic, section, table, etc., writing the content, embedding semantic markup through attributes, ensuring compliance with specification standards, and publishing for multiple deliveries including PDF and IETMs.

<img src="/portfolio/assets/images/Publications.png" alt="XML S1000D Publications" width="500" height="500">


XML authoring for structured content creation was a core skill I used extensively. As an example, this is a fragment of an operational test data module written in XML according to the S1000D scheme (from [www.w3.org](http://www.w3.org/)):

```xml
<dmodule xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    ...
    <procedure>
    <figure id="fig-0001"><title>PDLMC Operational Test</title>
    <graphic infoEntityIdent="ICN-AAA-DA52000-0-U8025-00523-A-04-1"/></figure>
    <title>Operational Test</title>
    <proceduralStep>
        <para>Make sure that none of the messages that follow are shown:</para>
        <randomList listItemPrefix="pf01">
        <listItem><para>PDLMC 1 FAIL (Advisory)</para></listItem>
        <listItem><para>PDLMC 2 FAIL (Advisory)</para></listItem>
        <listItem><para>PDLMC 1 FAIL (Status)</para></listItem>
        <listItem><para>PDLMC 2 FAIL (Status)</para></listItem>
        </randomList>
        <note><notePara>The PDLMC 3 OFF (Status) message will be shown as a result.</notePara></note>
    </proceduralStep>
    <proceduralStep applicRefId="apMK1">
        <proceduralStep><para>Before each flight, start the <internalRef internalRefId="seq-0003" internalRefTargetType="irtt05"/> APU 
        <internalRef internalRefId="sup-0002" internalRefTargetType="irtt04"/> and make sure that generator is operative.</para></proceduralStep>
        <proceduralStep><para>APU is operated continuously during flight.</para>
        </proceduralStep>
        <figure id="fig-0001">
        <proceduralStep><para>Push the CMD APR 1. <internalRef internalRefId="sup-0002" internalRefTargetType="irtt04"/>Make sure that all messages are removed.</para></proceduralStep>
        <proceduralStep><para>Rotate the knob, CC21, to select ENG 1.</para></proceduralStep>
        <proceduralStep applicRefId="apMK9"><para>If any of the ANTI-ICE warning is shown <internalRef
        internalRefId="seq-0003" internalRefTargetType="irtt05"/> into <internalRef internalRefId="sup-0003" internalRefTargetType="irtt04"/> move the switch TD4 to off position.</para></proceduralStep>
        <proceduralStep><para>In the Main Menu, select ENG PDLMC Conf 1.</para></proceduralStep>
        <proceduralStep><para>On <internalRef internalRefId="seq-0003" internalRefTargetType="irtt05"/> ENG Parameters <internalRef internalRefId="sup-0002" internalRefTargetType="irtt04"/> select ENG 2.</para></proceduralStep>
        <proceduralStep><para>APU generator is verified operative.</para></proceduralStep>
        <proceduralStep><para>Fully complete the ENG 1 and ENG 2 cycle before landing.</para></proceduralStep>
        <proceduralStep><para>Select ENG EFC function to remove all fault codes in the ENG CTRL menu.</para></proceduralStep>
        </proceduralStep>
    </procedure>
    ...
</dmodule>
```

A major part of my role involved the modular authoring of XML topics and data modules to enable content reuse across documentation deliverables. This required conceptualising, structuring and interlinking aircraft system data through a network of XML elements containing technical details. I used reusable data modules with controlled metadata to insert and assemble procedures, equipment descriptions, maintenance data and troubleshooting steps.

My expertise includes advanced XML architectures, automated cross-referencing, repository attribute keys, configuration control management, inline effectivity, and building QA deliverables through tailored validation VBA scripts. 

<img src="/portfolio/assets/images/S1000d-Process.png" alt="XML S1000D Publications" width="500" height="500">

I enforced integrity checks within the XML code to meet customer-specific customisations, while coordinating between authors and engineering teams to synchronise documents with system upgrades and specification changes. The aim was to optimise content for multiple outputs including IETMs, PDFs for tablets and web delivery via CCMS.

## ASD STE-100

This is a controlled grammar and vocabulary standard made for non-native English users in aviation. Through numerous projects standardising documentation for training technicians, my STE skills aid technical comprehension across global readership.

<img src="/portfolio/assets/images/json-gui-term-checker.png" alt="XML S1000D Publications" width="600" height="600">

## Communication

As Technical Writer, clear and empathetic communication marks effective coordination across teams critical for project success. My typical week would witness touchpoints through emails, calls and remote sessions with various stakeholders like engineers, customers, illustrators, training developers and reviewers:

- I leveraged tools like Teams, Google Meet, Cisco and Zoom for daily stand-ups with offshore writing teams to unblock issues through collaborative troubleshooting. 

- Session recordings aided asynchronous progress monitoring. 

- I frequently conducted SME interviews to analyse aircraft software and understand failure scenarios, while whiteboarding flowcharts ensured all details were captured. 

- Conversations were summarised through meeting minutes and circulated for common understanding. 

My working style balanced technical precision with active listening to address concerns, manage expectations and maintain amicable relationships with advisors involved in publication sign-offs.

<img src="/portfolio/assets/images/ata-2200.jpg" alt="XML arbortext editor" width="500" height="500">

As RFC Focal Point, I demonstrated specialist customer relationship management by continually engaging with stakeholders to understand change requests. I acted as a communication bridge, resolving release change requests, clarifying specifications, and realigning deliverables to meet dynamic requirements while meeting adjusted deadlines.

I look forward to channelizing these well-rounded communication abilities for bolstering documentation quality and timely, within-budget deliveries.

## Research and Analysis

My analytical approach has been vital in projects involving vast amounts of complex, interdependent data. Cataloguing and tracking thousands of aircraft equipment parts requires meticulous attention to detail to avoid inconsistencies.

Equally important is the efficient parsing of vast quantities of system documents, interface control sheets, test specifications and software fault code logs to produce technical publications under the tightest of regulatory conditions.

<img src="/portfolio/assets/images/Gantt_S1000D.PNG" alt="XML arbortext editor" width="400" height="400">

I use my organisational skills to map information in a structured way, filter data correlations, and prioritise topic clusters. For example, fault isolation requires an understanding of cascading software-hardware interactions. I have been able to reconstruct such failure linkages into troubleshooting flows. 

Through research skills that include data mining, conceptual linkages, and visualisation of relationships, I bring clarity to technical complexity for users.

## Editor and Proofreader

Careful editing of all publications to ensure continuous content improvement according to quality frameworks such as EN ISO 9100, ATA 100/iSpec 2200 and S1000D. Internally benchmarked procedures have helped achieve zero audit findings.

<img src="/portfolio/assets/images/iso-en_9100.png" alt="XML arbortext editor" width="150" height="150">

Adopt a perfectionist, error-finding approach to proofreading. Rigorously examine documents through multiple reviews under tight deadlines, looking for errors in terminology, grammar and formatting consistency.

## Team Manager

On two opportunities, provided strategic leadership to a team of over 15 technical writers, engineers and graphic illustrators working on aircraft systems documentation projects.

Using agile methodologies, promoted a collaborative working culture that balanced individual skill building with shared accountability for publication quality. Established mentoring framework for writers, leveraging expertise of senior illustrators and peer feedback channels.

<img src="/portfolio/assets/images/projects-agile.PNG" alt="XML arbortext editor" width="400" height="400">

## Wrapping up

My broad yet specialised publication skills now seek new applications in software and technology, where user empathy and simplification are essential. I hope we can explore documentation opportunities where both my technical writing insider knowledge and thirst for mastery find renewed purpose.