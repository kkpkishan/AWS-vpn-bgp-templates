# AWS-VPN-BGP CloudFormation Templates
<table>
    <tr>
        <th align="left" colspan="2"><h4><a href="https://github.com/kkpkishan/aws-vpn-bgp-cf.git">VPN BGP (Virtual Private Network using Border Gateway Protocol)</a></h4></th>
    </tr>
    <tr>
        <td valign="top">
            <p>Creates a Site-to-Site BGP VPN Connection in and existing VPC with public and/or private networks.
             There is an option to not exclude allowing VPN access to the public networks.
             Simply select false for the 'Include Public Subnets', leave default value in Public Network ACL and Route Table.
             The values will just be ignored. This only sets up the AWS side of the VPN.
             </p>
             <h6>Prerequisites</h6>
             <ol>
                <li>VPC</li>
                <ul>
                  <li>Public Subnet, IGW, Private Subnet/s.</li>
                  <li>Either use an existing VPC Infrastructure or you can use the following <a href="https://github.com/kkpkishan/aws-vpc-cloudformation-Templates.git" target="_blank">VPC Template</a> to create a one.</li>
                </ul>
              <li>Remote Network (Office) VPN Device WAN IP</li>
              <li>Remote Network CIDR Block to Allow Access and Propagate.</li>
             </ol>
            <h6>Create Details</h6>
            <ol>
             <li>Customer Gateway</li>
             <li>Virtual Private Gateway</li>
             <li>VPN Connection</li>
             <li>Enable Route Propagation on Route Table/s</li>
             <li>Add Network ACL to Allow Remote Network</li>
            </ol>
        </td>

