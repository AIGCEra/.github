<div align=center>

# Developing WinForm Desktop Application with Web Runtime
  
</div>
  
<div align=center id="FormDemo"><img src="https://user-images.githubusercontent.com/26355688/178508943-38767355-0878-4104-85e7-2a12b50c4d61.gif" width="75%" height="100%"/></div>
<div align=center id="FirstApp"><img src="https://user-images.githubusercontent.com/26355688/178510020-57c78ddb-499c-4bb1-8388-c4d181477e76.gif" width="75%" height="100%"/></div>

<div align=center id="GridNode"><img src="https://user-images.githubusercontent.com/26355688/178513189-7108ee88-9bf4-4cca-bea4-ca2ee9a9a3a7.gif" width="80%" height="100%"/></div>
<div align=center>

# .NET Development of WebRuntime Applications need to pay attention to the following aspects：
  
</div>
<div align=left>
<ol>
<li>Reference cosmos.dll component library</li>
<li>replace "Application.Run" with " Universe WebRT. Run"</li>
<li>correctly process the "manifest configuration" of the .NET project</li>
<li>configure the compilation options correctly(WebRuntime only supports 64-bit applications).</li>
</ol>
</div>
  
</div>
<hr />
<div align=center>
  
# Prepare a C# WinForm Project (create a new Project, or open an existing Project).
</div>
<div>
  
  **Here we preset the name of the project as "FirstApp". All WinForm projects need the following three steps to support Web Runtime.**
  
</div>

## (1)Reference “cosmos.dll”, adjust manifest configuration

<div align=center id ="WinFormDev_manifest"><img src="https://user-images.githubusercontent.com/26355688/178502519-b3f3344c-634e-437a-8d5b-e4851f5d24db.gif" width="100%" height="100%"/></div>
<hr />

## (2)Adjust compilation configuration

<div align=center id ="WinFormDev_compilecfg"><img src="https://user-images.githubusercontent.com/26355688/178502697-56718182-8cf0-43f6-944e-fad62db908aa.gif" width="100%" height="100%"/></div>
<hr />
  
## (3)Open "program.cs" file, Modify main function

<div align=center id="WinFormDev_main"><img src="https://user-images.githubusercontent.com/26355688/178502334-f3e819d3-6898-4d21-b0a4-9efbf805f4aa.gif" width="100%" height="100%"/></div>
<hr />
</div>
