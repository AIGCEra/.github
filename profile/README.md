<div align=center>

# [Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)

<div align=center>

## The innate Desktop Software Genes enable each Desktop Child Window to have powerful and flexible component organization capabilities, and various window objects can be aggregated around it. In a sense, each Desktop Child Window could become something like "the galactic nuclei of those huge galaxies in the universe". We know that every Milky Way like galaxy is surrounded by hundreds of billions of stars, **WebRuntime** acts like a Hubble telescope, allowing us to see under certain conditions each Window Object surrounded by a huge, Web Description-Driven Object Structure.

</div>

<div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="90%" />

## **(With the help of Webb and Hubble, people can see an extremely enlarged universe. From Hubble deep space to Webb deep space, unimaginable details in the past appear in our sight. Similarly, when we have webruntime in the field of desktop software, a scene worthy of expectation will also appear. With the help of Web Runtime, the desktop is enlarged, and the infinite hierarchy of desktop window can be displayed, If the surrounding space of many child windows enters our horizon, a magnified universe will surface. Indeed, from the perspective of webruntime, a desktop software itself is a universe, and different desktop software can be regarded as different "parallel universes".)**

</div> 
<hr />

<div align=center id="CoreConcept"><img src="https://user-images.githubusercontent.com/26355688/177946608-74c5ab41-95fc-42e8-b3db-6c69459396a6.jpg" width="95%" /></div> 
<hr />

<div align=center id="CoreConcept">
  
# Technical Strategy of Web Runtime

<div align=center>

<div align=left>How to activate the inherent genes of "Desktop Child Window" and make those components (.Net, COM, C++, Java, etc.) that meet industrial standards surround them according to the rules of modern web is the basic problem faced by Web Runtime. To this end, we need to implement the following technical strategies:</div><br>

