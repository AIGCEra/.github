<div align=center>

# Converting MFC Application <br>into Chromium Project Browser Process
  
<div align=center>

## (1)Prepare a MFC Project <br>(create a new Project, or open an existing Project)
<div align=center>

<h3 align=left>
<p>
  
Copy all files included with [***MFCPlus***](https://github.com/TangramDev/OpenWebRunTime/tree/master/src/sdk/MFCPlus) into the prepared MFC desktop software project.</p>

<div align=center id="mfcdevmanifest"><img src="https://user-images.githubusercontent.com/26355688/181698116-74b3824c-4e1b-457e-92c4-587d4c0b914b.jpg" width="80%"/></div>
</h3>
<hr />

## (2)AppBase: Replace CWinApp(Ex) with CWebRTApp(Ex)
  
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr style="font-size: 16px; font-weight:bold; color:midnightblue">
                    <th> <h3>Tabbed MDI Application</h3>
                    <th> <h3>Dialog Application</h3>
                </tr>
            <tbody>
                <tr>
                    <td width="50%">
			<p><strong>MDIFrameBase: Replace CMDIFrameWndEx with CWebRTMDIFrame,</strong></p>
                        <p>Replace</p><p align=center><strong>BEGIN_MESSAGE_MAP(CMainFrame, CMDIFrameWndEx)</strong></p><p align=left>with</p><p align=center><strong align=center>BEGIN_MESSAGE_MAP(CMainFrame, CWebRTMDIFrame)</strong></p>
                    </td>
                    <td class="sunnysolution" width="50%" rowspan=5>
                        <p>Modify the return value of </p><p><div align=center><strong>BOOL CMFCDlgApp::InitInstance()</strong></p><p align=left>to</p> <p align=center><strong>TRUE</strong>.</p>
                        </p>
                    </td>
            </tbody>
            <thead>
                <tr style="font-size: 16px; font-weight:bold; color:midnightblue">
                    <th> <h3>CFormView</h3>
                    <th> <h3>Document Serialization</h3>
                </tr>
            <tbody>
            <tbody>
                <tr>
                    <td class="sunnysolution" width="50%">
                        <p align=left>For "CFormView Derived Class", you need to remove the Call:</p><p align=center><strong>ResizeParentToFit();</strong></p> <p>from</p><p align=center><strong>OnInitialUpdate();</strong> </p>
                    </td>
                    <td class="sunnysolution" width="50%">
                      </p>
                        <p>Add the following serialization code in the body of the Serialize (CArchive & ar) function:                            
                        </p>
                      <p>                   
                      
    void CMFCApplicationDoc::Serialize(CArchive& ar){
	  if (ar.IsStoring())
	  {
		  ar << theApp.GetDocTemplateID(this);	
		  // TODO: add storing code here
	  }
	  else
	  {
		  ar >> theApp.m_strCreatingDOCID;
		  // TODO: add loading code here
	  }
    }
</p>
                    </td>
            </tbody>
        </table>
</center>  
 
