<div align=center>

# Converting WinForm Application <br>into Chromium Project Browser Process
  
</div>

<div>
  
<h2>Prepare a C# WinForm Project(create a new Project, or open an existing Project), All WinForm projects need the following three steps to support Web Runtime.
  
</div>
<div align=center>

## (1)Reference “cosmos.dll”, adjust manifest configuration
</div>
<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/183279374-c7684046-c242-4f36-b246-0f4dec7361db.jpg" width="80%"/></div>
<hr />
<div align=center>

## (2)Adjust compilation configuration
</div>
<div align=center id ="WinFormDev_compilecfg"><img src="https://user-images.githubusercontent.com/26355688/183279105-219cf910-3b5a-48d1-be85-d8a4e23a6c88.jpg" width="80%"/></div>
<hr />
<div align=center>
  
## (3)Open "program.cs" file.
</div>

## _Modify main function_, Replace:<br><br><div align=center>Application.Run</div><br><div align=left>with</div><br><div align=center>Universe.WebRT.Run</div>
</h2>
