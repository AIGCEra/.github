<h1 align=center>

[Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)
</h1>
<h3 align=center><div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="100%" /></div>(In most scenarios, Desktop Software is like a Universe, with many local huge worlds hidden around numerous child windows, and the Web Runtime is a space telescope, revealing the depths of the universe that have been hidden from the developer's sight...)
</h3>

<h1 align=center><strong>Tribute to Classic</strong>           
<h2>
<p>At different stages of Scientific and Technological Development, there will be classics corresponding to the era to embellish the marvellous of that era. The classic is called a "classic" not only because of its own value, but also because it has a profound impact on a specific historical period. How should we pay tribute to the classics? Letting them conform to the rhythm of the times to continue may be a way to pay homage to the classics. We are lucky because we have benefited from a large number of classics, those who made classics, those achievements let us see further and inspire us to continue to create...<p>

<p>There is no doubt that the Chromium Project is a "fully deserve" classic in the Internet age, Visual Studio Wizard is also a classic that has influenced generations of developers. When we enter the era of Internet entrance competition between Microsoft and Google based on "Chromium Project", we are not only the audience in the giant competition field, of course, we expect to become a member of the competition field, otherwise the Oligarchic Competition stage will become a little boring. Web Runtime attempts to build a larger <i>Web DOM</i> and bring together more classic works. If we can only carry out according to the specifications formulated by chromium, then we are doomed to be spectators, and we may have to applaud the competition between giants, so it is imperative to change the rules.</p>
<p>The Mission of Web Runtime is to allow more desktop software developers to inherit the advantages of the Chromium Project to the greatest extent, and at the same time, it can also best continue the technical accumulation of the developers themselves. Further, considering the basic characteristics of Web technology, we hope to reasonably expand the boundaries of the Web, and then the technical resources from the .NET Framework, COM, C++ and many other infrastructures will be incorporated into the scope of the Web DOM.</p>
</h2> 

<h1 align=center>
The Core Job of Web Runtime:<br><i>Eliminate</i> the <i>Gap</i> between <i>Desktop Software</i> and <i>Web Browser</i>
</h1>
<h2>
<p>The Web Runtime provides developers with a "<i>Simplest Technical Strategy</i>" <ins>to convert an "existing" or "newly created" <i>Desktop Software Project</i> into "<i>Browser Process</i>" of "Chromium Project"</ins>, thus realizing Web pageization of "Desktop Application Functions", it will completely eliminate the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and make Web Technology an inherent part of <i>Desktop Software Architecture</i>: 
</p>
<div align=center>
<p > 

[<ins>WinForm Project</ins>](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)&emsp;&emsp;[<ins>MFC Project</ins>](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)</p>
</div>

<p  align=left>The Web Runtime believes the <i>Expressive</i>, <i>Comprehensive</i>, and <i>Powerful</i> Desktop Windows are composed by using the traditional Web DOM to describe various programmable objects (COM, .Net controls, Win32 windows, etc.), rather than created through complex code technology. This is the key reason to the conversion of the Main Process of Desktop Software into a Browser Process. Describing as many objects as possible with the Web DOM is the basic principle of Web Runtime.
</p> 

<p><div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181908801-0910fdc6-23b6-457e-bf30-76cfc66097d3.gif" width="80%" /><br>(The stage of "Web Page Define Desktop Window")</div>
</p>

<p align=left>Desktop applications are about to usher in the "<i>Web Page Define Desktop Window</i>" stage, in this sense, Desktop Web Browser should be the "<i>Smallest Desktop Application</i>". When developers can reinterpret the specific UI presentation of Web pages, the boundaries between browsers and desktop applications completely disappear.</p>
       
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/readmeex.md)
</div>
</h1> 

<div align=center>

# [Converting WinForm Application <br>into Chromium Project Browser Process](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)
  
</div>

<div>
  
<h2>Prepare a C# WinForm Project(create a new Project, or open an existing Project), All WinForm projects need the following three steps to support Web Runtime.
  
</div>
<div align=center>

## (1)Reference “cosmos.dll”, adjust manifest configuration
</div>
<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/181695908-5c796645-f37c-44f7-bcba-6270cf20b748.jpg" width="80%"/></div>
<hr />
<div align=center>

## (2)Adjust compilation configuration
</div>
<div align=center id ="WinFormDev_compilecfg"><img src="https://user-images.githubusercontent.com/26355688/181693960-f4857d56-3cb4-427f-896e-1574c391f409.jpg" width="80%"/></div>
<hr />
<div align=center>
  
## (3)Open "program.cs" file.
</div>

## _Modify main function_, Replace:<br><br><div align=center>Application.Run</div><br><div align=left>with</div><br><div align=center>Universe.WebRT.Run</div>
</h2>

<div align=center>

# [Converting MFC Application <br>into Chromium Project Browser Process](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)
  
<div align=center>

## (1)Prepare a MFC Project <br>(create a new Project, or open an existing Project)
<div align=center>

<h3 align=left>
<p>
  
Copy all files included with [***MFCPlus***](https://github.com/TangramDev/OpenWebRunTime/tree/master/src/sdk/MFCPlus) into the prepared MFC Desktop Software Project.</p>
<p>
<div align=center id="mfcdevmanifest"><img src="https://user-images.githubusercontent.com/26355688/181698116-74b3824c-4e1b-457e-92c4-587d4c0b914b.jpg" width="80%"/></div>
</p>	
</h3>
<hr />

<div align=center>

## (2)Modify Precompiled Header Files
</div>
<h3 align=left>
<p>Open the "stdafx.h(stdafx.cpp)" or "pch.h(pch.cpp)" file of the developer's desktop software project, add the following code at the end of the opened file at a suitable position(please refer to our provided examples):</p>
<p align=center>#include "WebRuntimeApp.h" //for stdafx.h or pch.h</p>
<p>and</p>	
<p align=center>#include "WebRuntimeApp.cpp" //for stdafx.cpp or pch.cpp</p>
<p align=center id="PrecompiledHeaderFiles"><img src="https://user-images.githubusercontent.com/26355688/183267877-aa023d27-15d2-4994-bae4-a9c65d3bab90.jpg" width="75%"/></p>	

</h3>

<hr />

## (3)Base Class Replacement
<h2 align=left><p>AppBase: Replace "public CWinApp(Ex)" with "public CWebRTApp(Ex)"</p><p>MDIFrameBase: Replace "public CMDIFrameWndEx" with "public CWebRTMDIFrame"</p></h2>

## (4)Matters Needing Attention
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Needing Attention</strong>
                    <th> <strong>Description</strong>
                </tr>                     
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
		  // TODO: add storing code here
	  }
	  else
	  {
		  ar >> theApp.m_strCreatingDOCID;
		  // TODO: add loading code here
	  }
    }
</p>
</strong>
                    </td>
            </tbody>
        </table>
</center>

