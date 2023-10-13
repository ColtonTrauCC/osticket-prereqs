<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align = "center">osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>
<ol>
  <li>Set up an Azure Virtual Machine (VM) environment (Windows 10 4 vCPUs Recommended)</li>
  <li><a href = "https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">osTicket Installation Files</a> (Download these files on your Azure Virtual Machine) </li>
  <li>Enable IIS in I.S.S.</li>
  <li>Install Web Platform Installer</li>
  <li>Install MySQL and set up username and password</li>
    <ul>
    <li>For this tutorial, we will set up our username and password as such:</li>
      <ul>
      <li>username: root</li>
      <li>password: Password1</li>
      </ul>
    </ul>
  <li>Install C++ Redistributable</li>
  <li>Configure permissions and install osTicket</li>
</ol>

<h2>Installation Steps</h2>

<h3>Install / Enable IIS in Windows WITH CGI and Common HTTP Features</h3>

<p>
  <ul>
    <li>In your VM, go to the <b>Control Panel</b> and head to <b>Programs</b>. </li>
    <li>Under <b>Program and Features</b> click on <b>Turn Windows features on or off</b></li>
    <li>Navigate the list and check the box for <b>Internet Information Services</b></li>
    <li>Expand the list for <b>Internet Information Services</b>, navigate to <b>World Wide Web Services</b> then expand that to find <b>Application Development Features</b>, expand that and check the box for <b>CGI</b>.</li>
    <li>Before closing, make sure the boxes under <b>Common HTTP Features</b> in World Wide Web Services are checked.</li>
      <ul>
        <li><b>Check these boxes in Turn Windows Features on or off</b></li>
        <li><img src="https://github.com/ColtonTrauCC/osticket-prereqs/assets/147654000/e770403c-5def-4c58-a2ad-24b61a859078" height="50%" width="50%" alt="Disk Sanitization Steps"/></li>
      </ul>
    <li>To confirm everything is set accordingly, go to your browser in your VM and type in <b>127.0.0.1</b>, it should load the page to Internet Information Services</li>
      <ul>
        <li><img src="https://github.com/ColtonTrauCC/osticket-prereqs/assets/147654000/b6fdbb5f-73c6-4aaf-ac8c-3e9690303d7b" height="50%" width="50%" alt="Disk Sanitization Steps"/></li>
      </ul>
  </ul>
</p>


<br />

<h3>PHP Manager and Rewrite Module</h3>

<p>
  <ul>
    <li>From the Installation Files, download <b>PHP Manager</b> (PHPManagerForIIS_V1.5.0.msi) and <b>Rewrite Module</b> (rewrite_amd64_en-US.msi) </li>
  </ul>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />
