<div class="Section1">

<Project Name>

Software Architecture Document

<span style="font-size:
14.0pt;">Version <1.0></span>

_[Note: The following template is provided for use with the Rational Unified Process.  Text enclosed in square brackets and displayed in blue italics (style=InfoBlue) is included to provide guidance to the author and should be deleted before publishing the document. A paragraph entered following this style will automatically be set to normal (style=Body Text).]_

</div>

<div class="Section2">

Revision History

<table style="border-collapse:collapse;
 border:none;" cellspacing="0" cellpadding="0" border="1">

<tbody>

<tr>

<td style="width:1.6in;border:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="154" valign="top">

**Date**

</td>

<td style="width:.8in;border:solid windowtext .75pt;
  border-left:none;padding:0in 5.4pt 0in 5.4pt" width="77" valign="top">

**Version**

</td>

<td style="width:2.6in;border:solid windowtext .75pt;
  border-left:none;padding:0in 5.4pt 0in 5.4pt" width="250" valign="top">

**Description**

</td>

<td style="width:1.6in;border:solid windowtext .75pt;
  border-left:none;padding:0in 5.4pt 0in 5.4pt" width="154" valign="top">

**Author**

</td>

</tr>

<tr>

<td style="width:1.6in;border:solid windowtext .75pt;
  border-top:none;padding:0in 5.4pt 0in 5.4pt" width="154" valign="top">

<dd/mmm/yy>

</td>

<td style="width:.8in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="77" valign="top">

<x.x>

</td>

<td style="width:2.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="250" valign="top">

<details>

</td>

<td style="width:1.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="154" valign="top">

<name>

</td>

</tr>

<tr>

<td style="width:1.6in;border:solid windowtext .75pt;
  border-top:none;padding:0in 5.4pt 0in 5.4pt" width="154" valign="top"> </td>

<td style="width:.8in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="77" valign="top"> </td>

<td style="width:2.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="250" valign="top"> </td>

<td style="width:1.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="154" valign="top"> </td>

</tr>

<tr>

<td style="width:1.6in;border:solid windowtext .75pt;
  border-top:none;padding:0in 5.4pt 0in 5.4pt" width="154" valign="top"> </td>

<td style="width:.8in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="77" valign="top"> </td>

<td style="width:2.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="250" valign="top"> </td>

<td style="width:1.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="154" valign="top"> </td>

</tr>

<tr>

<td style="width:1.6in;border:solid windowtext .75pt;
  border-top:none;padding:0in 5.4pt 0in 5.4pt" width="154" valign="top"> </td>

<td style="width:.8in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="77" valign="top"> </td>

<td style="width:2.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="250" valign="top"> </td>

<td style="width:1.6in;border-top:none;border-left:none;
  border-bottom:solid windowtext .75pt;border-right:solid windowtext .75pt;
  padding:0in 5.4pt 0in 5.4pt" width="154" valign="top"> </td>

</tr>

</tbody>

</table>

**<span style="font-size:18.0pt;font-family:Arial;">  
</span>**

Table of Contents

</div>

<dl>

<dt>

