<div align=center>

# [Converting WinForm Application <br>into Chromium Project Browser Process](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)
  
## (1)Prepare a C# WinForm Project<br>(create a new Project, or open an existing Project)
</div>
<h3>Reference “cosmos.dll”, adjust manifest and compilation configurations</h3>


<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/183294437-cf6a3f96-69ed-4274-936c-ba963e21537d.jpg" width="100%"/></div>

<h2 align=center><p>(2)Open "program.cs" file.</p> <p align=left><i>Modify main function</i>, Replace: "Application.Run" with:<p align=center>Universe.WebRT.Run</p></p>
</h2>
