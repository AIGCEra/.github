<div align=center>

# Converting MFC Application <br>into Chromium Project Browser Process

<div align=center id="MfcApp"><img src="https://user-images.githubusercontent.com/26355688/178436304-730ede1e-23c1-4bc9-b94b-4b082dc3e7ab.jpg" width="67%" height="100%"/></div>
<hr />  
  
<div align=center>

## (1)Prepare a MFC Project <br>(create a new Project, or open an existing Project)
<div align=center>

<h3 align=left>
<p>
  
Copy all files included with [***MFCPlus***](https://github.com/TangramDev/OpenWebRunTime/tree/master/src/sdk/MFCPlus) into the prepared MFC desktop software project.</p>

<div align=center id="mfcdevmanifest"><img src="https://user-images.githubusercontent.com/26355688/181698116-74b3824c-4e1b-457e-92c4-587d4c0b914b.jpg" width="80%"/></div>
</h3>
<hr />

## (2)AppBase: Replace CWinApp(Ex) with CWebRTApp(Ex), <br>MDIFrameBase: Replace CMDIFrameWndEx with CWebRTMDIFrame<br>
<div align=left>

### _If your Application is Tabbed MDI Application_:<br><br><div align=center>Replace</div><br><div align=center>BEGIN_MESSAGE_MAP(CMainFrame, CMDIFrameWndEx)</div><br><div align=center>with</div><br><div align=center>BEGIN_MESSAGE_MAP(CMainFrame, CWebRTMDIFrame)</div>

### For _MFC Dialog Application_, you need to modify the return value of <br><br><div align=center>BOOL CMFCDlgApp::InitInstance()</div> <br>to <div align=center>TRUE. </div> 
<hr />
</div>   
  
## (3)CFormView: <br>Delete the Call to ResizeParentToFit()

### <div align=left>For "CFormView Derived Class", you need to remove the Call:<br><br><div align=center>ResizeParentToFit();</div> <br>from<br><br><div align=center>OnInitialUpdate(); </div> </div>
<hr />

## (4)Serialization
![](https://)

<div align=center id ="mfc_serialization"><img src="https://user-images.githubusercontent.com/26355688/181699626-f1f2ae6e-1c7b-499e-a86d-d09f07c07cdc.jpg" width="80%"/></div>
