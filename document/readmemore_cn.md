
<h1 align=center><strong>向经典致敬</strong>           
<h2>
<p>在科技发展的不同阶段，都会有与时代相对应的经典来点缀那个时代的精彩。经典之所以被称为“经典”，不仅是因为它本身的价值，还因为它对特定历史时期有着深远的影响。我们应该如何致敬经典？让他们顺应时代节奏延续，或许是致敬经典的一种方式。我们很幸运，因为我们受益于大量的经典，那些创造经典的人，那些<ins>经典成就</ins>让我们看得更远，激励我们继续创造......</p>

<p>
  
毫无疑问，<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>是互联网时代“当之无愧”的经典之作，Visual Studio Wizard也是影响了一代又一代开发者的经典之作。当我们进入微软和谷歌基于“<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>”的互联网入口竞争时代时，我们不仅仅是巨人竞争领域的观众，当然，我们希望成为竞争领域的一员，否则寡头竞争的舞台会变得有些单调、索然无味。[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)试图构建一个更大的Web DOM，并将更多经典作品汇集在一起。如果我们只能遵守<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>制定的规范，那么我们注定是旁观者，与此同时可能还要为巨头之间的竞争鼓掌、喝彩，所以改变规则势在必行。</p>

<p>
  
[<i>Web Runtime</i>](https://github.com/TangramDev/OpenWebRunTime)的使命是让更多的桌面软件开发者最大限度地继承<i>[Chromium Project](https://chromium.googlesource.com/chromium/src.git)</i>的优势，同时，也能最好地延续开发者自身的技术积累。此外，考虑到Web技术的基本特征，我们希望合理地扩展Web的边界，进而将来自.NET Framework，COM，C++和许多其他基础架构的技术资源纳入Web的范围。...</p>
	
<h1 align=center>
一切从<i>窗口核</i> 开始
</h1>
<h2>
如果一个桌面子窗口的<i><ins>运行时屏幕位置</ins></i> 仅依赖于其父窗口的
<p>
<div align=center>

[WM_WINDOWPOSCHING](https://docs.microsoft.com/en-us/windows/win32/winmsg/wm-windowposchanging)
</div>
</p>
<p>
<p>

消息处理, 那么该子窗口称为其父窗口的一个“窗口核”（[Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md)）, 窗口核的任何一个父窗口称为“有核窗口”（<ins><i>Nucleated Window</i></ins>）。
</p>

<h2>
<p>当我们用裸眼观察宇宙时，我们的直觉会告诉我们，地球是宇宙的中心，一切都会围绕地球旋转。人类有限的裸眼视野使我们的祖先形成了地心说来描述宇宙。我们今天对宇宙的认知是早期的地心说无法比拟的。哈勃和韦伯的出现，让我们看到了地心说的巨大局限、狭隘，这些巡天望远镜让我们清楚地看到宇宙中充满了河外星系，每个星系核都可能被数千亿颗恒星包围，让我们看到裸眼无法看到的场景。</p>

<div align=center id="WndNucleus2"><img src="https://user-images.githubusercontent.com/26355688/198916669-c7c4059f-d096-4020-ae9e-c1d38c86efeb.jpg" width="100%"/></div>

<p>  
每一个“窗口核”（<i><ins>Window Nucleus</ins></i>）的周围都环绕着一个Web驱动、无限维的窗口对象世界, 这个场景使得窗口核可以媲美宇宙之中巨大星系的星系核, 由于桌面软件领域缺乏类似哈勃、Webb这类的“天文望远镜”，这个<i><ins>局部无限维环绕世界</i></ins>一直隐藏在开发者的视线之外，如同地心说时代人类所看到的宇宙一样，我们的祖先在地心说阶段只能看到有限个数的星体，完全不知道河外星系的存在。</p>
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th align=center> <strong>Form1 at <i>Run Time</i></strong>
                    <th align=center> <strong>Content World Arounded Form1</strong>
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
	<p>
		
也许我们忽略了一些重要的东西，自从桌面软件问世以来，我们一直不知道围绕每个窗口核的巨大内容世界的存在，所以我们可以看到的桌面窗口只是真实窗口世界的冰山一角（类似于裸眼视界下的宇宙）。[<i><ins>Web Runtime</ins></i>](https://github.com/TangramDev/OpenWebRunTime) 的使命是为开发人员揭示这些周围世界的真实面貌，促使我们重新思考桌面软件的世界。</p>

<div align=center id="Form1DesignTime"><img src="https://user-images.githubusercontent.com/26355688/199191407-76986b82-5195-4bf6-8c70-fff5f86f8d27.jpg" width="67%"/></div>
<p>环绕在桌面窗口对象周围的、<i><ins>Web驱动的窗口对象世界</ins></i>是桌面窗口对象与生俱来的基因，我们称之为窗口对象的“Web本质属性”。</p>

<div align=center id="Form1DesignTime"><img src="https://user-images.githubusercontent.com/26355688/199193074-1849c4a9-c958-4a1f-8db8-1ba6880eb61a.jpg" width="67%"/></div>
</h2>

<h1 align=center>
窗口核（Window Nucleus）：桌面软件的全新突破点
</h1>
<h2>
<p>窗口核（Window Nuclei）是一类广泛存在的桌面窗口对象。决定窗口对象是否为窗口核的关键因素是一个“几何约束条件”，这个约束条件使每个窗口对象都可能成为窗口核，顾名思义，“窗口核”意味着必须有东西围绕它。</p>

<div align=center id="WndNucleus"><img src="https://user-images.githubusercontent.com/26355688/198913804-8c7e198b-71de-4e33-a4d7-60ae0eec4ac2.jpg" width="80%"/></div> 

<p>
	
每个窗口对象都有可能成为某个窗口的“窗口核”，窗口核心外围世界的发现使我们能够看到桌面软件系统的新层次结构。从天文学的角度来看，人眼视野内只有大约6000颗恒星，与我们看到的真实宇宙尺度相比，这是微不足道的。类似于我们的可观测宇宙包含无数的星系核，每个桌面软件都包含无数个窗口核，由于某种原因，这些窗口核都处于不可见的状态，如果这种说法是正确的，那么我们需要像哈勃和韦伯这样的设备，这样我们才能清楚地理解和看到这些窗口核及其周围的环绕世界。[<i><ins>Web Runtime</ins></i>](https://github.com/TangramDev/OpenWebRunTime)实际上相当于类似哈勃这样的巡天望远镜。当我们用宇宙的视角来看待桌面软件时，[<i><ins>Web Runtime</ins></i>](https://github.com/TangramDev/OpenWebRunTime)让我们看到了一个宇宙尺度的对象结构和一个全新的 Web 世界。......
</p>
</h2>

<h1 align=center>
Web-Native Duality
</h1>
<h2>
<p>
	
[<i><ins>Web Runtime</ins></i>](https://github.com/TangramDev/OpenWebRunTime)的核心思想是：每个桌面窗口对象同时具有“原生本质性质（<i>Native Nature</i>）”和“Web本质性质（<i>Web Nature</i>）”，这与物理领域的“波粒二象性”非常相似，我们称之为桌面窗口对象的“Web-原生二象性”（Web-Native Duality）。
</p>
<p>

[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)为开发人员提供了<p align=center>"<i>[最简单的技术策略](https://github.com/TangramDev/.github/blob/main/document/WinFormandMFCApp2BrowserProcess.md)</i>"</p>将“现有的”或“新创建的”桌面软件项目转换为“[Chromium Project](https://chromium.googlesource.com/chromium/src.git)”的“浏览器进程”，进而激活窗口核的“Web本质性质”，实现“桌面应用功能”的网页化，完全弥合了<i>桌面软件</i>与<i>Web浏览器</i>之间的鸿沟，使Web技术成为<i>桌面软件架构固有的一部分</i>。</p>

</h2>

<h1 align=center>

[Web 运行时将如何改变<i>桌面应用程序</i>？](https://github.com/TangramDev/.github/blob/main/document/HowWebRTChangeYourApp.md)
</h1>
<h2 align=left>
<p>如下图所示，我们看到一个处于设计时的WinForm应用程序：</p>
	
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

当我们把这个项目转换成一个支持[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)的项目时，我们会看到任意数量的完全不同的运行时场景，如下图所示，就是其中之一：
</p>

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
	迎接Web定义<i>桌面窗口</i> 的时代
</h1>
<h2 align=left>
<p>
	
[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)允许开发人员使用Chromium标签页来组织应用程序内容，每个标签页对应于一个应用程序页面，每个应用程序页面可以包含标准网页元素以及各种可编程组件（如 .NET 控件、MFC CView 等）。对于大多数桌面/Web软件开发人员，[<i>Web Runtime</i>](https://github.com/TangramDev/OpenWebRunTime)将重新建立他们对<i>Windows桌面开发</i>的基本理解。
</p>

<div align=center id="TabsPage"><img src="https://user-images.githubusercontent.com/26355688/196898272-858b5d56-6cc9-425a-acb3-bce1f0ee5182.jpg" width="100%" /><br>(Use Chromium Tabs to Organize Application Contents)</div>

<p>
	
[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)认为，富有表现力、功能全面、强大的桌面窗口是通过使用Web DOM来描述各种可编程对象（COM、.Net 控件、Win32 窗口等）而合成的，而不是通过复杂的代码技术创建的，这是将桌面软件的主进程转换为浏览器进程的关键原因。使用Web DOM描述尽可能多的对象是[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)的基本原则。
</p>	

<p><div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181908801-0910fdc6-23b6-457e-bf30-76cfc66097d3.gif" width="100%" /><br>(The Era of "Web Page Define Desktop Window")</div>
</p>
<p>
	桌面应用即将迎来“<i>Web网页定义桌面窗口</i>”时代，从这个意义上说，桌面Web浏览器应该是“<i>最小的桌面应用</i>”。当开发人员可以重新基于Web技术解释Web网页的特定UI表现层时，<ins>Web浏览器</ins>和<ins>桌面应用程序</ins>之间的界限将完全消失。
</p>
       
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/readmeex.md)
</div>
<h1 align=center>

[使用最新版本的<i>Chromium Project源代码<br/></i> 以及Web Runtime<i>二进制编译包</i>](https://github.com/TangramDev/.github/blob/main/document/WorkingwithChromiumSourceCode_cn.md)
</h1>
<h2  align=left>
<p>
	
[OpenWebRuntime](https://github.com/TangramDev/OpenWebRunTime)可以与最新版本[Chromium Project](https://chromium.googlesource.com/chromium/src.git)源代码（[Canary](https://github.com/TangramDev/WebRT_Chromium_Canary), [Dev](https://github.com/TangramDev/WebRT_Chromium_Dev), [Beta](https://github.com/TangramDev/WebRT_Chromium_Beta), and [Stable Version](https://github.com/TangramDev/WebRT_Chromium_Stable)）同步工作，要做到这一点，你需要参考

<div align=center>

[**构建 Chromium for Windows**](https://chromium.googlesource.com/chromium/src/+/main/docs/windows_build_instructions.md)</div>

获取 Chromium 项目最新完整版的源代码，并确保此版本能够正确编译，以便编译后的结果能够正常运行。我们在这里工作的 IDE 环境是 Visual Studio 2022 17.3.5（或更高版本）。
</p>
</h2>

<verinfo>
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases/download/v110.0.5435.0/webrt_110.0.5441.1.7z)</p>			
		     </h3>
                    </td>
                    <td  align=center>
		        Version: [**110.0.5445.1**](https://github.com/TangramDev/WebRT_Chromium_Canary/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases/download/v109.0.5414.12/webrt_109.0.5414.9.7z)</p>		
		     </h3>
                    </td>
                    <td  align=center>
		        Version: [**109.0.5414.19**](https://github.com/TangramDev/WebRT_Chromium_Dev/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Beta/releases/download/v108.0.5359.54/webrt_108.0.5359.66.7z)</p>
		     </h3>
                    </td>
                    <td  align=center>
		        Version: [**108.0.5359.x**(x>=24)](https://github.com/TangramDev/WebRT_Chromium_Beta/releases)
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
			
[**Latest Binary Package**](https://github.com/TangramDev/WebRT_Chromium_Stable/releases/download/v108.0.5359.67/webrt_108.0.5359.68.7z)</p>		
		     </h3>
                    </td>
                    <td  align=center>
		        Version: [**108.0.5359.x**(x>=67)](https://github.com/TangramDev/WebRT_Chromium_Stable/releases)
                    </td>
		</tbody>	  
        </table>
</verinfo>
<div align=center>

**([Chromium Project](https://chromium.googlesource.com/chromium/src.git)源代码补丁和[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)二进制编译包)**</div>

