
<div align=center id="CoreConcept">
  
# The Technical Strategy of Web Runtime will _Eliminate_ <br>the Boundary between _Desktop Software_ and _Web Browser_

<div align=center>

**Thanks to Web Runtime's implementation of _the Dynamic Link Library Version of the Chromium Project_, <br>developers can use their _most familiar development languages_(such as C#, MFC, etc.) and _the most familiar <br>application structure_ (such as the application structure from the _Visual Studio Wizard_) to  develop the "_Browser Process_" <br>of Chromium Project. This strategy will eliminate the Boundary between Desktop Software and Web Browser, <br>and make Web Technology become a part of _Desktop Software Basic Technical Architecture_.**
</div>

<div align=left>

**Developers can develop the _Browser Process_ of the Chromium Project according to their own wishes, which means that completely different from Standard Web Browsers, the First Visible Window can be a Developer-Defined Window (such as WinForms or MFC windows, etc.):**</div>
<div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896509-92769481-8558-4add-948a-8b0e3e6d2269.jpg" width="45%" /><br>
  
  **(First Visible Window is a WinForm)**</div>

<div align=center id="WinFormBrowser"><img src="https://user-images.githubusercontent.com/26355688/176896016-13973932-53ef-4749-9ea6-ccb5c95f9fa8.jpg" width="45%" /></div><br>
  
  **(First Visible Window is a MFC MDI Frame Window)**</div>
<div align=left>
  
  **In a specific Desktop Application, other Processes of the Chromium Project(such as renderer process, GPU process, etc.) are completely preserved. In fact, the difference between _a Desktop Web Browser_ and _a Desktop Application_ is just the difference in the First Web Page, the design principle of the Web Browser is that after the first Web page is opened, a Browser Window is generated. When developers have the ability to develop their own Browser Process, this principle changes when the Browser Process is started. Developers are fully capable of interpreting the First Web Page of the Browser Process as an object they want, in this sense, the Web Browser should be the Smallest Desktop Application System, the Browser Windows(and .NET WinForm Objects) should be a group of objects shared by all Desktop Software. Developers can write Web pages belonging to the application system for their own application systems, and each Web page can open a browser window, of course, can also open a more general window object(such as WinForm). We see that the meaning of a web page changes when the Browser Process can be redefined by the developer...**</div>
  
<div align=center id="AppPage1"><img src="https://user-images.githubusercontent.com/26355688/179521064-8798c09c-5e1a-480d-ad80-a69b931f9684.jpg" width="80%" /><br>
  
  **(Developers can write application-oriented web pages <br>for the host application system according to the object model of desktop applications}**</div>
<div align=center id="AppPage2"><img src="https://user-images.githubusercontent.com/26355688/179521598-c58b6b53-40ba-4e1d-8701-a5005dd13a09.jpg" width="80%" /><br>
  
  **(Application oriented web pages mean that there is <br>a software content ecosystem based on Web technology for desktop applications}**</div>

<div align=left>
  
**When the developer can define the Browser Process by himself, he is fully capable of mixing his Own Defined Window Object Queue with the Browser Window Queue, and then scheduling these window objects with the Web-based driving ability. In the vision of WebRuntime, The independent window objects (such as WinForm, MFC Frame, etc.) are parallel to the Browser Window, and each type of window can support the display of Web pages, which means that the privileged status of the Browser Window will disappear, The dynamic description technique will be fully embodied in the more general window object.**
</div>

<div align=center id="CoreConcept">

# The Technical Strategy of Web Runtime allows us <br>to build a Larger Web DOM <br>around the Peripheral Space of Window Nucleus

**Every window nucleus can be comparable to the galactic nucleus of a huge galaxy, <br>and the world around it has an infinite level of hierarchy. Let's take WinForms as <br>examples to take a look at the dynamic world around the window nucleus, which <br>is a web driven world that developers have never touched. Once we regard the window <br>nucleus as a galactic nucleus, then every desktop software structure will show a <br>cosmic structure similar to that observed today......**

<div align=center id="ChildWndGene2"><img src="https://user-images.githubusercontent.com/26355688/179511606-32ec35a9-9835-4698-a243-e87476a5e165.jpg" width="80%"/><br>

**(Around the green window nucleus, we see a surrounding structure}**
</div> 
<div align=center id="ChildWndGene2"><img src="https://user-images.githubusercontent.com/26355688/179515631-59d4bacd-2ef0-4a2c-a36f-abf118e13f8c.jpg" width="80%"/><br>

**(Around the green window nucleus, we see another surrounding structure}**
</div>
<div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179698094-40585138-11c7-46bb-863b-afec911129ea.gif" width="80%" /></div>

