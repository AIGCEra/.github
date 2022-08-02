<h1 align=center>

[Open Web Runtime Source Code](https://github.com/TangramDev/OpenWebRuntime)
</h1>
<h3 align=center><div align=center id="StartTitle"><img src="https://user-images.githubusercontent.com/26355688/179231601-e18d1e1d-c4a1-422c-bcf3-7111013959bb.gif" width="100%" /></div>(In most scenarios, Desktop Software is like a Universe, with many local huge worlds hidden around numerous child windows, and the Web Runtime is a space telescope, revealing the depths of the universe that have been hidden from the developer's sight...)
</h3>

<h1 align=center><strong>Tribute to Classic</strong>           
<h2>
<p>At different stages of Scientific and Technological Development, there will be classics corresponding to the era to embellish the marvellous of that era. The classic is called a "classic" not only because of its own value, but also because it has a profound impact on a specific historical period. How should we pay tribute to the classics? Letting them conform to the rhythm of the times to continue may be a way to pay homage to the classics. We are lucky because we have benefited from a large number of classics, those who made classics, those achievements let us see further and inspire us to continue to create...<p>

<p>There is no doubt that the Chromium Project is a "fully deserve" classic in the Internet age, Visual Studio Wizard is also a classic that has influenced generations of developers. When we enter the era of Internet entrance competition between Microsoft and Google based on "Chromium Project", we are not only the audience in the giant competition field, of course, we expect to become a member of the competition field, otherwise the Oligarchic Competition stage will become a little boring. Web Runtime attempts to build a larger <i>Web DOM</i> and bring together more classic works. If we can only carry out according to the specifications formulated by chromium, then we are doomed to be spectators, and we may have to applaud the competition between giants, so it is imperative to change the rules.</p>
<p>The mission of Web Runtime is to allow more desktop software developers to inherit the advantages of the Chromium Project to the greatest extent, and at the same time, it can also best continue the technical accumulation of the developers themselves. Further, considering the basic characteristics of Web technology, we hope to reasonably expand the boundaries of the Web, and then the technical resources from the .NET Framework, COM, C++ and many other infrastructures will be incorporated into the scope of the Web.</p>

</h2> 
</h1> 

<h1 align=center>

The Basic Concepts for Web Runtime
</h1>
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Basic Concepts</strong>
                    <th> <strong>Description</strong>
                </tr>
             <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Window Nucleus</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>
If the Runtime Position of a  Child Window only depends on the
<p>
<div align=center>

[WM_WINDOWPOSCHING](https://docs.microsoft.com/en-us/windows/win32/winmsg/wm-windowposchanging)
</div>
</p>
<p>
<h3>

Message of its Parent Window, then this Child Window is called a [Window Nucleus](https://github.com/TangramDev/.github/blob/main/WinNucleusDef.md) of its Parent Window, any <ins><i>Parent Window</ins></i> of Window Nucleus is called a <ins><i>Nucleated Window</i></ins>.
</p>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Browser Process</strong></j3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>The Main Process of the Chromium Project is called the Chromium Project Browser Process, 
                        which provides the UI system for Web Browsers.
                        </h3>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Common Component Space</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>We call the set of all <ins><i>Dynamic Link Libraries</i></ins> that can provide <ins>Component Services</ins> (object services or UI services, such as providing Controls, Windows. Forms, etc.) for other <i>Desktop Applications</i> as the "Common Component" Space.<h3>             
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Private Component Space of Desktop Software</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>The components from the main process and those components from all the dynamic link library which directly depend on the main process form a set,  which is called the "private component space of desktop software".<h3>
                    </td>
                </tr>
            </tbody>
            <tbody>
                <tr>
                    <td width="25%">
                        <h3 align=center><strong>Component Space of Desktop Software</strong></h3>
                    </td>
                    <td width="75%" rowspan=5>
                        <h3>The union set of "<ins>Common Component Space</ins>" and "<ins>Private Component Space of Desktop software</ins>" is called "<ins>Component Space of Desktop software</ins>".<h3>
                    </td>
                </tr>
            </tbody>
        </table>
    </center>

<h1 align=center>
Two Core Jobs of Web Runtime
</h1>
<h2>    
<p>Web Runtime will make Desktop Applications the Organizer and Scheduler of Various Application Components (such as COM, .NET, C++ components, etc.) based on Web-driven technology.
</p>
<center>
        <table border="3" cellpadding="3">
            <thead>
                <tr>
                    <th> <strong>Core Job</strong>
                    <th> <strong>Description</strong>
                </tr>
            <tbody>
                <tr>
                    <td width="25%">
                        <p align=center><strong>Convert Windows Desktop Software Projects into Chromium Project Browser Processes</strong></p>
                    </td>
                    <td width="75%" rowspan=5>
                        <p>The Web Runtime provides developers with a "<i>Simplest Technical Strategy</i>" <ins>to convert "existing" or "newly created" <i>Desktop Software Projects</i> into "<i>Browser Processes</i>" of "Chromium Project"</ins>, it will completely eliminate the gap between <i>the Desktop Software</i> and <i>Web Browser</i> and makes Web Technology an inherent part of <i>Desktop Software Architecture</i>: 
                            </p>
<div align=center>
<p > 

[<ins>WinForm Project</ins>](https://github.com/TangramDev/.github/blob/main/document/winformdev.md)&emsp;&emsp;[<ins>MFC Project</ins>](https://github.com/TangramDev/.github/blob/main/document/mfcexe.md)</p>
</div>
                            <p>When a Desktop Software Process is converted into a Chromium Browser Process, the Desktop Software Process naturally integrates all the Chromium Browser UI Mechanism from the Chromium technology system, which means that the original UI mechanism is broken. Web Runtime tells us that the breakthrough of the boundary is just the beginning, once the Desktop Process itself has the ability to drive the web, more UI Mechanism parallel to the Browser Window(for example: WinForms UI mechanism) will follow. Every Desktop Application-Oriented Browser Process will contain a structure similar to the Universe, Converting the Desktop Process into the Browser Process is the beginning of this prologue...
                            </p>
                    </td>
                </tr>
            </tbody>            
            <tbody>
                <tr>
                    <td width="25%">
                        <p align=center><strong>Build a "Local Web Description Space" around every Window nucleus</strong></p>
                    </td>
                    <td width="75%" rowspan=5>
                        <h4 align=left>
                        <p>
                        The theory of relativity tells us, that massive matter causes the space around it producing "space-time bending", which in turn enables other small-mass matter to revolve around it, <ins>the Window Nucleus has a similar effect on the geometric space around it: the window nucleus can deform the surrounding space according to the geometric layout structure controlled by the Web, and then form a surrounding geometric layout, the UI elements in the "Component Space of Desktop Software" will find their "position" in the specific layout. This geometric effect is similar to the theory of relativity, and it is the theoretical basis for Web Runtime to form a new Web technology entrance.</ins>
                        </p>
                        <p align=center id="LayoutLayer"><img src="https://user-images.githubusercontent.com/26355688/182055784-6b9fd7c0-2328-428a-9b64-e8b65ba8f316.jpg" width="100%"/>
                        </p>
                        <p>
                        For all Desktop Software Developers, the Window Nucleus is a brand new concept, since it is a "Nucleus", it must be surrounded by other objects. One of the core tasks of Web Runtime is to reveal that the Window Nucleus is surrounded by a huge content world driven by Web Description, this content world is a New World that software developers have not touched so far ...
                        </p>
                        <p>Taking the Window Nucleus as the <ins><i>Local Center</ins></i>, based on the <ins><i>Component Space of Desktop Software</ins></i> and <ins><i>Web Driving Technology</ins></i>, establish a "<ins><i>Local Web Description Space</ins></i>" around the Window Nucleus to realize the <i>Dynamic Description</i>, <i>Creation</i> and <i>Control</i> of <ins>Desktop Windows</ins> based on Web Technology.
                        </p>
                        </h4>
                     </td>
                </tr>
            </tbody>            
         </table>
</center>    
<div align=right>

[More Information ...](https://github.com/TangramDev/.github/blob/main/document/readmeex.md)
</div>
</h2>
