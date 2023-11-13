<h1>Define Directory Home Lab</h1>

<h2>Description</h2>
In this lab, we will walk through an Active directory home lab Environment Using Oracle Virtual Box. Configuration and running this lab will define and help understand how active directory and Windows networking works, So I'd highly recommend running through it a couple of times.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Oracle Vbox </b> 
- <b>Windows 10</b>
- <b>Server 2019</b> 

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Home Lab Setup</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }
    h3 {
      color: #007BFF;
    }
  </style>
</head>
<body>

<h3>Step 1: Install VirtualBox</h3>

<ol>
  <li><strong>Download and Install VirtualBox:</strong>
    <ul>
      <li>Visit the official VirtualBox website and download the latest version.</li>
      <li>Follow the installation instructions for your operating system.</li>
    </ul>
  </li>
</ol>

<h3>Step 2: Create a Virtual Machine for Windows Server</h3>

<ol>
  <li><strong>Download Windows Server ISO:</strong>
    <ul>
      <li>Obtain the Windows Server ISO file from the official Microsoft website.</li>
    </ul>
  </li>
  <li><strong>Create a New Virtual Machine:</strong>
    <ul>
      <li>Open VirtualBox and click on "New" to create a new virtual machine.</li>
      <li>Name the VM and select "Microsoft Windows" as the type and version.</li>
    </ul>
  </li>
  <li><strong>Allocate Resources:</strong>
    <ul>
      <li>Assign an appropriate amount of RAM and create a new virtual hard disk.</li>
    </ul>
  </li>
  <li><strong>Mount the ISO:</strong>
    <ul>
      <li>In the VM settings, mount the Windows Server ISO in the virtual optical drive.</li>
    </ul>
  </li>
  <li><strong>Install Windows Server:</strong>
    <ul>
      <li>Start the VM and follow the Windows Server installation prompts.</li>
    </ul>
  </li>
</ol>

<!-- Repeat similar structure for each step -->

</body>
</html>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Creating DC server: <br/>
<img src="https://i.imgur.com/kkfssSV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Create Password and finalize setup : <br/>
<img src="https://i.imgur.com/5AHCStB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Importance of Windows Server VM</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }
    h1, h2 {
      color: #007BFF;
    }
  </style>
</head>
<body>

<h1>Creation of Windows Server VM: Significance and Importance</h1>

<h2>1. Virtualization Concept:</h2>
<p><strong>What is Virtualization?</strong> Virtualization is the process of creating a virtual instance of a computer system within another, allowing multiple operating systems to run on a single physical machine.</p>

<h2>2. Importance of Windows Server VM:</h2>
<ul>
  <li><strong>Server Operating System:</strong> Windows Server is a specialized operating system designed for server environments, providing features essential for managing network resources, security, and services.</li>
  <li><strong>Isolation and Resource Allocation:</strong> Creating a Windows Server VM isolates the server environment from the host machine, allowing specific resource allocation (CPU, RAM, storage) without impacting the host.</li>
  <li><strong>Testing and Learning:</strong> Virtualized Windows Server environments are ideal for testing and learning, enabling experimentation with configurations, Active Directory settings, and various server roles.</li>
</ul>

<h2>3. Why VirtualBox?</h2>
<ul>
  <li><strong>Virtualization Platform:</strong> VirtualBox is a free, open-source virtualization platform supporting various guest operating systems, making it versatile for labs and testing.</li>
  <li><strong>Snapshot and Restore:</strong> VirtualBox allows snapshots for easy experimentation, providing the ability to revert to previous states if needed.</li>
  <li><strong>Portability:</strong> VMs created in VirtualBox are portable, facilitating easy transfer and use on other machines with VirtualBox installed.</li>
</ul>

<h2>4. Installation of Windows Server:</h2>
<ul>
  <li><strong>ISO Mounting:</strong> To install Windows Server, mount the Windows Server ISO file in the virtual optical drive of the VM.</li>
  <li><strong>Configuration:</strong> During installation, configure settings such as the server's name, networking parameters, and security options.</li>
</ul>

<h2>5. Role in Active Directory Setup:</h2>
<p><strong>Domain Controller:</strong> The Windows Server VM becomes the foundation for setting up Active Directory, serving as the domain controller responsible for managing user accounts, group policies, and directory services.</p>

<p>In summary, creating a Windows Server VM in VirtualBox provides an isolated, configurable, and portable environment for installing and running the Windows Server operating system, becoming the cornerstone for establishing an Active Directory infrastructure in your home lab.</p>

</body>
</html>

