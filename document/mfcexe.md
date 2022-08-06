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

## (2)Base Class Replacement
<h2 align=left><p>AppBase: Replace "public CWinApp(Ex)" with "public CWebRTApp(Ex)"</p><p>MDIFrameBase: Replace "public CMDIFrameWndEx" with "public CWebRTMDIFrame"</p></h2>

## (3)Matters Needing Attention
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Needing Attention</strong>
                    <th> <strong>Description</strong>
                </tr>                     
            <tbody>
                <tr>
                    <td class="sunnysolution" width="30%">
                        <strong><p align=center>Dialog Application</strong> </p>
                    </td>
                    <td class="sunnysolution" width="70%">
		     <strong><p>Modify the return value of</p><p><div align=center>BOOL CMFCDlgApp::InitInstance()</p><p align=left>to</p> <p align=center>TRUE</strong>.</p>
                        </p></strong>
                    </td>
            </tbody>
	    <tbody>
                <tr>
                    <td class="sunnysolution" width="30%">
                        <strong><p align=center>For "CFormView Derived Class"</strong> </p>
                    </td>
                    <td class="sunnysolution" width="50%">
		     <strong><p align=left>For "CFormView Derived Class", you need to remove the Call:</p><p align=center>ResizeParentToFit();</p> <p>from</p><p align=center><strong>OnInitialUpdate();</strong> </p>
</p>
</strong>
                    </td>
            </tbody>
	    <tbody>
                <tr>
                    <td class="sunnysolution" width="30%">
                        <strong><p align=center>Document Serialization</p></strong>
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
