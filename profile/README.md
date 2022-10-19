<h1 align=center>
The Core Job of Web Runtime:<br><i>Eliminate</i> the <i>Gap</i> between <i>Desktop Software</i> and <i>Web Browser</i>
</h1>
<h2>
<p>The Web Runtime provides developers with a <p align=center>"<i>Simplest Technical Strategy</i>"</p> <ins>to convert an "existing" or "newly created" <i>Desktop Software Project</i> into "<i>Browser Process</i>" of "Chromium Project"</ins>, thus realizing Web pageization of "Desktop Application Functions", it completely bridges the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and make Web Technology an inherent part of <i>Desktop Software Architecture</i>. 
</p>
</h2>

<div align=center>

# [WinFormPlus](https://github.com/TangramDev/WinFormPlus): Converting WinForm Application <br>into Chromium Project Browser Process
<div align=left>

**From the code perspective, for WinForm Applications, developers only need to modify <i><ins>a line of code</ins></i> to convert their application system into a <i><ins>Chromium Browser Process</ins></i> supported by WebRuntime. The rest of the work is basically the <i>Compilation Configuration Adjustment</i> of WinForm Projects and necessary <i>Component References</i>.**</div>	
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
<h3>
<p>

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
<div align=left>

**From the code point of view, for MFC Applications, developers can convert their application system into a <i><ins>Chromium Browser Process</ins></i> supported by WebRuntime by replacing <i>up to <ins>Two Base Classes</ins></i>, the remaining work is basically the <i>Compilation and Configuration Adjustment</i> of the MFC project and <i>a Very Small Amount of Code Modification</i>.**</div>	
  
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
How Will WebRuntime Change <i>Desktop Applications</i>?
</h1>
<h2 align=left>
<p>As shown in the figure below, we see a WinForm Application at <i>Design Time</i>:</p>
 <div align=center id="Form1DesignTime"><img src="https://user-images.githubusercontent.com/26355688/196173217-dfe1d7d1-5ae3-4da4-a455-1462d86ef20b.jpg" width="67%"/></div>
<p>Generally, we will see the following <i>Runtime Results</i>:</p>
<div align=center id="Form1Runtime"><img src="https://user-images.githubusercontent.com/26355688/196174538-97d01137-f58c-4a6e-a878-6246824ec7c7.jpg" width="33%"/></div>
<p>When we convert this project into a project that supports WebRuntime, we will see any number of <i>Completely Different Runtime Scenarios</i>, as shown in the following figure, which is <ins><i>one of them</i></ins>:</p>
<div align=center id="dynForm"><img src="https://user-images.githubusercontent.com/26355688/196175684-e6f36ad4-d7df-4a9e-9f62-b4ce3b78ab6f.jpg" width="67%"/></div>


<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/HowWebRTChangeYourApp.md.md)
</div>


<p>Similar to those Second Order Partial Differential Equations with significant physical significance(they need <i>Specific Boundary Conditions</i> and <i>Initial Value Conditions</i>), every Desktop Application Systems supported by WebRuntime need an <i>Initialization Run Description</i>(which is usually described by a Web page or an Xml document). due to the differences in initialization descriptions, we will see the startup main window with <i>Completely Different Structures</i>. Different initialization conditions correspond to different runtime results, which we call a "<ins><i>Runtime State</i></ins>". WebRuntime enables a <i>Desktop Application</i> to support <i>Three Types of <ins>Runtime States</ins></i>: 

<div align=left>

- [Desktop Application Runtime State with Web Ecology](https://github.com/TangramDev/.github/blob/main/document/DesktopAppRuntimeState.md).
<p><div align=center id="ApplicationwithWebEcology"><img src="https://user-images.githubusercontent.com/26355688/196022828-1af528ef-f135-4236-8d2e-b2fa719d2018.jpg" width="75%" /><br>(Desktop Application with Web Ecology)</div><br/>
<div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896016-13973932-53ef-4749-9ea6-ccb5c95f9fa8.jpg" width="75%" /><br/>( MFC MDI Application with Web Ecology)</div></p>
 
- [Personalized Modern Web Browser Runtime State](https://github.com/TangramDev/.github/blob/main/document/WebBrowserRuntimeState.md).
<p><div align=center id="ApplicationAsBrowser"><img src="https://user-images.githubusercontent.com/26355688/196023584-4ec77d1a-a754-4a64-9161-2bf4fd9c8447.jpg" width="75%" /><br>(Run Desktop Application As a Web Browser with Extended Web DOM Support)</div>
</p>

- [Win32 Desktop Application Runtime State](https://github.com/TangramDev/.github/blob/main/document/Win32AppRuntimeState.md)(no Built-in Browser Support).
<p><div align=center id="Application"><img src="https://user-images.githubusercontent.com/26355688/196025011-4d77d697-698c-44f3-b15b-9565446eac21.jpg" width="75%" /><br>(Win32 Desktop Application Runtime State)</div>
</p>
</div>

<div align=left>
Each type of application state has any number of runtime personalized instances to adapt to different application scenarios.
</div>

</p>
</h2> 

<h1 align=center>
Working with <i>Latest Chromium Project Source Code</i>
</h1>
<h2  align=left>
<p>

[OpenWebRuntime](https://github.com/TangramDev/OpenWebRunTime) can work synchronously with the <i>Latest Version Chromium Project</i>(Canary, Dev, Beta, and Stable Version) Source Code, to do this, you need to refer to the 
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases/download/v109.0.5366.1/webrt_109.0.5366.1.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 109.0.5366.1, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases/download/v108.0.5359.7/webrt_108.0.5359.7.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 108.0.5359.7, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases/download/v107.0.5304.50/webrt_107.0.5304.50.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 107.0.5304.50, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Stable/releases/download/v106.0.5249.158/webrt_106.0.5249.158.7z)</p>		
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 106.0.5249.158, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Stable/releases)
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