<p align="center">
After Installation : <br/>
<img src="https://i.imgur.com/tViFC6s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Os loaded and Server startup: <br/>
<img src="https://i.imgur.com/OxS1a6H.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Active Directory Setup Diagram</title>
  <style>
    body {
      font-family: Arial, sans-serif;
    }
    .box {
      border: 1px solid #000;
      padding: 10px;
      margin: 10px;
      background-color: #f0f0f0;
    }
  </style>
</head>
<body>

<div class="box">
  <strong>Home Lab Setup</strong>
</div>

<div class="box">
  <strong>Virtualization Platform</strong>
  <div>
    <strong>(e.g., VirtualBox)</strong>
  </div>
</div>

<div class="box">
  <strong>Create VM for Windows Server</strong>
  <div>
    <strong>(e.g., VirtualBox)</strong>
  </div>
</div>

<div class="box">
  <strong>Install Windows Server on the VM</strong>
</div>

<div class="box">
  <strong>Install Active Directory Services</strong>
</div>

<div class="box">
  <strong>Configure Active Directory: Add Roles and Features</strong>
</div>

<div class="box">
  <strong>Set up Networking</strong>
  <div>
    <strong>(e.g., IP configuration)</strong>
  </div>
</div>

<div class="box">
  <strong>Update Windows Server</strong>
  <div>
    <strong>with the latest security patches</strong>
  </div>
</div>

<div class="box">
  <strong>Test Active Directory Environment</strong>
  <div>
    <strong>Create users and groups</strong>
  </div>
</div>

<div class="box">
  <strong>Snapshot and Backup VM</strong>
</div>

<div class="box">
  <strong>Additional Configurations</strong>
  <div>
    <strong>- Configure Group Policies</strong>
    <br>
    <strong>- Install Additional Services (Optional)</strong>
  </div>
</div>

<div class="box">
  <strong>Active Directory Environment Setup Completed!</strong>
</div>

</body>
</html>

<p align="center">
Diagram explanation: <br/>
<img src="https://i.imgur.com/aHFlMyQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Importance of Renaming IP Addresses</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }
    h1, h2 {
      color: #007BFF;
    }
    ol, ul {
      margin-bottom: 20px;
    }
  </style>
</head>
<body>

<h1>Importance of Renaming IP Addresses</h1>

<ol>
  <li><strong>Network Identification:</strong>
    <ul>
      <li><strong>Uniqueness:</strong> IP addresses serve as unique identifiers for devices on a network. Renaming IP addresses ensures distinct and recognizable identities.</li>
    </ul>
  </li>

  <li><strong>Domain Controller Role:</strong>
    <ul>
      <li><strong>Role in Active Directory:</strong> A Domain Controller is a central server in an Active Directory environment responsible for authentication, authorization, and directory services. Consistent and identifiable IP addresses are vital for stability.</li>
    </ul>
  </li>

  <li><strong>Consistency in Network Configuration:</strong>
    <ul>
      <li><strong>Uniform Configuration:</strong> Renaming IP addresses helps maintain a consistent and organized network configuration, simplifying troubleshooting and management tasks.</li>
    </ul>
  </li>

  <li><strong>Avoiding IP Address Conflicts:</strong>
    <ul>
      <li><strong>Preventing Conflicts:</strong> Renaming IP addresses helps prevent conflicts and confusion in the network, reducing the risk of connectivity issues.</li>
    </ul>
  </li>

  <li><strong>DNS and Active Directory Integration:</strong>
    <ul>
      <li><strong>DNS Resolution:</strong> Domain Controllers rely on DNS for name resolution. Renaming IP addresses ensures proper DNS records and name resolution within the Active Directory domain.</li>
    </ul>
  </li>

  <li><strong>Scalability and Flexibility:</strong>
    <ul>
      <li><strong>Scalability:</strong> Renaming IP addresses allows for scalability, accommodating changes in the network as it expands or undergoes modifications.</li>
    </ul>
  </li>

  <li><strong>Documentation and Traceability:</strong>
    <ul>
      <li><strong>Documentation:</strong> Renaming IP addresses contributes to clear documentation, aiding future administrators in understanding the network architecture.</li>
    </ul>
  </li>

  <li><strong>Security Considerations:</strong>
    <ul>
      <li><strong>Security Policies:</strong> Renaming IP addresses can be part of a security strategy, enhancing the overall security posture of the network.</li>
    </ul>
  </li>

  <li><strong>Preventing Service Disruption:</strong>
    <ul>
      <li><strong>Minimizing Disruption:</strong> Planned changes, including renaming IP addresses, help minimize disruptions to services and users.</li>
    </ul>
  </li>

  <li><strong>Compliance and Best Practices:</strong>
    <ul>
      <li><strong>Alignment with Best Practices:</strong> Renaming IP addresses aligns with best practices for network management and administration, promoting a structured approach.</li>
    </ul>
  </li>
