<h1 align=center>
The Core Job of Web Runtime:<br><i>Eliminate</i> the <i>Gap</i> between <i>Desktop Software</i> and <i>Web Browser</i>
</h1>
<h2>
<p>The Web Runtime provides developers with a <p align=center>"<i>Simplest Technical Strategy</i>"</p> <ins>to convert an "existing" or "newly created" <i>Desktop Software Project</i> into "<i>Browser Process</i>" of "Chromium Project"</ins>, thus realizing Web pageization of "Desktop Application Functions", it completely bridges the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and make Web Technology an inherent part of <i>Desktop Software Architecture</i>.
</p>
</h1> 

<div align=center>

# [WinFormPlus](https://github.com/TangramDev/WinFormPlus): Converting WinForm Application <br>into Chromium Project Browser Process
	
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
<h3><p>

Copy all files included with [***WinFormPlus***](https://github.com/TangramDev/WinFormPlus/archive/refs/tags/v1.0.0.1.zip) into the prepared WinForm Project,</p> Reference “cosmos.dll”, adjust manifest and compilation configurations</h3>


<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/183294437-cf6a3f96-69ed-4274-936c-ba963e21537d.jpg" width="100%"/></div>
                    </td>
                    <td width="25%">
		     <h3 align=center><p>Open "program.cs" file.</p> <p align=center>Replace </p> <p align=center>"Application.Run"</p> <p align=center>with </p><p align=center>Universe.WebRT.Run</p></h3>
                    </td>
            </tbody>
        </table>
</p>
</h2>

<div align=center>

# [MFCPlus](https://github.com/TangramDev/MFCPlus): Converting MFC Application <br>into Chromium Project Browser Process
  
<div align=center>

## Prepare a MFC Project <br>(create a new Project, or open an existing Project)

<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Code Modifications</strong>
                    <th> <strong>Adjust Precompiled Header File, Manifest Files and DPI</strong>
               </tr>            
	<tbody>
                <tr>
                    <td width="33%">
                        <h4 align=left><p>
			
Copy all files included with [***MFCPlus***](https://github.com/TangramDev/MFCPlus/archive/refs/tags/v1.0.0.0.zip) into the prepared MFC Project.</p><p> Pay attention to the processing of "WebRTApp.h" and "WebRTApp.cpp" in the picture on the right.</p>
			<hr/>
			<strong><p align=center><ins>Modify Base Class</ins></p>
		     Replace "public CWinApp(Ex)" with: <p align=center>public CWebRTApp(Ex)</p>
		     Replace "public CMDIFrameWndEx" with: <p align=center>public CWebRTMDIFrame</p>
		     </strong>
		     <hr />
		     <p align=center><ins>For Dialog Application</ins></p>
		     <strong><p>Modify the return value of</p><p><div align=center>BOOL CMFCDlgApp::InitInstance()</p><p align=left>to</p> <p align=center>TRUE</strong>.</p>
                        </p></strong>
		     <hr />
		     <p align=center><ins>[About Document Serialization](https://github.com/TangramDev/.github/blob/main/document/DocSerialization.md)</ins></p>
		     </h4>
                    </td>
                    <td width="67%">
		     <div align=center id="mfcdevmanifest"><img src="https://user-images.githubusercontent.com/26355688/183423613-a9258a4c-a0bc-4553-88b6-4b347ea56ab2.jpg" width="100%"/></div>
                    </td>
            </tbody>	  
        </table>
</center>
	
# Web Runtime Binary Package

<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Milestone Version</strong>
                    <th> <strong>Chromium Version</strong>
                    <th> <strong>Notes</strong>
               </tr>            
	<tbody>
                <tr>
                    <td width="25%">
                        <h4 align=center>
				
[M108](https://github.com/TangramDev/WebRT_M108/releases/tag/m108)
			</h4>
                    </td>
                    <td width="30%">
                        <h3 align=center><p>
			
[**108.0.5322.1**](https://github.com/TangramDev/WebRT_M108/releases/download/m108/webrt_108.0.5322.1.7z)</p>			
		     </h3>
                    </td>
                    <td width="45%">
		        2022-09-26 02:08 Build, size: 90.50 MB
                    </td>
                <tr>
                    <td width="25%">
                        <h4 align=center>
				
[M107](https://github.com/TangramDev/WebRT_M107/releases/tag/M107)
			</h4>
                    </td>
                    <td width="30%">
                        <h3 align=center><p>
			
[**107.0.5304.13**](https://github.com/TangramDev/WebRT_M107/releases/download/M107/webrt_107.0.5304.13.7z)</p>			
		     </h3>
                    </td>
                    <td width="45%">
		        2022-09-25 09:41 Build, size: 89.8 MB
                    </td>
                <tr>
                    <td width="25%">
                        <h4 align=center>
				
[M106](https://github.com/TangramDev/WebRT_M106/releases/tag/M106)
			</h4>
                    </td>
                    <td width="30%">
                        <h3 align=center><p>
			
[**106.0.5249.67**](https://github.com/TangramDev/WebRT_M106/releases/download/M106/webrt_106.0.5249.67.7z)</p>			
		     </h3>
                    </td>
                    <td width="45%">
		        2022-09-25 09:06 Build, size: 88.8 MB
                    </td>
		</tbody>	  
        </table>
</center>
<h2 align=center>
	
<div align=right>

[More Download ...](https://github.com/TangramDev/.github/blob/main/document/WebRTDownkoad.md)
</div>
</h2>

<h1 align=center>
Ushering in the Era of the <i>Web-Defining Desktop Window</i>
</h1>
<h2>
<p align=left>Web Runtime allows developers to use Chromium tabs to organize application functions, each tab corresponds to an application page, and each application page can contain standard web page elements as well as various programmable components (such as .NET Control, MFC CView, etc.). For most desktop software developers, WebRuntime will re-establish their basic understanding of Windows desktop development.</p>
<p align=left>The Web Runtime believes the <i>Expressive</i>, <i>Comprehensive</i>, and <i>Powerful</i> Desktop Windows are composed by using the traditional Web DOM to describe various programmable objects (COM, .Net controls, Win32 windows, etc.), rather than created through complex code technology. This is the key reason to the conversion of the Main Process of Desktop Software into a Browser Process. Describing as many objects as possible with the Web DOM is the basic principle of Web Runtime.
</p> 

<p><div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181908801-0910fdc6-23b6-457e-bf30-76cfc66097d3.gif" width="80%" /><br>(The Era of "Web Page Define Desktop Window")</div>
</p>

<p align=left>Desktop applications are about to usher in the "<i>Web Page Define Desktop Window</i>" era, in this sense, Desktop Web Browser should be the "<i>Smallest Desktop Application</i>". When developers can reinterpret the specific UI presentation of Web pages, the boundaries between browsers and desktop applications completely disappear.</p>
       
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/readmeex.md)
</div>
</h1>