<div class="Section2">[1. <span style="font-size:12.0pt"></span> Introduction](#1\.                  Introduction)         </div>

</dt>

<dd>

<div class="Section2">[1.1 <span style="font-size:12.0pt"></span> Purpose](#1.1               Purpose)     </div>

<div class="Section2">[1.2 <span style="font-size:12.0pt"></span> Scope](#1.2               Scope)     </div>

<div class="Section2">[1.3 <span style="font-size:12.0pt"></span> Definitions, Acronyms and Abbreviations](#1.3               Definitions, Acronyms and Abbreviations)     </div>

<div class="Section2">[1.4 <span style="font-size:12.0pt"></span> References](#1.4               References)     </div>

<div class="Section2">[1.5 <span style="font-size:12.0pt"></span> Overview](#1.5               Overview)     </div>

</dd>

</dl>

<div class="Section2">

[2. <span style="font-size:12.0pt"></span> Architectural Representation](#2\.                  Architectural Representation)

[3. <span style="font-size:12.0pt"></span> Architectural Goals and Constraints](#3\.                  Architectural Goals and Constraints)   

</div>

<dl>

<dt>

<div class="Section2">[4. <span style="font-size:12.0pt"></span> Use-Case View](#4\.                  Use-Case View)</div>

</dt>

<dd>

<div class="Section2">[4.1 <span style="font-size:12.0pt"></span> Use-Case Realizations](#4.1               Use-Case Realizations)     </div>

</dd>

<dt>

<div class="Section2">[5. <span style="font-size:12.0pt"></span> Logical View](#5\.                  Logical View)</div>

</dt>

<dd>

<div class="Section2">[5.1 <span style="font-size:12.0pt"></span> Overview](#5.1               Overview)     </div>

<div class="Section2">[5.2 <span style="font-size:12.0pt"></span> Architecturally Significant Design Packages](#5.2               Architecturally Significant Design Packages)     </div>

</dd>

</dl>

<div class="Section2">

[6. <span style="font-size:12.0pt"></span> Process View](#6\.                  Process View)

[7. <span style="font-size:12.0pt"></span> Deployment View](#7\.                  Deployment View)

</div>

<dl>

<dt>

<div class="Section2">[8. <span style="font-size:12.0pt"></span> Implementation View](#8\.                  Implementation View)</div>

</dt>
<dd>
<div class="Section2">[8.1 <span style="font-size:12.0pt"></span> Overview](#8.1               Overview)     </div>
![](https://github.com/LittleBeasts/documentation/blob/master/classDiagram.svg)

<div class="Section2">[8.2 <span style="font-size:12.0pt"></span> Layers](#8.2               Layers)     </div>

</dd>

</dl>

<div class="Section2">

[9. <span style="font-size:12.0pt"></span> Data View (optional) ](#9\.                  Data View (optional))      

[10. <span style="font-size:12.0pt"></span> Size and Performance](#10\.             Size and Performance)               

[11. <span style="font-size:12.0pt"></span> Quality](#11\.             Quality)               

Software Architecture Document

#### <font face="Arial, Helvetica, sans-serif"><a name="1\.                  Introduction">1.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Introduction</a></font>

[The introduction of the **Software Architecture Document** should provide an overview of the entire **Software Architecture Document**. It should include the purpose, scope, definitions, acronyms, abbreviations, references, and overview of the **Software Architecture Document**.]

##### <font face="Arial, Helvetica, sans-serif"><a name="1.1               Purpose">1.1<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Purpose</a></font>

This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.

[This section defines the purpose of the **Software Architecture Document**, in the overall project documentation, and briefly describes the structure of the document. The specific audiences for the document should be identified, with an indication of how they are expected to use the document.]

##### <font face="Arial, Helvetica, sans-serif"><a name="1.2               Scope">1.2<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Scope</a></font>

[A brief description of what the Software Architecture Document applies to; what is affected or influenced by this document.]

##### <font face="Arial, Helvetica, sans-serif"><a name="1.3               Definitions, Acronyms and Abbreviations">1.3<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Definitions, Acronyms and Abbreviations</a></font>

[This subsection should provide the definitions of all terms, acronyms, and abbreviations required to properly interpret the **Software Architecture Document**.  This information may be provided by reference to the project Glossary.]

##### <font face="Arial, Helvetica, sans-serif"><a name="1.4               References">1.4<span style="font:7.0pt &quot;Times New Roman&quot;"></span> References</a></font>

[This subsection should provide a complete list of all documents referenced elsewhere in the **Software Architecture Document**. Each document should be identified by title, report number (if applicable), date, and publishing organization. Specify the sources from which the references can be obtained. This information may be provided by reference to an appendix or to another document.]

##### <font face="Arial, Helvetica, sans-serif"><a name="1.5               Overview">1.5<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Overview</a></font>

[This subsection should describe what the rest of the **Software Architecture Document** contains and explain how the **Software Architecture Document** is organized.]

#### <font face="Arial, Helvetica, sans-serif"><a name="2\.                  Architectural Representation">2.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Architectural Representation</a></font>

[This section describes what software architecture is for the current system, and how it is represented. Of the **Use-Case**, **Logical**, **Process**, **Deployment**, and **Implementation Views**, it enumerates the views that are necessary, and for each view, explains what types of model elements it contains.]

#### <font face="Arial, Helvetica, sans-serif"><a name="3\.                  Architectural Goals and Constraints">3.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Architectural Goals and Constraints</a></font>

[This section describes the software requirements and objectives that have some significant impact on the architecture, for example, safety, security, privacy, use of an off-the-shelf product, portability, distribution, and reuse. It also captures the special constraints that may apply: design and implementation strategy, development tools, team structure, schedule, legacy code, and so on.]

#### <font face="Arial, Helvetica, sans-serif"><a name="4\.                  Use-Case View">4.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Use-Case View</a></font>

[This section lists use cases or scenarios from the use-case model if they represent some significant, central functionality of the final system, or if they have a large architectural coverage - they exercise many architectural elements, or if they stress or illustrate a specific, delicate point of the architecture.]

##### <font face="Arial, Helvetica, sans-serif"><a name="4.1               Use-Case Realizations">4.1<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Use-Case Realizations</a></font>

[This section illustrates how the software actually works by giving a few selected use-case (or scenario) realizations, and explains how the various design model elements contribute to their functionality.]

#### <font face="Arial, Helvetica, sans-serif"><a name="5\.                  Logical View">5.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Logical View</a></font>

[This section describes the architecturally significant parts of the design model, such as its decomposition into subsystems and packages. And for each significant package, its decomposition into classes and class utilities. You should introduce architecturally significant classes and describe their responsibilities, as well as a few very important relationships, operations, and attributes.]

##### <font face="Arial, Helvetica, sans-serif"><a name="5.1               Overview">5.1<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Overview</a></font>

[This subsection describes the overall decomposition of the design model in terms of its package hierarchy and layers.]

##### <font face="Arial, Helvetica, sans-serif"><a name="5.2               Architecturally Significant Design Packages">5.2<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Architecturally Significant Design Packages</a></font>

[For each significant package, include a subsection with its name, its brief description, and a diagram with all significant classes and packages contained within the package.

For each significant class in the package, include its name, brief description, and, optionally a description of some of its major responsibilities, operations and attributes.]

#### <font face="Arial, Helvetica, sans-serif"><a name="6\.                  Process View">6.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Process View</a></font>

[This section describes the system's decomposition into lightweight processes (single threads of control) and heavyweight processes (groupings of lightweight processes). Organize the section by groups of processes that communicate or interact. Describe the main modes of communication between processes, such as message passing, interrupts, and rendezvous.]

#### <font face="Arial, Helvetica, sans-serif"><a name="7\.                  Deployment View">7.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Deployment View</a></font>

[This section describes one or more physical network (hardware) configurations on which the software is deployed and run. It is a view of the Deployment Model. At a minimum for each configuration it should indicate the physical nodes (computers, CPUs) that execute the software, and their interconnections (bus, LAN, point-to-point, and so on.) Also include a mapping of the processes of the **Process View** onto the physical nodes.]

#### <font face="Arial, Helvetica, sans-serif"><a name="8\.                  Implementation View">8.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Implementation View</a></font>

[This section describes the overall structure of the implementation model, the decomposition of the software into layers and subsystems in the implementation model, and any architecturally significant components.]

##### <font face="Arial, Helvetica, sans-serif"><a name="8.1               Overview">8.1<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Overview</a></font>

[This subsection names and defines the various layers and their contents, the rules that govern the inclusion to a given layer, and the boundaries between layers. Include a component diagram that shows the relations between layers. ]

##### <font face="Arial, Helvetica, sans-serif"><a name="8.2               Layers">8.2<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Layers</a></font>

[For each layer, include a subsection with its name, an enumeration of the subsystems located in the layer, and a component diagram.]

#### <font face="Arial, Helvetica, sans-serif"><a name="9\.                  Data View (optional)">9.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Data View (optional)</a></font>

[A description of the persistent data storage perspective of the system. This section is optional if there is little or no persistent data, or the translation between the Design Model and the Data Model is trivial.]

#### <font face="Arial, Helvetica, sans-serif"><a name="10\.             Size and Performance">10.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Size and Performance</a></font>

[A description of the major dimensioning characteristics of the software that impact the architecture, as well as the target performance constraints.]

#### <font face="Arial, Helvetica, sans-serif"><a name="11\.             Quality">11.<span style="font:7.0pt &quot;Times New Roman&quot;"></span> Quality</a></font>

[A description of how the software architecture contributes to all capabilities (other than functionality) of the system: extensibility, reliability, portability, and so on. If these characteristics have special significance, for example safety, security or privacy implications, they should be clearly delineated.]

</div>

<font size="1" face="Arial">![](../../../applet/images/artfc_w.gif) [Artifacts](../../../process/artifact/ovu_arts.htm) > ![](../../../applet/images/artfc_y.gif) [Analysis & Design Artifact Set](../../../process/artifact/ars_dsg.htm) > ![](../../../applet/images/ar_doc.gif) [Software Architecture Document](../../../process/artifact/ar_sadoc.htm) > ![](../../../applet/images/ie.gif) rup_sad.htm</font>
