# DHCP Installation configuration in Active Directory.




<h2>Description</h2>
This repository provides a comprehensive guide on the steps taken to configure the installation of DHCP on Active Directory. This walkthrough is aimed at system administrators and IT professionals who want to install and configure DHCP in the Active Directory environment.
<br />

<h2>Purpose</h2>
Enumerating the step by step guideline that can be used to install and configure DHCP in Active Directory environment.

<h2>Environments Used </h2>

- <b>VirtualBox</b>
- <b>Windows Server 2019</b>
- <b>PowerShell ISE</b>

<h2>Project walk-through:</h2>

<p align="center">
First step is selecting DHCP and ensuring to select "Management Tools" to ensure that the process of managing and configuring the DHCP can be done after installation has been complete. <br/>
<img src="https://imgur.com/a/VGA12y6.png" height="80%" width="80%" alt="Installing DHCP"/>
<br /> 
<br />
Select Install to kickstart the installation process. <br/>
<img src="https://imgur.com/wWb9X9d.png" height="80%" width="80%" alt="Selec Install to start installation process."/>
<br />
<br />
Installation complete.<br/>
<img src="https://imgur.com/qvVAwla.png" height="80%" width="80%" alt="Installation complete"/>
<br />
<br />
After After installation is complete, proceed to right click on either ipv4 or ipv6 depending on the particular one to be worked on. Select new scope to start configuration process.<br/>
<img src="https://imgur.com/FVaMKec.png" height="80%" width="80%" alt="Inability to run script due to it not being digitally signed"/>
<br />
<br />
Click on the next option after the New Scope configuration page has displayed  <br/>
<img src="https://imgur.com/PGXt0Ce.png" height="80%" width="80%" alt="Start the configuration proces."/>
<br />
<br />
Specify the scope of the DCHP IP addresses that systems and users on the Active Directory environment are going to be configured by. <br/>
<img src="https://imgur.com/8ReAqWd.png" height="80%" width="80%" alt="Specify IP addresses going to be used for configuration"/>
<br />
<br />
Continue the configuration process by setting the start and end of the IP address scope. Also, on this page, the length of the IP address can be specified and also the subnet mask. <br/>
<img src="https://imgur.com/voyYfGW.png" height="80%" width="80%" alt="Advance scope configuration."/>
<br />
<br />
Set DCHP IP address lease duration on this page. The length of the lease duration would depend on the type of the network being worked on. For example, if this is a restuarant kind of network, it is best to set the duration to less than 24hours so the IP address does not get exhuasted. <br/>
<img src="https://imgur.com/zRI4CwT.png" height="80%" width="80%" alt="Setting DHCP IP Address Lease Duration."/>
<br />
<br />
Set the Default Gateway, this is the Router or Access Point the users or systems in the Active Directory environment will utilize to access the internet. <br/>
<img src="https://imgur.com/ib9FoIu.png" height="80%" width="80%" alt="Default Gateway configuration."/>
<br />
<br />
Set the parent domain by filling in the name or address used to name the origin domain. <br/>
<img src="https://imgur.com/XPoNKhg.png" height="80%" width="80%" alt="Configuring parent domain."/>
<br />
<br />
Activate the configured scope to test and confirm that it is all working properly. <br/>
<img src="https://imgur.com/edfLtRl.png" height="80%" width="80%" alt="Activate the scope."/>
<br />
<br />
Complete scope configuration by selecting "Finish". <br/>
<img src="https://imgur.com/4sYl82h.png" height="80%" width="80%" alt="Complete scope configuration."/>
<br />
<br />
Authorize the configured scope by right clicking on the domain icon then selecting "authorize". Authorization means putting it to work or just turning it on, the ipv4 and ipv6 means that it is turned off or unauthorized, when it is on, the red icon the IPv's will turn to green. <br/>
<img src="https://imgur.com/zPBYpQ6.png" height="80%" width="80%" alt="Authorize the configured scope."/>
<br />
<br />
The DHCP scope is now activated, this can be confirmed by seeing that the ipv4 and ipv6 icons have now turned to green. <br/>
<img src="https://imgur.com/lXPvOOe.png" height="80%" width="80%" alt="Activated DHCP scope."/>
<br />
<br />
The configured and activated scope can be confirmed and seen by clicking the ipv4 to see the scope, filters, policies and other information about the configured DHCP scope. <br/>
<img src="https://imgur.com/ZRKddEa.png" height="80%" width="80%" alt="View configured DHCP scope."/>
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
