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
  
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr style="font-size: 16px; font-weight:bold; color:midnightblue">
                    <th> <h3>MFC Tabbed MDI Application</h3>
                    <th> <h3>MFC Dialog Application</h3>
                </tr>
            <tbody>
                <tr>
                    <td class="sunnysolution" width="50%">
                        <p>Replace</p><p align=center><strong>BEGIN_MESSAGE_MAP(CMainFrame, CMDIFrameWndEx)</strong></p><p align=left>with</p><p align=center><strong align=center>BEGIN_MESSAGE_MAP(CMainFrame, CWebRTMDIFrame)</strong></p>
                    </td>
                    <td class="sunnysolution" width="50%" rowspan=5>
                        <p>Modify the return value of </p><p><div align=center><strong>BOOL CMFCDlgApp::InitInstance()</strong></p><p align=left>to</p> <p align=center><strong>TRUE</strong>.</p>
                        </p>
                    </td>
            </tbody>
            <thead>
                <tr style="font-size: 16px; font-weight:bold; color:midnightblue">
                    <th> <h3>MFC CFormView</h3>
                    <th> <h3>Serialization</h3>
                </tr>
            <tbody>
            <tbody>
                <tr>
                    <td class="sunnysolution" width="50%">
                        <p align=left>For "CFormView Derived Class", you need to remove the Call:</p><p align=center><strong>ResizeParentToFit();</strong></p> <p>from</p><p align=center><strong>OnInitialUpdate();</strong> </p>
                    </td>
                    <td class="sunnysolution" width="50%">
                        <p>Add the following serialization code in the body of the Serialize (CArchive & ar) function:
                            <div align=center id ="mfc_serialization"><img src="https://user-images.githubusercontent.com/26355688/181708729-873e05bb-8212-469b-aa5c-c9108a520434.jpg" width="80%"/></div>
                        </p>
                    </td>
            </tbody>
        </table>
</center>  
 