</ol>

</body>
</html>


<p align="center">
Renaming IP address and name properties: <br/>
<img src="https://i.imgur.com/2HgVBfZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Adding a Domain to Active Directory</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }
    h1, h2 {
      color: #007BFF;
    }
    ol, ul {
      margin-bottom: 20px;
    }
  </style>
</head>
<body>

<h1>Adding a Domain to Active Directory</h1>

<ol>
  <li><strong>Prepare the Environment:</strong>
    <ul>
      <li>Ensure the existing Active Directory environment is healthy and reachable.</li>
      <li>Verify hardware and software requirements for the new server.</li>
    </ul>
  </li>

  <li><strong>Install Windows Server on the New Server:</strong>
    <ul>
      <li>Create a new virtual machine or use a physical server.</li>
      <li>Install Windows Server on the new server.</li>
    </ul>
  </li>

  <li><strong>Join the Server to the Existing Domain:</strong>
    <ul>
      <li>During installation, specify joining the existing domain.</li>
      <li>Provide credentials with sufficient permissions.</li>
    </ul>
  </li>

  <li><strong>Promote the Server to a Domain Controller:</strong>
    <ul>
      <li>Open Server Manager and add the Active Directory Domain Services role.</li>
      <li>Run the Active Directory Domain Services Configuration Wizard.</li>
      <li>Choose to add a domain controller to an existing domain.</li>
      <li>Provide necessary credentials and select the domain.</li>
    </ul>
  </li>

  <li><strong>Configure DNS and Global Catalog:</strong>
    <ul>
      <li>Ensure DNS is installed and points to the existing DNS server.</li>
      <li>Consider making the new domain controller a Global Catalog server.</li>
    </ul>
  </li>

  <li><strong>Replication and Data Transfer:</strong>
    <ul>
      <li>Allow time for data replication from the existing domain controller.</li>
      <li>Monitor the replication process.</li>
    </ul>
  </li>

  <li><strong>Verify Domain Addition:</strong>
    <ul>
      <li>Use tools like Active Directory Users and Computers to verify visibility.</li>
      <li>Check Event Viewer for any related errors or warnings.</li>
    </ul>
  </li>

  <li><strong>Testing and Troubleshooting:</strong>
    <ul>
      <li>Create test users and groups to ensure successful replication.</li>
      <li>Test domain logins and permissions.</li>
    </ul>
  </li>

  <li><strong>Backup and Documentation:</strong>
    <ul>
      <li>Perform a backup of the new domain controller.</li>
      <li>Update documentation with information about the new domain controller.</li>
    </ul>
  </li>

  <li><strong>Monitor and Maintain:</strong>
    <ul>
      <li>Regularly monitor health and performance.</li>
      <li>Implement a maintenance plan for updates and security patches.</li>
    </ul>
  </li>
</ol>

</body>
</html>

<p align="center">
Adding roles and promoting DC: <br/>
<img src="https://i.imgur.com/tj9gHPm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Installation: <br/>
<img src="https://i.imgur.com/b3YHXc9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Building Active Directory with Server Manager</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      max-width: 800px;
      margin: 20px auto;
    }
    h1, h2 {
      color: #007BFF;
    }
    ol, ul {
      margin-bottom: 20px;
    }
  </style>
</head>
<body>

<h1>Building Active Directory with Windows Server Manager</h1>

<ol>
  <li><strong>Install Windows Server:</strong>
    <ul>
      <li>Install Windows Server on the target machine.</li>
      <li>Ensure the server meets the hardware and software requirements.</li>
    </ul>
  </li>

  <li><strong>Configure Static IP Address:</strong>
    <ul>
      <li>Assign a static IP address to the server.</li>
    </ul>
  </li>

  <li><strong>Install Active Directory Domain Services (AD DS):</strong>
    <ul>
      <li>Open Windows Server Manager.</li>
      <li>Click on "Add roles and features."</li>
      <li>Select "Active Directory Domain Services" and any additional features.</li>
      <li>Complete the installation process.</li>
    </ul>
  </li>

  <li><strong>Promote the Server to a Domain Controller:</strong>
    <ul>
      <li>Open the Active Directory Domain Services Configuration Wizard.</li>
      <li>Choose "Add a new forest."</li>
      <li>Set domain information and forest functional level.</li>
      <li>Set a Directory Services Restore Mode (DSRM) password.</li>
      <li>Complete the installation process.</li>
    </ul>
  </li>

  <!-- Continue the list with the remaining steps -->

</ol>

<p>Refer to Microsoft's official documentation for detailed guidance and best practices.</p>

</body>
</html>

<p align="center">
Setup: <br/>
<img src="https://i.imgur.com/WuDqcdL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
