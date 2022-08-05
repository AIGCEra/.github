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

## (2)AppBase: Replace "public CWinApp(Ex)" with "public CWebRTApp(Ex)"
  
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Tabbed MDI Application</strong>
                    <th> <strong>Dialog Application</strong>
                </tr>
            <tbody>
                <tr>
                    <td width="50%">
			<h3><strong>MDIFrameBase: Replace "public CMDIFrameWndEx" with "public CWebRTMDIFrame"</strong></h3>                        
                    </td>
                    <td class="sunnysolution" width="50%" rowspan=5>
                        <strong><p>Modify the return value of</p><p><div align=center>BOOL CMFCDlgApp::InitInstance()</p><p align=left>to</p> <p align=center>TRUE</strong>.</p>
                        </p></strong>
                    </td>
            </tbody>
            <thead>
                <tr style="font-size: 16px; font-weight:bold; color:midnightblue">
                    <th> <strong>CFormView</strong>
                    <th> <strong>Document Serialization</strong>
                </tr>
            <tbody>
            <tbody>
                <tr>
                    <td class="sunnysolution" width="50%">
                        <strong><p align=left>For "CFormView Derived Class", you need to remove the Call:</p><p align=center>ResizeParentToFit();</p> <p>from</p><p align=center><strong>OnInitialUpdate();</strong> </p>
                    </td>
                    <td class="sunnysolution" width="50%">
		      <strong>
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
</strong>
                    </td>
            </tbody>
        </table>
</center>  
 
