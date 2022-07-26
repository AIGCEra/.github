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
<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/180940809-4fbef7d2-4d6f-472c-a073-70a9f12c352c.gif" width="100%" height="100%"/></div>
<hr />
<div align=center>

## (2)Adjust compilation configuration
</div>
<div align=center id ="WinFormDev_compilecfg"><img src="https://user-images.githubusercontent.com/26355688/180941030-dfb5c762-1e4b-4bfc-a049-8794d4bd15ac.gif" width="100%" height="100%"/></div>
<hr />
<div align=center>
  
## (3)Open "program.cs" file.
</div>

## _Modify main function_, Replace:<br><br><div align=center>Application.Run</div><br><div align=left>with</div><br><div align=center>Universe.WebRT.Run</div><br><div align=center id ="program_main"><img src="https://user-images.githubusercontent.com/26355688/180941619-45fde4d7-2830-4e72-944f-2ad41e047fb0.jpg" width="100%"/></div>

</div>
