# fortinet-scenario
A scenario that use service component and composition of 3 tier application, fortigate firewall on openstack (+ network) and port-forwarding configuration on top, to create a secured access to the webserver (private shop app)



*** this scenario is designed for cloudify version 5 and above ***

requires the below secrets created on the manager (masked values for privacy)-

=====================================================================OPENSTACK
cfy secrets create external_network_name -s XXXXXXXX
cfy secrets create keystone_password -s xxxxxxxxxx
cfy secrets create keystone_region -s RegionOne
cfy secrets create keystone_tenant_name -s xxxxxxxxxxx
cfy secrets create keystone_url -s https://xxxxxx:5000/v3
cfy secrets create keystone_username -s xxxxxxx
cfy secrets create centos_image_id -s xxxxxxxxxxx
cfy secrets create centos_flavor_id -s xxxxx
cfy secrets create small_image_flavor -s 3
