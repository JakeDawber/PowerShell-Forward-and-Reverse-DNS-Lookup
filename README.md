<h1>PowerShell Forward and Reverse DNS Lookup</h1>


<h2>Process</h2>

<b>Forward DNS Lookup</b>

Testing that the DNS server can resolve my domain controller's hostname to its IPv4 address.

<img src="Screenshots/PS Forward DNS lookup.png"/>



<b>Configuring a DNS PTR Record (Reverse Lookup)</b>

I configured a Pointer (PTR) record in DNS Manager to enable reverse DNS lookups within my jakehomelab.test domain.

The PTR record maps the server's IP address (192.168.193.10) back to its fully qualified domain name (FQDN), jh-dc01.jakehomelab.test. This allows DNS clients and troubleshooting tools to identify the hostname associated with an IP address.

<img src="Screenshots/PTR record.png"/>


<b>Reverse DNS Lookup</b>

I verified the configuration using PowerShell's Resolve-DnsName cmdlet with the -Type PTR parameter. The query successfully returned jh-dc01.jakehomelab.test, confirming that the reverse lookup record was configured correctly.

<img src="Screenshots/PTR record.png"/>
