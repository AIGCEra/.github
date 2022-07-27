<h1 align=center>

[Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)
</h1>
<h3 align=center><div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="100%" /></div>(In most scenarios, Desktop Software is like a _Universe_, with many local huge worlds hidden around numerous child windows, and the Web Runtime is a space telescope, revealing the depths of the universe that have been hidden from the developer's sight...)
</h3>

<h1 align=center><strong>Tribute to Classic</strong>           
<h2>
<p>At different stages of Scientific and Technological Development, there will be classics corresponding to the era to embellish the splendor of that era. The classic is called a "classic" not only because of its own value, but also because it has a profound impact on a specific historical period. How should we pay tribute to the classics? Letting the classics conform to the rhythm of the times to continue may be a way to pay homage to the classics. We are lucky because we have benefited from a large number of classics, those who made classics, those achievements let us see further and inspire us to continue to create...<p>

<p>There is no doubt that the Chromium Project is a "fully deserve" classic in the Internet age, Visual Studio Wizard is also a classic that has influenced generations of developers. When we enter the era of Internet entrance competition between Microsoft and Google based on "Chromium Project", we are not only the audience in the giant competition field, of course, we expect to become a member of the competition field, otherwise the Oligarchic Competition stage will become a little boring. Web Runtime attempts to build a larger <i>Web DOM</i> and bring together more classic works. If we can only carry out according to the specifications formulated by chromium, then we are doomed to be spectators, and we may have to applaud the competition between giants, so it is imperative to change the rules.</p>
<p>The mission of Web Runtime is to allow more desktop software developers to inherit the advantages of the Chromium Project to the greatest extent, and at the same time, it can also best continue the technical accumulation of the developers themselves. Further, considering the basic characteristics of Web technology, we hope that the scope of the Web can be reasonably expanded, and then the technical resources from the .NET Framework, COM, C++ and many other infrastructures will be incorporated into the scope of the Web.</p>

</h2> 
</h1> 

<div align=left>

<div align=center id="CoreConcept"> 

# [Eliminate the _Gap_ <br>Between _Desktop Software_ and _Web Browser_](https://github.com/TangramDev/.github/blob/main/document/TechnicalStrategy.md)

<h2 align=left>
<p>The Web Runtime provides developers with a "<i>Simplest Technical Strategy</i>" to convert "existing" or "newly created" <i>Desktop Software Projects</i> into "<i>Browser Processes</i>" of "Chromium Project", it will completely eliminate the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and makes Web Technology an inherent part of <i>Desktop Software Architecture</i>: </p>
<div align=center>
<p > 

[WinForm](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)&emsp;&emsp;[MFC](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)</p>
</div>
<p><i>When the Desktop Software Project created by the developer with Visual Studio Wizard can fully assume the role of the Browser Process of Chromium Project, then the Desktop Application first gets all the Web browsing functions that a Modern Web Browser should have, and it already has a complete Browser Window UI system, you can use it to browse the Web. Since the Desktop Software itself also has its own functional system and UI Mechanism, this new Browser Process should be able to support application-oriented Web pages, as shown in the following figure</i>:</p>
<p align=center id="WebRuntime2"><img src="https://user-images.githubusercontent.com/26355688/180951488-6044fa9f-e816-4526-acd1-a28cb3aa71dd.jpg" width="80%"><br>(Application-Oriented Web Pages)</img></p>

<p>

We hope that the new _Browser Process_ can bring the Web Page Mechanism based on the Host Application Object Model to the Application, if this vision can be realized, then Web pages will become more important to specific desktop applications, and a Web Application Ecological Mechanism will naturally be formed.</p>

<p>In fact, we can do more, for example, once the developer's Desktop Application fully assumes the role of Browser Process, then the whole .Net WinForms architecture will become a part of the new Web DOM, which means that developers can instantiate WinForm objects in the web pages supported by the new application system, and WinForms and UserControls can participate in writing new web pages,  of course, it is perfectly possible to handle events of .NET objects in a Web page.</p>

<p align=center id="WinFormsforApplication"><img src="https://user-images.githubusercontent.com/26355688/180966988-ed42d50d-410b-41cd-acaa-ccf007c8d1e7.png" width="80%"><br>(.NET WinForms for Application fully comparable to _Visual Basic for Application_)</img></p>

<p>Desktop Application has ushered in the stage of "Web Page is Application", in this sense, Desktop Web Browser should be the smallest Desktop Application. When developers can reinterpret the specific UI presentation of Web pages, the boundaries between browsers and desktop applications completely disappear.
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/TechnicalStrategy.md)
</div></p>
</h2>

<h1  align=center>

The Core Object <br>of Web Runtime: [Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md)
</h1>
<div align=left>
<h2>
If the Runtime Position of a  Child Window only depends on the
<p>
<div align=center>

