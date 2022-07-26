<div align=center>

# Converting MFC Application <br>into Chromium Project Browser Process

<div align=center id="MfcApp"><img src="https://user-images.githubusercontent.com/26355688/178436304-730ede1e-23c1-4bc9-b94b-4b082dc3e7ab.jpg" width="67%" height="100%"/></div>
<div align=center>
  
## (1)Prepare a MFC Project <br>(create a new Project, or open an existing Project).
<div align=center>
  
### <div align=center id="MFCAppDev_Prepare"><img src="https://user-images.githubusercontent.com/26355688/178929103-5ef5b22a-4618-4e41-ae73-5bc1ff4ebc02.gif" width="100%" height="100%"/></div>
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

<div align=center id ="MFCAppDev_Serialization"><img src="https://user-images.githubusercontent.com/26355688/178399660-91de2238-936b-4ac6-bb44-c4f41f641cb6.gif" width="100%" height="100%"/></div>
