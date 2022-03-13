# windows-secured-uac
<h2>Registry patch which makes Windows UAC more secure. Great solution against ducky scripts.</h2>
<hr>
<h3>Default Windows UAC</h3>

<p>To get administrator privileges in Windows by default you will see "y/n" UAC window.</p>

![default](https://user-images.githubusercontent.com/101452307/158059643-9f165f3e-cc05-44aa-9198-e77d21ac4e12.png)
<p>It's easy way for unauthorized users or malicious scripts to get administrator access.</p>

<h3>How to get Windows UAC more secure?</h3>
<p>In regedit find <b><i>ConsentPromptBehaviorAdmin</i></b> registry key.</p>
<p>Location: [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System]</p>

![reg1](https://user-images.githubusercontent.com/101452307/158060047-5d196a4b-5958-4633-a1d4-dff5c2b29848.png)

<p>Change its value from <b>5</b> to <b>1</b>.</p>

![change](https://user-images.githubusercontent.com/101452307/158060322-f0064776-6bfe-4aca-8136-4ee77c9496d6.png)


![reg2](https://user-images.githubusercontent.com/101452307/158060225-727ff035-9396-4832-9c5b-d7d6d789c160.png)

<h3>Results:</h3>
<p>Now every UAC will prompt you for admin password, making it much harder to baypass.</p>

![patched](https://user-images.githubusercontent.com/101452307/158060454-c044167f-a773-4ef4-bbc7-fca353ad7e63.png)

<hr>

<h4><code>UAC patch.reg</code> file will do this all for you.</h4>



