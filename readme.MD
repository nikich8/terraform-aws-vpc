## Aws vpc modules.
# this module create following resources
# vpc 
# IGT with vpc association
# 2 public subnets in 1a @ 1b
# 2 private subnets in 1a @ 1b
# 2 database subnets in 1a @ 1b
# Elastic ip
# nat gate way in 1a public subnet
# public route table
# public route table
# database route table
# subnets &  route table association
# vpc peering if user requests
# Adding the peering route in default vpc,if user don't provide explicitly.
# Adding the peering routes in public ,private and database route tables,

Mandatory things
# Inputs
# Project_Name -Your project name
# Environmern - Which environment your are working.
# vpc_cidr -(optional) -Default value is 10.0.0.0/16, user can override
# Enable_dns_hostname- Default value is true.
# common_tags - Better to provide
# vpc_tags -optional
# igw_tags -optional
# Public_subnet_cidr -user must be provide 2 valid subnets cidr
# Public_subnet_tags (optional)-
# private_subnet_cidr -user must be provide 2 valid subnets cidr
# private_subnet_tags (optional)-
# database_subnet_cidr -user must be provide 2 valid subnets cidr
# database_subnet_tags (optional)-
# nat_gateway_tags -(optional)
# public_route_table_tags -(optional)
# private_route_table_tags -(optional)
# database_route_table_tags -(optional)
# is_peering_required -(optional) default valu is false
# acceptor_vpc_id -optional -default value is default vpc id
# vpc_peering_tags- (optional) default value is empty.type is map
