<h1 align=center>
Working with <i>Latest Chromium Project Source Code</i>
</h1>
<h2  align=left><p>

We designed [OpenWebRuntime](https://github.com/TangramDev/OpenWebRunTime) to work in sync with the latest Chromium Stable Source Code for Chromium Stable Version. To do this, you need to refer to the 
<div  align=center>
	
[**Building Chromium for Windows**](https://chromium.googlesource.com/chromium/src/+/main/docs/windows_build_instructions.md)</div>

to obtain the source code of the latest full version of the Chromium Project, and to ensure that this version can be compiled correctly so that the compiled results can run properly. The IDE Environment we work here is Visual Studio 2022 17.3.5, which requires C++/CLI support.</p>
</p> 
</h2>
<h1 align=center>
Preparation: <i>Download Chromium Source Code Patch</i>
</h1>
<h2  align=left><p>You'll need to download the latest Canary Patch, Dev Patch, Beta Patch, and Stable Patch zips separately, or some of them, depending on your needs. 
  
<center>
        <table border="3" cellpadding="3" align=center>
	            <tbody>
                <tr>
                    <td width="200" align=center>
                      
[**<i>Canary Patch</i>**](https://github.com/TangramDev/WebRT_Chromium_Canary/archive/refs/heads/main.zip)
                    </td>
                    <td width="200" align=center>
                      
[**<ins><i>Dev Patch</i></ins>**](https://github.com/TangramDev/WebRT_Chromium_Dev/archive/refs/heads/main.zip)
                    </td>
                <tr>
                    <td width="200" align=center>
                      
[**<ins><i>Beta Patch</i></ins>**](https://github.com/TangramDev/WebRT_Chromium_Beta/archive/refs/heads/main.zip)
                    </td>
                    <td width="200" align=center>
                      
[**<i><ins>Stable Patch</ins></i>**](https://github.com/TangramDev/WebRT_Chromium_Stable/archive/refs/heads/main.zip)
                    </td>
          </tbody>	  
        </table>
</center> 
  
Unzip the Patch zip you downloaded separately, you will get four folders.</p>
</p> 
</h2>

<h1 align=center>

How to Use <i>[ChromiumVer.txt](https://github.com/TangramDev/WebRT_Chromium_Canary/blob/main/ChromiumVer.txt)</i>
</h1>
<h2><p>Each Chromium WebRT Patch contains a file "ChromiumVer.txt" to specify the Tag of the Chromium Project version corresponding to the Patch, for example: 106.0.5249.99.</p>
</h2>

<h1 align=center>
How to use <i>Batch Files</i> in Chromium WebRT Patch</i>
</h1>
<h2><p>Each Chromium WebRT Patch contains a group of batch files to handle the various work done by WebRuntime for the Chromium Project, including necessary source code modifications, toolchain adjustments, project compilation, and code synchronization with the Chromium Project.</p>
</h2>

<h2 align=center>

How to Use <i>[GetBranch.Bat](https://github.com/TangramDev/WebRT_Chromium_Canary/blob/main/ChromiumSRC/getbranch.bat)</i>

<p align=left>The role of GetBranch is to create a new source code branch based on the Tag value of the given Chromium Project version. GetBranch.Bat requires two parameters. The first parameter is the Tag value provided by [ChromiumVer.txt](https://github.com/TangramDev/WebRT_Chromium_Canary/blob/main/ChromiumVer.txt), and the second parameter is the name of the new branch you wish to create.</p>
<h2>