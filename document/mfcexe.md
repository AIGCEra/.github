<div align=center>

# Convertng MFC Desktop Application <br>into Chromium Project Browser Process

<div align=center id="MfcApp"><img src="https://user-images.githubusercontent.com/26355688/178436304-730ede1e-23c1-4bc9-b94b-4b082dc3e7ab.jpg" width="75%" height="100%"/></div>
<div align=center>
  
## (1)Preparation: This step is required <br>_for all types of MFC Desktop Applications_

### <div align=left>You need to create a new MFC project using the MFC development wizard, or prepare an existing MFC Project:</div>
<div align=center id="MFCAppDev_Prepare"><img src="https://user-images.githubusercontent.com/26355688/178929103-5ef5b22a-4618-4e41-ae73-5bc1ff4ebc02.gif" width="100%" height="100%"/></div>
<hr />

## (2)AppBase: Replace CWinApp(Ex) with CWebRTApp(Ex), <br>MDIFrameBase: Replace CMDIFrameWndEx with CWebRTMDIFrame<br>
<div align=left>

### _If your Application is Tabbed MDI Application_:<br><br><div align=center>Replace</div><br><div align=center>BEGIN_MESSAGE_MAP(CMainFrame, CMDIFrameWndEx)</div><br><div align=center>with</div><br><div align=center>BEGIN_MESSAGE_MAP(CMainFrame, CWebRTMDIFrame)</div>

  
### _More information after Replace CWinApp(Ex) with CWebRTApp(Ex)_:
  
| _MFC Application Type_       | _description_                                                                                                    |
| -- | ---------------------------------------------------------------------------------------------------------------- |
|  <div align=center>**If your app is an MFC Dialog Type Application**</div> |&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  <div align=center id="MFCAppDev_dlg"><img src="https://user-images.githubusercontent.com/26355688/178935032-29f4b4f5-7b91-41b7-a0de-2943368bb3ce.gif" width="100%"/></div>                           |
</div>   
  
## (3)CFormView: <br>Delete the Call to ResizeParentToFit()

<div align=center id ="MFCAppDev_FormView"><img src="https://user-images.githubusercontent.com/26355688/178399844-1678d591-160b-46ec-b2b8-c17711c88c4a.gif" width="100%" height="100%"/></div>
<hr />

## (4)Serialization

<div align=center id ="MFCAppDev_Serialization"><img src="https://user-images.githubusercontent.com/26355688/178399660-91de2238-936b-4ac6-bb44-c4f41f641cb6.gif" width="100%" height="100%"/></div>