<div align=center>Allow developers to use their most familiar development languages (such as C#, MFC, etc.)<br>and the most familiar application structure (such as the application structure from the Visual Studio Wizard) <br>to develop the Browsing Process of Chromium Project. This strategy will eliminate <br>the Boundary between Desktop Software and Web Browser, and make Web Technology <br>become a part of Desktop Software  Basic Technical Architecture.
</div><br>

<div align=left>Once developers can develop the browsing process of the Chromium Project according to their own wishes, the boundary of the Web DOM will be broken naturally, and the Peripheral Space of the Window Nucleus will become an extension of the scope of the Web DOM.</div><br>

<div align=center id="PeripheralSpace"><img src="https://user-images.githubusercontent.com/26355688/179315596-9e163a5f-c7c3-4dd6-8817-3b9df85dc017.jpg" width="100%" /></div>  
<hr/>
 
<div align=center id="CoreConcept">
  
# The Goal of Web Runtime is devoted to unify <br>the Development of Desktop and Web Software, <br>it is based on the following core features:

<div align=center>

|_Core Features_|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;_Description_&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|
| ------ | ---------------------------------------------------------------------------------------------------------------- |
|  <div align=center>**Between any Window Nucleus <br>and its Immediate Parent Window there exists a Web/XML DOM controllable “Window Object Layer Space Structure” around it;**</div> |<div align=center></div><div align=center id = "WebGeneChildWnd"><br><img id="WebGeneChildWnd" src="https://user-images.githubusercontent.com/26355688/179388697-a054c09d-90cb-4a78-b7a6-1ac2df6cb856.jpg" width="100%"/><br><img src="https://user-images.githubusercontent.com/26355688/177030478-b4953bb3-b301-4ab4-9203-18a660307732.gif" width="100%"/></div>|
|<div align=center id="BasicLayout"><img src="https://user-images.githubusercontent.com/26355688/179394341-176ee7c1-0a9b-44c1-a435-1aa7123fc2dc.png" width="100%"/></div>| <div align=center>**_The Web Runtime_ enables developers to load a Layout Layer Structure <br>between _the Window Nucleus_ and _its Parent Window_ <br>using Web or XML DOM Technology at any stage of the Software Runtime**</div><div align=center id="tabs1"><img src="https://user-images.githubusercontent.com/26355688/179235961-8a088dd4-27c9-42d9-8179-db5ffaf0d3f4.gif" width="100%" /></div>|
|<div align=center id="BasicLayout"><img src="https://user-images.githubusercontent.com/26355688/179395039-e1be757f-c499-4ba1-9ec8-21dcacccf469.png" width="100%"/></div>|<div align=center>__Thanks to Web Runtime's implementation of _the Dynamic Link Library Version of the <br>Chromium Project_, developers can use their familiar development techniques to <br>develop the Browsing Process of Chromium Project, which means that completely <br>different from standard browsers, the first visible window can be a developer-defined <br>window (such as WinForms or MFC windows, etc.).In a specific Desktop Application, <br>other Processes of the Chromium project(such as rendering process, GPU process, etc.) <br>are completely preserved.__</div><br><div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896509-92769481-8558-4add-948a-8b0e3e6d2269.jpg" width="45%" /><br>(__First Visible Window is a WinForm__)</div><br><br><div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896016-13973932-53ef-4749-9ea6-ccb5c95f9fa8.jpg" width="45%" /><br>(__First Visible Window is a MFC MDI Frame Window__)</div><hr /><img id="BrowsingProcess" src="https://user-images.githubusercontent.com/26355688/179390066-6163f407-8424-4c68-9217-fffe300e062c.gif" width="100%"/></div>|  
| <div align=center>__.NET Framework for Desktop Application__</div> |<div align=center>_Similar to __Microsoft Visual Basic for Application__, __Web Runtime__ supports <br>__.NET Framework for Desktop Application__, which means that both __WinForm__ and __Usercontrol__ <br>are  within the scope of "__Content-Oriented WebDOM__" of the application._</div><div align=center id="ClrForApp"><img src="https://user-images.githubusercontent.com/26355688/179387353-e9ad7cab-20ac-401d-89dd-ae0396e6e20b.jpg" width="100%"/></div><br><div align=center>__Developers can instantiate WinForm object instances in web pages, and use WinForm, <br>Usercontrol and standard DOM elements to synthesize new web pages. Developers can process .NET object events in the page. Web Runtime implements The two-way delegation mechanism makes Web and desktop elements (Win32 elements and WinForm, Usercontrol, etc.) friendly interoperability.__</div>|    
| <div align=center>__Desktop Application System <br>Runtime Instance State__</div> |<div align=center>__Web Runtime allows an executable file to have any number of "Runtime Instance States",<br> which is significantly different from traditional development techniques. Each <br>"Runtime Instance State“ depends on a local folder, and within each such folder contains a <br>configuration file, an initialization Web page and subfolders closely related to the runtime <br>state, data files, and a necessary component of the application system. Different Runtime <br>States have completely different runtime structures, like a Second-Order Partial Differential <br> Equation, we know that every Second-Order Partial Differential Equation with clear physical <br>meaning (such as the famous wave equation), Its initial value conditions and boundary <br>conditions determine the physical meaning of the solution of this equation. The description of <br> each Desktop Application Runtime Instance State may determine the structure of a software <br>universe, and the differences between different states can be interpreted as <br>Different Parallel Universes.__</div>|  
</div>
<hr />


  # Application Development

  
| _Application Type_       | _description_                                                                              |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| <div align=center>**[WinForm Application Development](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)**</div>|<div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896509-92769481-8558-4add-948a-8b0e3e6d2269.jpg" width="75%" /></div>|  
|  <div align=center> __[Modify the MFC Application Project so that it can be compiled into the Browsing Process of Chromium Project](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)__</div> |<div align=center>__How to convert existing or newly created desktop software projects into projects that match the Browser Process of Chromium Project is the first key problem faced by WebRuntime Development.__</div> <div align=center><img src="https://user-images.githubusercontent.com/26355688/178922407-5518d8eb-a7db-4cc1-912f-0f03060fbd32.gif" width="100%"/></div>|
| <div align=center>**[MFC Desktop Application System: Document Template](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)**</div> |<div align=center>_Different from the traditional MFC Architecture, WebRuntime enables every __MFC Multi-Document-Interface__ Application System that supports the Doc/View architecture to support the document architecture based on Web technology, which means that every "Runtime Instance State" of such application will support any number of document templates , each document template will have its own object structure. This design makes the Multi-Document-Interface application truly realize the meaning of "Multi-Document". If the traditional MFC Doc/View Architecture is "__rigid__", then the WebRuntime-based Doc/View architecture It can be said to be "__flexible__"._</div>| 
| <div align=center>**[MFC Desktop Application System: MFC View](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)**</div> |<div align=center>_Allowing MFC Desktop Applications to support any number of CView-derived objects is one of the places to reflect the flexibility of WebRuntime. When MFC View becomes part of the Web DOM, the Doc/View architecture based on traditional technology is dwarfed. In fact, WebRuntime provides developers with greater freedom, allowing developers to incorporate more generalized MFC CWnd derived objects into the scope of the Web DOM. Based on this idea, developers can flexibly use Web technology controls wider objects like "Docking ControlBar" etc......_</div>|
 
 
