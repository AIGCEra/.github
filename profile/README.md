<div align=center>

# [Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)
</div>

## <div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="100%" /></div><div align=center>(In most scenarios, Desktop Software is like a _Universe_, with many local huge worlds hidden around numerous child windows, and the Web Runtime is a space telescope, revealing the depths of the universe that have been hidden from the developer's sight...)</div>
<div align=left>

<div align=center id="CoreConcept"> 

# [Eliminate the _Gap_ <br>Between _Desktop Software_ and _Web Browser_](https://github.com/TangramDev/.github/blob/main/document/TechnicalStrategy.md)
<div align=left>

## The Web Runtime provides developers with a "_Simplest Technical Strategy_" to convert "existing" or "newly created" _Desktop Software Projects_ into "_Browser Processes_" of "Chromium Project", it will completely eliminate the gap between _the Desktop Software_ and _Web Browser_ and makes Web Technology an inherent part of _Desktop Software Architecture_: <br><br><div align=center><div align=center>__[WinForm](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)__&emsp;&emsp;__[MFC](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)__<br><br><div align=left>When the Desktop Software Project created by the developer with Visual Studio Wizard can fully assume the role of the Browser Process of Chromium Project, then the developer first gets all the Web browsing functions that a Modern Web Browser should have, and it already has a complete Browser Window UI system, you can use it to browse the Web. Since the Desktop Software itself also has its own functional system and UI Mechanism, this new Browser Process should be able to support application-oriented Web pages, as shown in the following figure:<br><br><div align=center id="WebRuntime2"><img src="https://user-images.githubusercontent.com/26355688/180951488-6044fa9f-e816-4526-acd1-a28cb3aa71dd.jpg" width="80%"><br>(Application-Oriented Web Pages)</img></div><br>We hope that the new Browser Process can bring the Web Page Mechanism based on the Host Application Object Model to the Application, if this vision can be realized, then Web pages will become more important to specific desktop applications, and a Web Application Ecological Mechanism will naturally be formed.<br><br>In fact, we can do more, for example, once the developer's Desktop Application fully assumes the role of Browser Process, then the whole .Net WinForms architecture will become a part of the new Web DOM, which means that developers can instantiate WinForm objects in the web pages supported by the new application system, and WinForms and UserControls can participate in writing new web pages,  of course, it is perfectly possible to handle events of .NET objects in a Web page.<br><br><div align=center id="WinFormsforApplication"><img src="https://user-images.githubusercontent.com/26355688/180966988-ed42d50d-410b-41cd-acaa-ccf007c8d1e7.png" width="80%"><br>(.NET WinForms for Application fully comparable to VBA)</img></div><br><div align=right>[More Information ...](https://github.com/TangramDev/.github/blob/main/document/TechnicalStrategy.md)</div></div>
<hr />

<div align=center>

# The Core Object <br>of Web Runtime: ***[Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md)***
</div>

## If the _Runtime Position_ of a ***Child Window*** only depends on the <div align=center><br>[WM_WINDOWPOSCHING](https://docs.microsoft.com/en-us/windows/win32/winmsg/wm-windowposchanging)</div><br>Message of its Parent Window, then this Child Window is called a [Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md) of its Parent Window.<br><br>***Every Window Nucleus has an Innate Web Gene***: <br><br><div align=center>__Between any Window Nucleus <br>and its Immediate Parent Window <br>there exists a Web/XML DOM controllable <br>“Window Layout Layer Space Structure” around it.__</div><br><div align=center id="periphery6"><img src="https://user-images.githubusercontent.com/26355688/180633438-d7025ce1-ba3f-438f-8bbe-7509b430de93.jpg" width="80%"/></div>
<hr />

<div align=center>

# Extending the Scope of the Web <br>to _the Periphery of Various Window Nuclei_
</div>

## <div align=left>In the Standard Web browser, the scope of the Web is completely limited inside the WebView, while the Web Runtime further extends the scope of the Web to _the Periphery_ of _Various Window nuclei_. <br><br><div align=center id="ActivateGene"><img src="https://user-images.githubusercontent.com/26355688/180607456-856f9d69-389d-4c2b-bd98-c315d10b553e.jpg" width="80%" /></div><div align=center>(Web Runtime makes the peripheral space of the _Window Nucleus_ <br>show its original face. For a long time, because we ignored the existence of peripheral space, a gap between _Web_ and _Desktop_ Software Technology was formed...)<br><div align=left><br>For each "Layout" in the "Window Layout Layer Space Structure", any type of child window(such as MFC Windows, WinForms, .Net Usercontrols, ActiveX Controls, ..., etc.) can be used to fill each specific position in the layout. The Web Gene of Window Nucleus enables most Desktop Windows to have Web Description Driven Capabilities comparable to WebView.</div>

<hr />
<div align=center>

# Using Web Technology <br>to Drive Window Nucleus and its Peripheral Space
</div>

## <div align=left>When the developer's "_Application Project_" is converted into "_the Browser Process_" of the Chromium Project, how to control the _Peripheral Space_ of the Window Nucleus based on Web technology is a brand-new Web topic, and a Desktop Software-Related "Web Application Ecological Chain" has revealed the tip of the iceberg...</div><br><div align=right>[More Information About Web Gene of Window Nucleus ...](https://github.com/TangramDev/.github/blob/main/document/WebGene.md)</div></div>  

<hr />

<div align=center id="CoreConcept">
  
# [The Core Features of Web Runtime](https://github.com/TangramDev/.github/blob/main/document/CoreFeatures.md)
</div>

|_Web Runtime Core Features_|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;_Description_&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|
| ------ | ---------------------------------------------------------------------------------------------------------------- |
|  <div align=center>**Between any Window Nucleus <br>and its Immediate Parent Window there exists a Web/XML DOM controllable “Window Object Layer Space Structure” around it;**</div> |<div align=center></div><div align=center id = "ChildWndGene2"><br><img id="WebGeneChildWnd" src="https://user-images.githubusercontent.com/26355688/179456149-1a007bee-ed02-4c52-bf8a-ddc55c715b21.jpg" width="100%"/></div>|
|<div align=center id="BasicLayout"><img src="https://user-images.githubusercontent.com/26355688/179394341-176ee7c1-0a9b-44c1-a435-1aa7123fc2dc.png" width="100%"/></div>| <div align=center>**_The Web Runtime_ enables developers to load a Layout Layer Structure <br>between _the Window Nucleus_ and _its Parent Window_ <br>using Web or XML DOM Technology at any stage of the Software Runtime**</div><div align=center id="tabs1"><img src="https://user-images.githubusercontent.com/26355688/179235961-8a088dd4-27c9-42d9-8179-db5ffaf0d3f4.gif" width="100%" /></div>|  
</div>
<div align=right>

## [more core features...](https://github.com/TangramDev/.github/blob/main/document/CoreFeatures.md)</div>

<div align=center id="CoreConcept">

# Every Desktop Software is an Vibrant Universe
<div align=left id="universe">

## The Web Runtime supports a large enough DOM model. In addition to the standard Web DOM elements, .NET, COM, MFC, etc. that we are currently familiar with are all embodied in this DOM in a suitable way. Developers can instantiate WinForm objects  in Web pages, handle events of .NET objects, and more. Each window object that contains a window nucleus must contain any number of window nuclei, which makes a nucleated window look very similar to the galaxy group in the universe. The well-known browser window, WinForm, etc. are regarded as the common resource of all desktop software. If the window nucleus is equivalent to the galaxy nucleus, then the desktop software itself is a descriptive universe based on Web technology.

</div>
</div>

