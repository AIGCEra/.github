<h1 align=center>

[Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)
</h1>
<h3 align=center><div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="100%" /></div>(In most scenarios, Desktop Software is like a Universe, with many huge local worlds hidden around numerous child windows, and the Web Runtime is a space telescope, revealing the depths of the universe that have been hidden from the developer's sight...)
</h3>

<h1 align=center>
The Core Job of Web Runtime:<br><i>Eliminate</i> the <i>Gap</i> between <i>Desktop Software</i> and <i>Web Browser</i>
</h1>
<h2>
<p>The Web Runtime provides developers with a <p align=center>"<i>Simplest Technical Strategy</i>"</p> <ins>to convert an "existing" or "newly created" <i>Desktop Software Project</i> into "<i>Browser Process</i>" of "Chromium Project"</ins>, thus realizing Web pageization of "Desktop Application Functions", it will completely eliminate the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and make Web Technology an inherent part of <i>Desktop Software Architecture</i>.
</p>
</h1> 

<div align=center>

# [Converting WinForm Application <br>into Chromium Project Browser Process](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)
  
## (1)Prepare a C# WinForm Project<br>(create a new Project, or open an existing Project)
</div>
<h3>Reference “cosmos.dll”, adjust manifest and compilation configurations</h3>


<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/183294437-cf6a3f96-69ed-4274-936c-ba963e21537d.jpg" width="100%"/></div>

<h2 align=center><p>(2)Open "program.cs" file.</p> <p align=left><i>Modify main function</i>, Replace: "Application.Run" with:<p align=center>Universe.WebRT.Run</p></p>
</h2>

<div align=center>

# [Converting MFC Application <br>into Chromium Project Browser Process](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)
  
<div align=center>

## (1)Prepare a MFC Project <br>(create a new Project, or open an existing Project)
<div align=center>

<h3 align=left>
<p>
  
Copy all files included with [***MFCPlus***](https://github.com/TangramDev/OpenWebRunTime/tree/master/src/sdk/MFCPlus) into the prepared MFC Desktop Software Project. Open the "pch.h(pch.cpp)" or "stdafx.h(stdafx.cpp)" file of the developer's desktop software project, add the following code at the end of the opened file at a suitable position:</p>
<p align=center>#include "WebRuntimeApp.h" // for pch.h or stdafx.h</p>
<p align=center>#include "WebRuntimeApp.cpp" // for pch.cpp or stdafx.cpp</p><br>	
	
<p>
<div align=center id="mfcdevmanifest"><img src="https://user-images.githubusercontent.com/26355688/183295042-d9f37362-9761-41a2-9f11-c93663bae44f.jpg" width="100%"/></div>
</p>	
</h3>
<hr />

## (2)Code Modifications
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Code modification</strong>
                    <th> <strong>Description</strong>
                </tr>                     
            <tbody>
                <tr>
                    <td width="30%">
                        <strong><p align=center>Modify Base Class</strong> </p>
                    </td>
                    <td width="70%">
		     <strong><p>For AppBase, Replace "public CWinApp(Ex)" with: <p align=center>public CWebRTApp(Ex)</p></p><p>For MDIFrameBase, Replace "public CMDIFrameWndEx" with: <p align=center>public CWebRTMDIFrame</p></p></strong>
                    </td>
            </tbody>
	    <tbody>
                <tr>
                    <td width="30%">
                        <strong><p align=center>Dialog Application</strong> </p>
                    </td>
                    <td width="70%">
		     <strong><p>Modify the return value of</p><p><div align=center>BOOL CMFCDlgApp::InitInstance()</p><p align=left>to</p> <p align=center>TRUE</strong>.</p>
                        </p></strong>
                    </td>
            </tbody>	    
	    <tbody>
                <tr>
                    <td class="sunnysolution" width="30%">
                        <strong><p align=center>Document Serialization</p></strong>
                    </td>
                    <td class="sunnysolution" width="50%">
		      <strong>
                      </p>
                        <p>Add the following serialization code in the body of the Serialize (CArchive & ar) function:                            
                        </p>
                      <p>                   
                      
    void CMFCApplicationDoc::Serialize(CArchive& ar){
	  if (ar.IsStoring())
	  {
		  ar << theApp.GetDocTemplateID(this);
	  }
	  else
	  {
		  ar >> theApp.m_strCreatingDOCID;
	  }
    }
</p>
</strong>
                    </td>
            </tbody>
        </table>
</center>

<h1 align=center>
Ushering in the Era of the <i>Web-Defining Desktop Window</i>
</h1>
<h2>
<p  align=left>The Web Runtime believes the <i>Expressive</i>, <i>Comprehensive</i>, and <i>Powerful</i> Desktop Windows are composed by using the traditional Web DOM to describe various programmable objects (COM, .Net controls, Win32 windows, etc.), rather than created through complex code technology. This is the key reason to the conversion of the Main Process of Desktop Software into a Browser Process. Describing as many objects as possible with the Web DOM is the basic principle of Web Runtime.
</p> 

<p><div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181908801-0910fdc6-23b6-457e-bf30-76cfc66097d3.gif" width="80%" /><br>(The Era of "Web Page Define Desktop Window")</div>
</p>

<p align=left>Desktop applications are about to usher in the "<i>Web Page Define Desktop Window</i>" era, in this sense, Desktop Web Browser should be the "<i>Smallest Desktop Application</i>". When developers can reinterpret the specific UI presentation of Web pages, the boundaries between browsers and desktop applications completely disappear.</p>
       
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/readmeex.md)
</div>
</h1>
