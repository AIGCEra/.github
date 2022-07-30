<h1 align=center>

[Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)
</h1>
<h3 align=center><div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="100%" /></div>(In most scenarios, Desktop Software is like a Universe, with many local huge worlds hidden around numerous child windows, and the Web Runtime is a space telescope, revealing the depths of the universe that have been hidden from the developer's sight...)
</h3>

<h1 align=center><strong>Tribute to Classic</strong>           
<h2>
<p>At different stages of Scientific and Technological Development, there will be classics corresponding to the era to embellish the marvellous of that era. The classic is called a "classic" not only because of its own value, but also because it has a profound impact on a specific historical period. How should we pay tribute to the classics? Letting the classics conform to the rhythm of the times to continue may be a way to pay homage to the classics. We are lucky because we have benefited from a large number of classics, those who made classics, those achievements let us see further and inspire us to continue to create...<p>

<p>There is no doubt that the Chromium Project is a "fully deserve" classic in the Internet age, Visual Studio Wizard is also a classic that has influenced generations of developers. When we enter the era of Internet entrance competition between Microsoft and Google based on "Chromium Project", we are not only the audience in the giant competition field, of course, we expect to become a member of the competition field, otherwise the Oligarchic Competition stage will become a little boring. Web Runtime attempts to build a larger <i>Web DOM</i> and bring together more classic works. If we can only carry out according to the specifications formulated by chromium, then we are doomed to be spectators, and we may have to applaud the competition between giants, so it is imperative to change the rules.</p>
<p>The mission of Web Runtime is to allow more desktop software developers to inherit the advantages of the Chromium Project to the greatest extent, and at the same time, it can also best continue the technical accumulation of the developers themselves. Further, considering the basic characteristics of Web technology, we hope to reasonably expand the boundaries of the Web, and then the technical resources from the .NET Framework, COM, C++ and many other infrastructures will be incorporated into the scope of the Web.</p>

</h2> 
</h1> 

<div align=left>

<div align=center id="CoreConcept"> 

# [Eliminate the _Gap_ <br>Between _Desktop Software_ and _Web Browser_](https://github.com/TangramDev/.github/blob/main/document/TechnicalStrategy.md)

<h2 align=left>
<p>The Web Runtime provides developers with a "<i>Simplest Technical Strategy</i>" <ins>to convert "existing" or "newly created" <i>Desktop Software Projects</i> into "<i>Browser Processes</i>" of "Chromium Project"</ins>, it will completely eliminate the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and makes Web Technology an inherent part of <i>Desktop Software Architecture</i>: </p>
<div align=center>
<p > 

[<ins>WinForm</ins>](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)&emsp;&emsp;[<ins>MFC</ins>](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)</p>
</div>
<p>Desktop applications are about to usher in the "Web Page Define Desktop Application" stage, in this sense, Desktop Web Browser should be the "Smallest Desktop Application". When developers can reinterpret the specific UI presentation of Web pages, the boundaries between browsers and desktop applications completely disappear.

<div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181904338-865e7b65-16c9-40a2-9e63-dc49db632acb.gif" width="90%" /><br>(The stage of "Web Page Define Desktop Application")</div>
<p align=center><div align=left>Once the developer's Desktop Application Project is converted into a Chromium Project Browser Process, It will support the four UI subsystems listed in the following table in the sense of the Web DOM (elements of these subsystems are used as new DOM elements in a Web page to compose a composite user interface):</p>
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>UI Subsystem</strong>
                    <th> <strong>Description</strong>
                </tr>
            <tbody>
                <tr>
                    <td width="30%">
                        <p align=center><strong>WebBrowser UI Subsystem.</strong></p>
                    </td>
                    <td width="70%" rowspan=5>
                        <p>The developer's project will inherit the functional system of the complete Chromium Project, and the Web Browser will be completely retained as a subsystem of the new desktop software project. <i><ins>Since the Desktop Software itself also has its own functional system and UI Mechanism, this new Browser Process should be able to support application-oriented Web pages</ins>, as shown in the following figure</i>:</p>
                        <p align=center id="WebRuntime2"><img src="https://user-images.githubusercontent.com/26355688/179390066-6163f407-8424-4c68-9217-fffe300e062c.gif" width="100%"><br>(Application-Oriented Web Pages)</img></p>
                        <p>
                            We hope that the new <i>Browser Process</i> can bring the Web Page Mechanism based on the Host Application Object Model to the Application, if this vision can be realized, then Web pages will become more important to specific desktop applications, and a Web Application Ecological Mechanism will naturally be formed.
                        </p>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="30%">
                        <p align=center><strong>.NET UI Subsystem.</strong></p>
                    </td>
                    <td width="70%" rowspan=5>
                        <p>The whole .Net WinForms Architecture will become a part of the new Web DOM, which means that developers can instantiate WinForm objects in the web pages supported by the new application system, and WinForms and UserControls can participate in writing new web pages,  of course, it is perfectly possible to handle events of .NET objects in a Web page.</p>
                        <p align=center id="WinFormsforApplication"><img src="https://user-images.githubusercontent.com/26355688/180966988-ed42d50d-410b-41cd-acaa-ccf007c8d1e7.png" width="80%"><br>(.NET WinForms for Application fully comparable to <i>Visual Basic for Application</i>)</img></p>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="30%">
                        <p align=center><strong>COM UI Subsystem.</strong></p>
                    </td>
                    <td width="70%" rowspan=5>
                        <p>
                            COM/ActiveX objects are used as elements of the new Web DOM, so that these two types of objects can participate in the production of application-oriented web pages, and the web pages can process the events of COM objects.
                        </p>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="30%">
                        <p align=center><strong>MFC UI Subsystem.</strong></p>
                    </td>
                    <td width="70%" rowspan=5>
                        <p>
                            The MFC CWnd/CView class is used as an element of the new Web DOM, so that these two types of objects can participate in the production of application-oriented web pages. The web page can process the Win32 messages of the CWnd object.
                        </p>
                    </td>
                </tr>
            </tbody>
        </table>
    </center>
 
<p>When a Process supports the above four UI subsystems, it means that a new "four-dimensional space" is supported at runtime, and the four dimensions here are used as the "base" of the UI space (similar to the vector space of linear algebra), Web pages are used to describe the "combination of base elements", and we can generate any number of Desktop Windows based on this. The following figure shows a Dynamic Desktop Window formed by BrowserUI, .NET UI and MFC UI:</p>
<div align=center id="mfcUI"><img src="https://user-images.githubusercontent.com/26355688/181903819-ae6a054b-67a0-4b3c-ab0b-33910d897930.jpg" width="75%" /></div>


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

<div align=center id="FormNucleus"><img src="https://user-images.githubusercontent.com/26355688/181654297-f2bafff1-5fe6-45a3-a1f5-5360f92f083c.gif" width="80%"/></div>
</h2>

<h1  align=center>

Extending the Scope of the Web <br>to _the Periphery of Various Window Nuclei_
</h1>
<h2>
  
<p align=left>

In the Standard Web browser, the scope of the Web is completely limited inside the WebView, while <strong><ins>the Web Runtime further extends the scope of the Web to <i>the Periphery</i> of <i>Various Window nuclei</i></ins></strong>. <p>
  
<div align=center id="ActivateGene"><img src="https://user-images.githubusercontent.com/26355688/180607456-856f9d69-389d-4c2b-bd98-c315d10b553e.jpg" width="80%" /></div>
  
<div align=center>(Web Runtime makes the peripheral space of the <i>Window Nucleus</i> <br>show its original face. For a long time, because we ignored the existence of peripheral space, a gap between <i>Web</i> and <i>Desktop</i> Software Technology was formed...)<br><div align=left><br>For each "Layout" in the "Window Layout Layer Space Structure", any type of child window(such as MFC Windows, WinForms, .Net Usercontrols, ActiveX Controls, ..., etc.) can be used to fill each specific position in the layout. The Web Gene of Window Nucleus enables most Desktop Windows to have Web Description Driven Capabilities comparable to WebView.</div>
</h2>

<h1 align=center>
Using Web Technology <br>to Drive Window Nucleus and its Peripheral Space
</h1>

<h2 align=left>

When the developer's "_Application Project_" is converted into "_the Browser Process_" of the Chromium Project, how to control the _Peripheral Space_ of the Window Nucleus based on Web technology is a brand-new Web topic, and a Desktop Software-Related "Web Application Ecological Chain" has revealed the tip of the iceberg...

<p>

In fact, the _Periphery_ of Window Nucleus is _an Infinite Hierarchy Object Structure_ driven by  _Web Descriptions_, we see that the Standard Web Technology _builds the Web Content inside the WebView_, and the Web Gene of the Window Nucleus enables Web Runtime further _extends the Web content to the Periphery of the Window Nuclei_ that widely exist in Desktop Applications. <br><div align=center id="periphery7"><img src="https://user-images.githubusercontent.com/26355688/180611630-810edca9-c1a4-4100-8df9-046f8e4fc24e.jpg" width="100%"/></div>
</p>
<p>

<div align=left>In a sense, every <i>Window Nucleus</i> has the <i>Potential</i> to become something like "<i>the Galactic Nuclei of those Huge Galaxies in the Universe</i>". We know that every Milky Way like Galaxy is surrounded by hundreds of billions of stars, Web Runtime acts like a Hubble Telescope, allowing us to see under certain conditions each Window Nucleus surrounded by a Huge, Web Description-Driven Object Structure.<br><br><div align=center id="periphery5"><img src="https://user-images.githubusercontent.com/26355688/180599198-2c6f7227-fdc3-43e1-ba9d-db97af06a98e.jpg" width="75%"/></div><div align=center>(When we suddenly find that more and more Desktop Windows can be described by Web Technology, the Desktop Software World in our minds may have to be re-understood ...)</div><br><div align=left>With the help of Webb and Hubble, people can see an extremely enlarged universe. From Hubble Deep Space to Webb Deep Space, unimaginable details of the Universe in the past appear in our sight. Similarly, when we have <i>Web Runtime</i> in the field of Desktop Software, a scene worthy of expectation will also appear. With the help of Web Runtime, the Desktop Software is enlarged, and <i>the infinite hierarchy of Desktop Window</i> can be displayed, If the surrounding space of many Window Nuclei enters our horizon, a magnified universe will surface. Indeed, from the perspective of <i>Web Runtime</i>, a desktop software itself is a <i>Universe</i>, and Different Desktop Software can be regarded as Different "<i>Parallel Universes</i>".</div></p>

<p><div align=right>

[More Information About Web Gene of Window Nucleus ...](https://github.com/TangramDev/.github/blob/main/document/WebGene.md)</div></p></h2>  

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
                    <td rowspan=5>
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
