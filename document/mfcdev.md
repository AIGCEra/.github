<div align=center>

# Developing MFC Desktop Application with Web Runtime
  
<div align=center id="MfcApp"><img src="https://user-images.githubusercontent.com/26355688/178436304-730ede1e-23c1-4bc9-b94b-4b082dc3e7ab.jpg" width="75%" height="100%"/></div>
<div align=center>

# MFC Development of WebRuntime Applications need to pay attention to the following aspects：
  
</div>
<div align=left>
<ol>
<li>correctly process the "manifest configuration" of the MFC project</li>
<li>configure the compilation options correctly(WebRuntime only supports 64-bit applications).</li>
<li>AppBase: Replace CWinApp(Ex) with CWebRTApp(Ex)</li>
<li>Tabbed MDI Application: Tabbed MDIFrame Window
<ol>
<li>The Base Class of Tabbed MDIFrame Window: Replace CMDIFrameWndEx with CWebRTMDIFrame</li>
<li>The Message Map of Tabbed MDIFrame Window: Replace CMDIFrameWndEx with CWebRTMDIFrame</li>
</ol>
</li>
<li>FormView: Delete the Call to ResizeParentToFit()</li>
<li>Serialization</li>
<li>Dialog Application: the Function "InitInstance" of App Class should return true</li>
</ol>  
</div>
  
<div align=center>
<hr />  
  
## (1)Preparation: This step is required for all types of MFC Desktop Applications

<div align=center><img src="https://user-images.githubusercontent.com/26355688/178430601-581d57a3-652b-4781-8da5-d1256c4f89b9.gif" width="100%" height="100%"/></div>
<hr />

## (2)AppBase: Replace CWinApp(Ex) with CWebRTApp(Ex), This step is required for all types of MFC Desktop Applications<div align=center id ="MFCAppDev_AppBase"><img src="https://user-images.githubusercontent.com/26355688/178430698-1bd5c36b-3828-41b1-807d-5f441d6902f6.gif" width="100%" height="100%"/></div>
  
### If your app is an MFC Dialog Type Application

<div align=left>
  
**Developer needs to change the return value of the overloaded function "InitInstance" of the App class to true, after replacing the base class of the App class, the C++ code part required by WebRuntime has been completed**
</dv>
<div align=center>

<div align=center><img src="https://media1.giphy.com/media/UGd99qfyY5XjvHhAXZ/giphy.gif?cid=790b76114983d155a4cdbee5f9903e16261bce4fba81c188&rid=giphy.gif&ct=g" width="67%"/></div>
<div align=center>  
  
### If your MFC application is an SDI, MDT or standard MFC MDI style Desktop Application
</div> 
<div align=left>
  
**If there is no CFormView or CFormView derived classes in your MFC application, as long as the replacement of the App class base class is completed, the C++ code part required by WebRuntime has been completed. If it contains CFormView or CFormView derived classes, please refer to the following CFormView section. If the application supports the Doc/View architecture, the document serialization please refers to the following serialization section.**  

</dv>  
<hr />
  
<div align=center>
  
## (3)Tabbed MDI Frame Window: Replace Base Class CMDIFrameWndEx with CWebRTMDIFrame<div align=center id ="MFCAppDev_MDIFrame"><img src="https://user-images.githubusercontent.com/26355688/178430840-f0145e7e-b7f1-418a-82f2-e7a3fe172dcd.gif" width="100%" height="100%"/></div>

## (4)Tabbed MDI Frame Wibndow Message Map: Replace CMDIFrameWndEx with CWebRTMDIFrame<div align=center id ="MFCAppDev_MsgLoop"><img src="https://user-images.githubusercontent.com/26355688/178400063-e23e474d-0127-43fe-95b5-c1ce724b4ee8.gif" width="100%" height="100%"/></div>
</div
<hr />

## (5)CFormView: Delete the Call to ResizeParentToFit()

<div align=center id ="MFCAppDev_FormView"><img src="https://user-images.githubusercontent.com/26355688/178399844-1678d591-160b-46ec-b2b8-c17711c88c4a.gif" width="100%" height="100%"/></div>
<hr />

## (6)Serialization

<div align=center id ="MFCAppDev_Serialization"><img src="https://user-images.githubusercontent.com/26355688/178399660-91de2238-936b-4ac6-bb44-c4f41f641cb6.gif" width="100%" height="100%"/></div>
<hr />
  
