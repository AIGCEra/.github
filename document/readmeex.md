  <h1 align=center>

The Basic Concepts for [Web Runtime](https://github.com/TangramDev/OpenWebRunTime)
</h1>
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Basic Concepts</strong>
                    <th> <strong>Description</strong>
                </tr>
             <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Window Nucleus</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>
If the Runtime Position of a  Child Window only depends on the
<p>
<div align=center>

[WM_WINDOWPOSCHING](https://docs.microsoft.com/en-us/windows/win32/winmsg/wm-windowposchanging)
</div>
</p>
<p>
<h3>

Message of its Parent Window, then this Child Window is called a [Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md) of its Parent Window, any <ins><i>Parent Window</ins></i> of Window Nucleus is called a <ins><i>Nucleated Window</i></ins>.
</p>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Browser Process</strong></j3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>The Main Process of the Chromium Project is called the Chromium Project Browser Process, 
                        which provides the UI system for Web Browsers.
                        </h3>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Common Component Space</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>We call the set of all <ins><i>Dynamic Link Libraries</i></ins> that can provide <ins>Component Services</ins> (object services or UI services, such as providing Controls, Windows. Forms, etc.) for other <i>Desktop Applications</i> as the "Common Component" Space.<h3>             
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Private Component Space of Desktop Software</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>The components from the main process and those components from all the dynamic link library which directly depend on the main process form a set,  which is called the "private component space of desktop software".<h3>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Component Space of Desktop Software</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>The union set of "<ins>Common Component Space</ins>" and "<ins>Private Component Space of Desktop software</ins>" is called "<ins>Component Space of Desktop software</ins>".<h3>
                    </td>
                </tr>
            </tbody>
        </table>
    </center>      


<h1  align=center>

The Core Object <br>of [Web Runtime](https://github.com/TangramDev/OpenWebRunTime): [Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md)
</h1>
<div align=left>
<h2>

<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Window Nucleus</strong>
                    <th> <strong>Description</strong>
                </tr>
            <tbody>
                <tr>
                    <td width="25%">
                        <p align=center><strong>Web Gene of Window Nucleus</strong></p>
                    </td>
                    <td width="75%" rowspan=5>
                        <h4 align=left>
                                <p>Every Window Nucleus has an Innate Web Gene:</p><p align=center>Between any Window Nucleus and its Immediate Parent Window there exists a Web/XML DOM controllable “Window Layout Layer Space” around it.</p>
                                <p align=center id="LayoutSpace"><img src="https://user-images.githubusercontent.com/26355688/182048931-17a7d63e-8c4d-4194-b032-9da79a74c29d.jpg" width="100%"/></p>
                        </h4>
                    </td>
                </tr>
            </tbody>            
            <tbody>
                <tr>
                    <td width="25%">
                        <p align=center><strong>Local Web Description Space of Window Nucleus</strong></p>
                    </td>
                    <td width="75%" rowspan=5>
                        <h4 align=left>
                        <p>For each "Layout" in the "Window Layout Layer Space", any type of child window comes from the "<ins><i>Component Space of Desktop Software</i></ins>"(such as <i>MFC Windows</i>, <i>WinForms</i>, <i>.Net Usercontrols</i>, <i>ActiveX Controls</i>, ..., etc.) can be used to fill each specific position in the layout.</p> <p><ins>The set of all possible filling results for all possible layout structures are filled by child windows in the "component space of Desktop Application" is called the "local Web Description Space" around a given window nucleus</ins>.</p> <p align=center id="periphery6"><img src="https://user-images.githubusercontent.com/26355688/180633438-d7025ce1-ba3f-438f-8bbe-7509b430de93.jpg" width="100%"/></p>
                        <p>The Web Gene of Window Nucleus enables most Desktop Windows to have Web Description Driven Capabilities comparable to WebView.
                        </p>
                        </h4>
                     </td>
                </tr>
            </tbody>            
            <tbody>
                <tr>
                    <td width="25%">
                        <p align=center><strong>Various types of Window Nuclei</strong></p>
                    </td>
                    <td width="75%" rowspan=5>
                        <h4 align=left><div align=center id="FormNucleus"><img src="https://user-images.githubusercontent.com/26355688/181654297-f2bafff1-5fe6-45a3-a1f5-5360f92f083c.gif" width="100%"/></div></h4>                                      </td>
                </tr>
            </tbody>
         </table>
    </center>
<p>
</h2>
        

<h1  align=center>

Extending the Scope of the Web to <br>_the Periphery of Various Window Nuclei_: the Local Web Description Space of Window Nucleus
</h1>   

<h2>
<p align=left>

In the Standard Web browser, the scope of the Web is completely limited inside the WebView, while <strong><ins>the [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) further extends the scope of the Web to <i>the Periphery</i> of <i>Various Window nuclei</i></ins>(the Local Web Description Space of Window Nucleus)</strong>. 
  
<div align=center id="ActivateGene"><img src="https://user-images.githubusercontent.com/26355688/180607456-856f9d69-389d-4c2b-bd98-c315d10b553e.jpg" width="80%" /></div>
  
<div align=center>
  
 ([Web Runtime](https://github.com/TangramDev/OpenWebRunTime) makes the peripheral space of the <i>Window Nucleus</i> <br>show its original face. For a long time, because we ignored the existence of peripheral space, a gap between <i>Web</i> and <i>Desktop</i> Software Technology was formed...)<p>

<div  align=left>
  
The [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) believes the <i>Expressive</i>, <i>Comprehensive</i>, and <i>Powerful</i> Desktop Windows are composed by using the traditional Web DOM to describe various programmable objects (COM, .Net controls, Win32 windows, etc.), rather than created through complex code technology. This is the key reason to the conversion of the Main Process of Desktop Software into a Browser Process. Describing as many objects as possible with the Web DOM is the basic principle of [Web Runtime](https://github.com/TangramDev/OpenWebRunTime).
</div> 

<p><div align=center id="dynwnd1"><img src="https://user-images.githubusercontent.com/26355688/181908801-0910fdc6-23b6-457e-bf30-76cfc66097d3.gif" width="80%" /><br>(The stage of "Web Page Define Desktop Application")</div>
</p>

<p align=left>Desktop applications are about to usher in the "<i>Web Page Define Desktop Application</i>" stage, in this sense, Desktop Web Browser should be the "<i>Smallest Desktop Application</i>". When developers can reinterpret the specific UI presentation of Web pages, the boundaries between browsers and desktop applications completely disappear.</p>

<p align=center><div align=left>Once the developer's Desktop Application Project is converted into a Chromium Project Browser Process, It will support <i><ins>four UI subsystems</ins></i> come from the "<ins><i>Component Space of Desktop Software</i></ins>" listed in the following table in the sense of the Web DOM (elements of these subsystems are used as new DOM elements in a Web page to compose a composite user interface):</p>
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
</div>
</p>
</h2>

<h1 align=center>
Using Web Technology <br>to Drive Window Nucleus and its Local Web Description Space
</h1>

<h2 align=left>

When the developer's "_Application Project_" is converted into "_the Browser Process_" of the Chromium Project, how to control the _Peripheral Space_ of the Window Nucleus(the Local Web Description Space of Window Nucleus) based on Web technology is a brand-new Web topic, and a Desktop Software-Related "Web Application Ecological Chain" has revealed the tip of the iceberg...

<p>

In fact, the _Periphery_ of Window Nucleus is _an Infinite Hierarchy Object Structure_ driven by  _Web Descriptions_, we see that the Standard Web Technology _builds the Web Content inside the WebView_, and the Web Gene of the Window Nucleus enables [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) further _extends the Web content to the Periphery of the Window Nuclei_ that widely exist in Desktop Applications. <br><div align=center id="periphery7"><img src="https://user-images.githubusercontent.com/26355688/180611630-810edca9-c1a4-4100-8df9-046f8e4fc24e.jpg" width="100%"/></div>
</p>
<p>

<div align=left>
  
In a sense, every <i>Window Nucleus</i> has the <i>Potential</i> to become something like "<i>the Galactic Nuclei of those Huge Galaxies in the Universe</i>". We know that every Milky Way like Galaxy is surrounded by hundreds of billions of stars, [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) acts like a Hubble Telescope, allowing us to see under certain conditions each Window Nucleus surrounded by a Huge, Web Description-Driven Object Structure.<br><br><div align=center id="periphery5"><img src="https://user-images.githubusercontent.com/26355688/180599198-2c6f7227-fdc3-43e1-ba9d-db97af06a98e.jpg" width="75%"/></div><div align=center>(When we suddenly find that more and more Desktop Windows can be described by Web Technology, the Desktop Software World in our minds may have to be re-understood ...)</div><br><div align=left>With the help of Webb and Hubble, people can see an extremely enlarged universe. From Hubble Deep Space to Webb Deep Space, unimaginable details of the Universe in the past appear in our sight. Similarly, when we have <i>[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)</i> in the field of Desktop Software, a scene worthy of expectation will also appear. With the help of Web Runtime, the Desktop Software is enlarged, and <i>the infinite hierarchy of Desktop Window</i> can be displayed, If the surrounding space of many Window Nuclei enters our horizon, a magnified universe will surface. Indeed, from the perspective of <i>[Web Runtime](https://github.com/TangramDev/OpenWebRunTime)</i>, a desktop software itself is a <i>Universe</i>, and Different Desktop Software can be regarded as Different "<i>Parallel Universes</i>".</div></p>

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

The [Web Runtime](https://github.com/TangramDev/OpenWebRunTime) supports a large enough DOM model. In addition to the standard Web DOM elements, .NET, COM, MFC, etc. that we are currently familiar with are all embodied in this DOM in a suitable way. Developers can instantiate WinForm objects  in Web pages, handle events of .NET objects, and more. Each window object that contains a window nucleus must contain any number of window nuclei, which makes a nucleated window look very similar to the galaxy group in the universe. The well-known browser window, WinForm, etc. are regarded as the common resource of all desktop software. If the window nucleus is equivalent to the galaxy nucleus, then the desktop software itself is a descriptive universe based on Web technology.
<div>
</p>
</h2>
</h1>
