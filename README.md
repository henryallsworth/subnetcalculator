# Visual Subnet Calculator
[David Croft's Original Site hosting the calculator](http://www.davidc.net/sites/default/subnets/subnets.html)

[David Griffith's Site hosting his fork of the calculator](https://www.subnetcalculator.org/)

---

# Updates
- Forked from George Griffith's [fork](https://github.com/georgewgriffith/subnets) of David Croft's - Visual Subnet Calculator [original repo](https://github.com/davidc/subnets)
- First update is to fix the show/hide function for the table.
    - Modified options in Index.html to remove Divide and Join column checkboxes
    - Modified subnet.js to fix the toggleColumn function, added classes to column create function

# Project Objectives are to expand this tool to support Azure Virtual Network Design needs.  Ideas are as follows
- Virtual Networks and Virtuall Subnets
    - Name each VNET and Subnet
    - Enable Endpoints
        - Define Service Endpoints
        - Define Private Endpoints
    - DDoS
        - Enable
        - Plan ID
    - Tags
    - NSGs
        - Assign only by name and description
        - Maybe a template for default stuff like HTTP, HTTPS, RDP?
        - DMZ concept
    - Route Tables
    - GatewaySubnet
        - Create yes/no
        - Placement preferrence
            - Begining/end
            - Subnet Mask (Default to /27)
    - Define a "DMZ"
        - Pick range and name
        - Define an NSG for standard services inbound/outbound
- Subscription Lookup
    - Signin to Azure Portal
    - Pull list of Subscriptions and GUIDs
- Define Region(s)
- Define Resource Group(s)
- Define DNS settings
    - Define DNS primary, secondary and teritiary servers
- Export Table to Excel file
- Export Table to PNG file
- Export to a JSON template
- Deploy to Azure
    - Depends on Subscription Lookup?
- Export to a Terraform file
- Export to a CLI command list
- Visualize the design using something like armviz.io
- Peering - Define, name, settings
- Host a VPN Gateway?
	- ExpressRoute
	- S2S VPN
	- P2S VPN
- Host a Network Virtual Appliance - Implications thereof?
	- Fortigate
	- Palo Alto
	- Meraki
	- Cisco CSR
	- Baricuda
	- CloudGenix
	- Veeam
	- VeloCloud
- Virtual WAN?