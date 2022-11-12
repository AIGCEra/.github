
<div align=center>

# [WinFormPlus](https://github.com/TangramDev/WinFormPlus)：将WinForm应用程序<br/>转换为<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>浏览进程
<div align=left>

**从代码的角度来看，对于WinForm应用程序，开发人员只需要修改一行代码即可将其应用程序系统转换为WebRuntime支持的<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>浏览进程。其余的工作基本上是WinForm项目的<ins>编译配置、manifest配置调整</ins>和<ins>必要的组件引用</ins>**。
</div>	
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

# [MFCPlus](https://github.com/TangramDev/MFCPlus)： 将MFC应用程序<br/>转换为<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>浏览进程
<div align=left>

**从代码的角度来看，对于 MFC 应用程序，开发人员可以通过替换最多两个基类将其应用程序系统转换为WebRuntime支持的<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>浏览进程，剩下的工作基本上是 MFC 项目的<ins>编译配置、manifest配置调整</ins>以及<ins>非常少量的代码修改</ins>。**</div>	
  
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
