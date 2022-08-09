# MFC Document Serialization

<strong>
                      </p>
                        <p>Add the following serialization code in the body of the Serialize (CArchive & ar) function:                            
                        </p>
                      <p>                   
                      
                      void CMFCApplicationDoc::Serialize(CArchive& ar){
                        if (ar.IsStoring())
                        {
                          ar << theApp.GetDocTemplateID(this);
                        }
                        else
                        {
                          ar >> theApp.m_strCreatingDOCID;
                        }
                      }
</p>
</strong>
