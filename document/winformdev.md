<div align=center>

# Converting WinForm Application <br>into Chromium Project Browser Process
  
</div>
  
<div align=center id="GridNode"><img src="https://user-images.githubusercontent.com/26355688/178513189-7108ee88-9bf4-4cca-bea4-ca2ee9a9a3a7.gif" width="80%" /></div>

<hr />
<div align=center>

# Prepare a C# WinForm Project <br>(create a new Project, or open an existing Project).
</div>
<div>
  
**Here we preset the name of the project as "Tangram". All WinForm projects need the following three steps to support Web Runtime.**
  
</div>
<div align=center>

## (1)Reference “cosmos.dll”, adjust manifest configuration
</div>
<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/181695908-5c796645-f37c-44f7-bcba-6270cf20b748.jpg" width="80%"/></div>
<hr />
<div align=center>

## (2)Adjust compilation configuration
</div>
<div align=center id ="WinFormDev_compilecfg"><img src="https://user-images.githubusercontent.com/26355688/181693960-f4857d56-3cb4-427f-896e-1574c391f409.jpg" width="80%"/></div>
<hr />
<div align=center>
  
## (3)Open "program.cs" file.
</div>

## _Modify main function_, Replace:<br><br><div align=center>Application.Run</div><br><div align=left>with</div><br><div align=center>Universe.WebRT.Run</div><br><div align=center id ="program_main"><img src="https://user-images.githubusercontent.com/26355688/180941619-45fde4d7-2830-4e72-944f-2ad41e047fb0.jpg" width="100%"/></div>

</div>
