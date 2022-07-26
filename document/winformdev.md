<div align=center>

# Converting WinForm Application <br>into Chromium Project Browser Process
  
</div>
  
<div align=center id="GridNode"><img src="https://user-images.githubusercontent.com/26355688/178513189-7108ee88-9bf4-4cca-bea4-ca2ee9a9a3a7.gif" width="80%" /></div>

<hr />
<div align=center>
  
# Prepare a C# WinForm Project <br>(create a new Project, or open an existing Project).
</div>
<div>
  
  **Here we preset the name of the project as "FirstApp". All WinForm projects need the following three steps to support Web Runtime.**
  
</div>
<div align=center>

## (1)Reference “cosmos.dll”, adjust manifest configuration
</div>
<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/180914430-4293ce50-3896-408d-b45e-ce91471c766f.gif" width="100%" height="100%"/></div>
<hr />
<div align=center>
  
## (2)Adjust compilation configuration
</div>
<div align=center id ="WinFormDev_compilecfg"><img src="https://user-images.githubusercontent.com/26355688/178502697-56718182-8cf0-43f6-944e-fad62db908aa.gif" width="100%" height="100%"/></div>
<hr />
<div align=center>
  
## (3)Open "program.cs" file.
</div>

## _Modify main function_:<br><br><div align=center>Replace</div><br><div align=center>Application.Run</div><br><div align=center>with</div><br><div align=center>Universe.WebRT.Run</div>

</div>
