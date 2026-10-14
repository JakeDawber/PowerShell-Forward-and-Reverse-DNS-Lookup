<h1>PowerShell Forward and Reverse DNS Lookup</h1>


<h2>Process</h2>

Testing that the DNS server can resolve my domain controller's hostname to its IPv4 address.

<img src="Screenshots/DNS service verification.png"/>

Active Directory DNS health: Used dcdiag to verify Active Directory DNS health and from the output, we can see that the Windows server JH-dc01 successfully passes both the connectivity test and the DNS test. We can also see that the domain jakehomelab.test successfully passed the DNS test.

<img src="Screenshots/AD health.png"/>
