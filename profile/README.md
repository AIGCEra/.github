<h1 align=center>
The Core Job of Web Runtime:<br><i>Eliminate</i> the <i>Gap</i> between <i>Desktop Software</i> and <i>Web Browser</i>
</h1>
<h2>
<p>The Web Runtime provides developers with a <p align=center>"<i>Simplest Technical Strategy</i>"</p> <ins>to convert an "existing" or "newly created" <i>Desktop Software Project</i> into "<i>Browser Process</i>" of "Chromium Project"</ins>, thus realizing Web pageization of "Desktop Application Functions", it completely bridges the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and make Web Technology an inherent part of <i>Desktop Software Architecture</i>. </p>
<p>WebRuntime enables a desktop application to support three types of <i>Runtime States</i>: 
<div align=left>

- Desktop Application State with Web ecology.
<br/><div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896509-92769481-8558-4add-948a-8b0e3e6d2269.jpg" width="45%" /><br>(First Visible Window is a WinForm)</div>
<div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896016-13973932-53ef-4749-9ea6-ccb5c95f9fa8.jpg" width="45%" /><br/>(First Visible Window is a MFC MDI Frame Window)</div>
 
- Personalized Modern Web Browser State.
- Win32 Desktop Application State(no Built-in Browser Support).
</div>
Each type of application state has any number of runtime personalized instances to adapt to different application scenarios.
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

Copy all files included with [***WinFormPlus***](https://github.com/TangramDev/WinFormPlus/archive/refs/heads/main.zip) into the prepared WinForm Project,</p> Reference “cosmos.dll”, adjust manifest and compilation configurations</h3>


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
			
Copy all files included with [***MFCPlus***](https://github.com/TangramDev/MFCPlus/archive/refs/heads/main.zip) into the prepared MFC Project.</p><p> Pay attention to the processing of "WebRTApp.h" and "WebRTApp.cpp" in the picture on the right.</p>
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

<h1 align=center>
Working with <i>Latest Chromium Project Source Code</i>
</h1>
<h2  align=left>
<p>

We designed [OpenWebRuntime](https://github.com/TangramDev/OpenWebRunTime) to work in sync with the latest Chromium Project source code for each version (Canary, Dev, Beta, and Stable Version). To do this, you need to refer to the 
<div align=center>

[**Building Chromium for Windows**](https://chromium.googlesource.com/chromium/src/+/main/docs/windows_build_instructions.md)</div>

to obtain the source code of the latest full version of the Chromium Project, and to ensure that this version can be compiled correctly so that the compiled results can run properly. The IDE Environment we work here is Visual Studio 2022 17.3.5(requires C++/CLI support).</p>
<div align=right>
</h2>

<center>
        <table border="3" cellpadding="3" align=center>
            <thead>
                <tr>
                    <th width="25%"> <strong>Chromium Build</strong>
                    <th width="25%"> <strong>Chromium Src Patch</strong>
                    <th width="25%"> <strong>Binary Package</strong>
                    <th> <strong>Notes</strong>
               </tr>            
	<tbody>
                <tr>
                    <td width="75">
                        <h4 align=center>
				
[Canary](https://github.com/TangramDev/WebRT_Chromium_Canary)
			</h4>
                    </td>
                    <td width="25%">
                        <h3 align=center><p>
			
[**Latest Patch**](https://github.com/TangramDev/WebRT_Chromium_Canary/archive/refs/heads/main.zip)</p>			
		     </h3>
                    </td>
                    <td width="300">
                        <h3 align=center><p>
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases/download/v109.0.5360.0/webrt_109.0.5360.0.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 109.0.5360.0, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases)
                    </td>
                <tr>
                    <td width="75">
                        <h4 align=center>
				
[Dev](https://github.com/TangramDev/WebRT_Chromium_Dev)
			</h4>
                    </td>
                    <td width="25%">
                        <h3 align=center><p>
			
[**Latest Patch**](https://github.com/TangramDev/WebRT_Chromium_Dev/archive/refs/heads/main.zip)</p>			
		     </h3>
                    </td>
                    <td width="300">
                        <h3 align=center><p>
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases/download/v108.0.5359.1/webrt_108.0.5359.1.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 108.0.5359.1, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases)
                    </td>
		<tr>
                    <td width="75">
                        <h4 align=center>
				
[Beta](https://github.com/TangramDev/WebRT_Chromium_Beta)
			</h4>
                    </td>
                    <td width="25%">
                        <h3 align=center><p>
			
[**Latest Patch**](https://github.com/TangramDev/WebRT_Chromium_Beta/archive/refs/heads/main.zip)</p>			
		     </h3>
                    </td>
		    <td width="300">
                        <h3 align=center><p>
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases/download/v107.0.5304.42/webrt_107.0.5304.42.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 107.0.5304.42, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases)
                    </td>
                <tr>
                    <td width="75">
                        <h4 align=center>
				
[Stable](https://github.com/TangramDev/WebRT_Chromium_Stable)
			</h4>
                    </td>
                    <td width="25%">
                        <h3 align=center><p>
			
[**Latest Patch**](https://github.com/TangramDev/WebRT_Chromium_Stable/archive/refs/heads/main.zip)</p>			
		     </h3>
                    </td>
                    <td width="300">
                        <h3 align=center><p>
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Stable/releases/download/v106.0.5249.134/webrt_106.0.5249.134.packed.7z)</p>		
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 106.0.5249.134, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Stable/releases)
                    </td>
		</tbody>	  
        </table>
</center>
<div align=center>

**(Chromium Src Patch and Web Runtime Binary Package)**</div>


<h1 align=center>
Ushering in the Era of the <i>Web-Defining Desktop Window</i>
</h1>
<h2>
<p align=left>Web Runtime allows developers to use Chromium tabs to organize application functions, each tab corresponds to an application page, and each application page can contain standard web page elements as well as various programmable components (such as .NET Control, MFC CView, etc.). For most desktop software developers, WebRuntime will re-establish their basic understanding of Windows desktop development.</p>
<p align=left>The Web Runtime believes the <i>Expressive</i>, <i>Comprehensive</i>, and <i>Powerful</i> Desktop Windows are composed by using the traditional Web DOM to describe various programmable objects (COM, .Net controls, Win32 windows, etc.), rather than created through complex code technology. This is the key reason to the conversion of the Main Process of Desktop Software into a Browser Process. Describing as many objects as possible with the Web DOM is the basic principle of Web Runtime.

<p><div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181908801-0910fdc6-23b6-457e-bf30-76cfc66097d3.gif" width="80%" /><br>(The Era of "Web Page Define Desktop Window")</div>
</p>

<p align=left>Desktop applications are about to usher in the "<i>Web Page Define Desktop Window</i>" era, in this sense, Desktop Web Browser should be the "<i>Smallest Desktop Application</i>". When developers can reinterpret the specific UI presentation of Web pages, the boundaries between browsers and desktop applications completely disappear.</p>
       
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/readmeex.md)
</div>
</h1>