[WM_WINDOWPOSCHING](https://docs.microsoft.com/en-us/windows/win32/winmsg/wm-windowposchanging)
</div>
</p>
<p>

Message of its Parent Window, then this Child Window is called a [Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md) of its Parent Window.
</p>
<p>

Every Window Nucleus has an Innate Web Gene: <br><div align=center>__Between any Window Nucleus <br>and its Immediate Parent Window <br>there exists a Web/XML DOM controllable <br>“Window Layout Layer Space Structure” around it.__</div><br><div align=center id="periphery6"><img src="https://user-images.githubusercontent.com/26355688/180633438-d7025ce1-ba3f-438f-8bbe-7509b430de93.jpg" width="80%"/></div>
</p>
</h2>
<hr />

<h1  align=center>

Extending the Scope of the Web <br>to _the Periphery of Various Window Nuclei_
</h1>
<h2>
  
<p align=left>

In the Standard Web browser, the scope of the Web is completely limited inside the WebView, while the Web Runtime further extends the scope of the Web to _the Periphery_ of _Various Window nuclei_. <p>
  
<div align=center id="ActivateGene"><img src="https://user-images.githubusercontent.com/26355688/180607456-856f9d69-389d-4c2b-bd98-c315d10b553e.jpg" width="80%" /></div>
  
<div align=center>(Web Runtime makes the peripheral space of the _Window Nucleus_ <br>show its original face. For a long time, because we ignored the existence of peripheral space, a gap between _Web_ and _Desktop_ Software Technology was formed...)<br><div align=left><br>For each "Layout" in the "Window Layout Layer Space Structure", any type of child window(such as MFC Windows, WinForms, .Net Usercontrols, ActiveX Controls, ..., etc.) can be used to fill each specific position in the layout. The Web Gene of Window Nucleus enables most Desktop Windows to have Web Description Driven Capabilities comparable to WebView.</div>
</h2>
<hr />

<h1 align=center>
Using Web Technology <br>to Drive Window Nucleus and its Peripheral Space
</h1>

<h2 align=left>

When the developer's "_Application Project_" is converted into "_the Browser Process_" of the Chromium Project, how to control the _Peripheral Space_ of the Window Nucleus based on Web technology is a brand-new Web topic, and a Desktop Software-Related "Web Application Ecological Chain" has revealed the tip of the iceberg...<p><div align=right>

[More Information About Web Gene of Window Nucleus ...](https://github.com/TangramDev/.github/blob/main/document/WebGene.md)</div></p></h2>  

<hr />

<h1 align=center id="CoreConcept">
  
[The Core Features of Web Runtime](https://github.com/TangramDev/.github/blob/main/document/CoreFeatures.md)
</h1>
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr style="font-size: 16px; font-weight:bold; color:midnightblue">
                    <th> Web Runtime Core Features
                    <th> <i>Description</i>
                </tr>
            <tbody>
                <tr>
                    <td class="sunnysolution" width="30%">
                        <h3 align=center>Between any Window Nucleus and its Immediate Parent Window there exists a Web/XML DOM controllable “Window Object Layer Space Structure” around it.</h3>
                    </td>
                    <td class="sunnysolution" width="70%" rowspan=5>
                        <p style="font-size: 16px; font-weight:bold; color:blueviolet">
                            <div align=center></div><div align=center id="ChildWndGene2"><br><img id="WebGeneChildWnd" src="https://user-images.githubusercontent.com/26355688/179456149-1a007bee-ed02-4c52-bf8a-ddc55c715b21.jpg" width="100%" /></div>
                        </p>
                    </td>
            </tbody>
            <tbody>
                <tr>
                    <td class="sunnysolution" width="30%">
                        <div align=center id="BasicLayout"><img src="https://user-images.githubusercontent.com/26355688/179394341-176ee7c1-0a9b-44c1-a435-1aa7123fc2dc.png" width="100%" /></div>
                    </td>
                    <td class="sunnysolution" width="70%" rowspan=5>
                        <p style="font-size: 16px; font-weight:bold; color:blueviolet">
                            <h3 align=center>The Web Runtime_ enables developers to load a Layout Layer Structure between the Window Nucleus and its Parent Window using Web or XML DOM Technology at any stage of the Software Runtime</div><div align=center id="tabs1"><img src="https://user-images.githubusercontent.com/26355688/179235961-8a088dd4-27c9-42d9-8179-db5ffaf0d3f4.gif" width="100%" /></h3>
                        </p>
                    </td>
            </tbody>
        </table>
    </center>

<div align=right>

## [more core features...](https://github.com/TangramDev/.github/blob/main/document/CoreFeatures.md)</div>

<h1 align=center id="CoreConcept">

Every Desktop Software is an Vibrant Universe

<h2>
<p><div align=left id="universe">

The Web Runtime supports a large enough DOM model. In addition to the standard Web DOM elements, .NET, COM, MFC, etc. that we are currently familiar with are all embodied in this DOM in a suitable way. Developers can instantiate WinForm objects  in Web pages, handle events of .NET objects, and more. Each window object that contains a window nucleus must contain any number of window nuclei, which makes a nucleated window look very similar to the galaxy group in the universe. The well-known browser window, WinForm, etc. are regarded as the common resource of all desktop software. If the window nucleus is equivalent to the galaxy nucleus, then the desktop software itself is a descriptive universe based on Web technology.
<div>
</p>
</h2>
</h1>
