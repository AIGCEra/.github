<h1 align=center>

[Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)
</h1>
<h3 align=center><div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="100%" /></div>(In most scenarios, Desktop Software is like a Universe, with many huge local worlds hidden around numerous child windows, and the Web Runtime is a space telescope, revealing the depths of the universe that have been hidden from the developer's sight...)
</h3>

<h1 align=center>
The Core Job of Web Runtime:<br><i>Eliminate</i> the <i>Gap</i> between <i>Desktop Software</i> and <i>Web Browser</i>
</h1>
<h2>
<p>The Web Runtime provides developers with a <p align=center>"<i>Simplest Technical Strategy</i>"</p> <ins>to convert an "existing" or "newly created" <i>Desktop Software Project</i> into "<i>Browser Process</i>" of "Chromium Project"</ins>, thus realizing Web pageization of "Desktop Application Functions", it completely bridges the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and make Web Technology an inherent part of <i>Desktop Software Architecture</i>.
</p>
</h1> 

<div align=center>

# [Converting WinForm Application <br>into Chromium Project Browser Process](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)
	
<p>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>First Step</strong>
                    <th> <strong>Second Step</strong>
                </tr>                     
            <tbody>
                <tr>
                    <td width="75%">
                        <h2 align=center> Prepare a C# WinForm Project<br>(create a new Project, or open an existing Project)</h2>
<h3>Reference “cosmos.dll”, adjust manifest and compilation configurations</h3>


<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/183294437-cf6a3f96-69ed-4274-936c-ba963e21537d.jpg" width="100%"/></div>
                    </td>
                    <td width="25%">
		     <h3 align=center><p>Open "program.cs" file.</p> <p align=center>Replace:</p> <p align=center>"Application.Run"</p> <p align=center>with:</p><p align=center>Universe.WebRT.Run</p></h3>
                    </td>
            </tbody>
        </table>
</p>
</h2>

<div align=center>

# [Converting MFC Application <br>into Chromium Project Browser Process](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)
  
<div align=center>

## (1)Prepare a MFC Project <br>(create a new Project, or open an existing Project)

<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Precompiled Header File</strong>
                    <th> <strong>Precompiled Header File, Manifest Files and DPI</strong>
               </tr>            
	<tbody>
                <tr>
                    <td width="33%">
                        <h3 align=left><p>
			
Copy all files included with [***MFCPlus***](https://github.com/TangramDev/OpenWebRunTime/tree/master/src/sdk/MFCPlus) into the prepared MFC Project. Open files "pch.h(stdafx.h)", "pch.cpp(stdafx.cpp)", add the following code at the end of the opened file at a suitable position:</p>
<h5>
<p>// for pch.h or stdafx.h</p>
<p align=left>#include "WebRTApp.h"</p>
<p>// for pch.cpp or stdafx.cpp</p>
<p align=left>#include "WebRTApp.cpp"</p><h5></h3>
                    </td>
                    <td width="67%">
		     <div align=center id="mfcdevmanifest"><img src="https://user-images.githubusercontent.com/26355688/183366016-6337524d-c195-4d0c-a2d5-8cd74f0baf17.jpg" width="100%"/></div>
                    </td>
            </tbody>
        </table>
</center>


<div align=center>


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
                    <td width="20%">
                        <strong><p align=center>Modify Base Class</strong> </p>
                    </td>
                    <td width="80%">
		     <strong>
		     Replace "public CWinApp(Ex)" with: <p align=center>public CWebRTApp(Ex)</p>
		     Replace "public CMDIFrameWndEx" with: <p align=center>public CWebRTMDIFrame</p>
		     </strong>
                    </td>
            </tbody>
	    <tbody>
                <tr>
                    <td width="20%">
                        <strong><p align=center>Dialog Application</strong> </p>
                    </td>
                    <td width="80%">
		     <strong><p>Modify the return value of</p><p><div align=center>BOOL CMFCDlgApp::InitInstance()</p><p align=left>to</p> <p align=center>TRUE</strong>.</p>
                        </p></strong>
                    </td>
            </tbody>	    
	    <tbody>
                <tr>
                    <td class="sunnysolution" width="20%">
                        <strong><p align=center>Document Serialization</p></strong>
                    </td>
                    <td class="sunnysolution" width="80%">
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
