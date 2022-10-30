<h1 align=center>

The Core Mission of [Web Runtime](https://github.com/TangramDev/OpenWebRunTime):<br><i>Eliminate</i> the <i>Gap</i> between <i>Desktop Software</i> and <i>Web Browser</i>
</h1>
<h2>
<p>When we observe the universe with naked eyes, our intuition will tell us that the earth is the center of the universe, and everything will revolve around the earth. The limited naked-eye horizon of human beings allowed our ancestors to form a geocentric theory to describe the system of the universe. Our view of the universe today is unmatched by the early geocentric theory. The advent of Hubble and Webb has allowed us to see the narrowness of the geocentric theory, these survey telescopes allow us to clearly see that the universe is full of extragalactic galaxies, each galactic nucleus is surrounded by hundreds of billions of stars, allowing us to see a scene that the naked eye cannot reach.

Every Desktop Window Object is surrounded by an infinite-dimensional, web-driven world of window objects, which looks very similar to the Galactic Nuclei of Giant Galaxies in the Universe. Perhaps we've overlooked something important, we've been ignorant of the huge world of content that surrounds window objects since desktop software came out., so the desktop windows we can see are probably just the tip of the iceberg of the real window object world(Similar to the universe under the naked eye). WebRuntime's responsibility is to reveal the true face of these surrounding worlds for developers, prompting us to rethink the world of desktop software. The Web-driven surround world around the Desktop Window Object is the innate gene of the Desktop Window Object, we call it the "Web nature" of the Window object.
</p>
If the Runtime Position of a  Child Window only depends on the
<p>
<div align=center>

[WM_WINDOWPOSCHING](https://docs.microsoft.com/en-us/windows/win32/winmsg/wm-windowposchanging)
</div>
</p>
<p>
<p>

Message of its Parent Window, then this Child Window is called a [Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md) of its Parent Window, any <ins><i>Parent Window</ins></i> of Window Nucleus is called a <ins><i>Nucleated Window</i></ins>.
</p>
<p>Window Nucleus is a widely existing desktop window object. The key factor that determines whether a window object is a window nucleus is a geometric constraint, which makes every window object possible to become a window nucleus.</p>
<p>

The <i>Core Idea</i> of [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) is: every <i>Desktop Window Object</i> has both "<i>Native Nature</i>" and "<i>Web Nature</i>", which is very similar to the "<i>Wave-particle duality</i>" in the field of Physics, which we call the "<i>Web-native duality</i>" of <i>Desktop Window Object</i>.
</p>
<p>

The [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) provides developers with a <p align=center>"<i>[Simplest Technical Strategy](https://github.com/TangramDev/.github/blob/main/document/ConvertWinFormandMFCProjecttoBrowserProcess.md)</i>"</p> <ins>to convert an "existing" or "newly created" <i>Desktop Software Project</i> into "<i>Browser Process</i>" of "Chromium Project"</ins>, and then activate the "Web Nature" of the Window Nucleus, thus realizing Web pageization of "Desktop Application Functions", it completely bridges the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and make Web Technology an inherent part of <i>Desktop Software Architecture</i>. 
</p>
</h2>

<h1 align=center>

[How Will Web Runtime Change <i>Desktop Applications</i>](https://github.com/TangramDev/.github/blob/main/document/HowWebRTChangeYourApp.md)?
</h1>
<h2 align=left>
<p>As shown in the figure below, we see a WinForm Application at <i>Design Time</i>:</p>
	
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th align=center> <strong>WinForm Application at <i>Design Time</strong>
                    <th align=center> <strong>WinForm Application at <i>Run Time</strong>
               </tr>            
	<tbody>
                <tr>
                    <td width="50%">
                     <div align=center id="Form1DesignTime"><img src="https://user-images.githubusercontent.com/26355688/196173217-dfe1d7d1-5ae3-4da4-a455-1462d86ef20b.jpg" width="100%"/></div>   
                    </td>
                    <td width="50%">
		      <div align=center id="Form1Runtime"><img src="https://user-images.githubusercontent.com/26355688/196174538-97d01137-f58c-4a6e-a878-6246824ec7c7.jpg" width="80%"/></div>
                    </td>
            </tbody>	  
        </table>
</center>	
	
<p>
	
When we convert this project into a project that supports [Web Runtime](https://github.com/TangramDev/OpenWebRunTime), we will see <i>any number</i> of <i>Completely Different Runtime Scenarios</i>, as shown in the following figure, which is <ins><i>one of them</i></ins>:</p>

<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th align=center> <strong>WinForm Application at <i>Design Time</strong>
                    <th align=center> <strong>WinForm Application at <i>Run Time</strong>
               </tr>            
	<tbody>
                <tr>
                    <td width="50%">
                     <div align=center id="Form1DesignTime"><img src="https://user-images.githubusercontent.com/26355688/196173217-dfe1d7d1-5ae3-4da4-a455-1462d86ef20b.jpg" width="100%"/></div>   
                    </td>
                    <td width="50%">
		      <div align=center id="dynForm1Runtime"><img src="https://user-images.githubusercontent.com/26355688/197387216-c4e163bb-0385-4973-86ba-df9073522e5a.jpg" width="80%"/></div>
                    </td>
            </tbody>	  
        </table>
</center>

<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th align=center> <strong>Form1 at <i>Run Time</i>(No WebRT Support)</strong>
                    <th align=center> <strong>Form1 at <i>Run time</i>(with WebRT Support)</strong>
               </tr>            
	<tbody>
                <tr>
                    <td width="50%">
                     <div align=center id="Form1DesignTime"><img src="https://user-images.githubusercontent.com/26355688/196174538-97d01137-f58c-4a6e-a878-6246824ec7c7.jpg" width="80%"/></div>   
                    </td>
                    <td width="50%">
		      <div align=center id="dynForm1Runtime"><img src="https://user-images.githubusercontent.com/26355688/197387216-c4e163bb-0385-4973-86ba-df9073522e5a.jpg" width="80%"/></div>
                    </td>
            </tbody>	  
        </table>
</center>

<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/HowWebRTChangeYourApp.md)
</div>

</h1>

<h1 align=center>
Ushering in the Era of the <i>Web-Defining Desktop Window</i>
</h1>
<h2 align=left>
<p>
	
[Web Runtime](https://github.com/TangramDev/OpenWebRunTime) allows developers to use <I>Chromium Tab Pages</I> to organize application contents, each tab page corresponds to an <i>application page</i> and each <i>application page</i> can contain standard web page elements as well as various programmable components (such as .NET Control, MFC CView, etc.). For most Desktop/Web Software Developers, WebRuntime will re-establish their Basic Understanding of <i>Windows Desktop Development</i>.</p>

<div align=center id="TabsPage"><img src="https://user-images.githubusercontent.com/26355688/196898272-858b5d56-6cc9-425a-acb3-bce1f0ee5182.jpg" width="100%" /><br>(Use Chromium Tabs to Organize Application Contents)</div>
	
<p align=left>
	
The [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) believes the <i>Expressive</i>, <i>Comprehensive</i>, and <i>Powerful</i> Desktop Windows are composed by using the traditional Web DOM to describe various programmable objects (COM, .Net controls, Win32 windows, etc.), rather than created through complex code technology. This is the key reason to the conversion of the Main Process of Desktop Software into a Browser Process. Describing as many objects as possible with the Web DOM is the basic principle of Web Runtime.

<p><div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181908801-0910fdc6-23b6-457e-bf30-76cfc66097d3.gif" width="100%" /><br>(The Era of "Web Page Define Desktop Window")</div>
</p>

<p align=left>Desktop applications are about to usher in the "<i>Web Page Define Desktop Window</i>" era, in this sense, Desktop Web Browser should be the "<i>Smallest Desktop Application</i>". When developers can reinterpret the specific UI presentation of Web pages, the boundaries between <i>Browsers</i> and <i>Desktop Applications</i> completely disappear.</p>
       
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/readmeex.md)
</div>

<h1 align=center>

[Working with <i>Latest Chromium Project <br/>Source Code</i> and <i>Binary Package</i>](https://github.com/TangramDev/.github/blob/main/document/WorkingwithChromiumSourceCode.md)
</h1>
<h2  align=left>
<p>

[OpenWebRuntime](https://github.com/TangramDev/OpenWebRunTime) can work synchronously with the <i>Latest Version Chromium Project Source Code</i>([Canary](https://github.com/TangramDev/WebRT_Chromium_Canary), [Dev](https://github.com/TangramDev/WebRT_Chromium_Dev), [Beta](https://github.com/TangramDev/WebRT_Chromium_Beta), and [Stable Version](https://github.com/TangramDev/WebRT_Chromium_Stable)), to do this, you need to refer to the 
<div align=center>

[**Building Chromium for Windows**](https://chromium.googlesource.com/chromium/src/+/main/docs/windows_build_instructions.md)</div>

to obtain the source code of the latest full version of the Chromium Project, and to ensure that this version can be compiled correctly so that the compiled results can run properly. The IDE Environment we work here is Visual Studio 2022 17.3.5(requires C++/CLI support).</p>

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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases/download/v109.0.5389.1/webrt_109.0.5390.1.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 109.0.5390.1, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases/download/v108.0.5359.22/webrt_108.0.5359.23.7z)</p>		
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 108.0.5359.23, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases/download/v108.0.5359.24/webrt_108.0.5359.25.7z)</p>
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 108.0.5359.25, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases/tag/v108.0.5359.24)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Stable/releases/download/v107.0.5304.72/webrt_107.0.5304.95.7z)</p>		
		     </h3>
                    </td>
                    <td  align=center>
		        Version: 107.0.5304.95, [**More>>**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases/tag/v108.0.5359.24)
                    </td>
		</tbody>	  
        </table>
</center>
<div align=center>

**(Chromium Src Patch and Web Runtime Binary Package)**</div>

