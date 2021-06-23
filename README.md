# ansible-ise
---------------------------
Requirements:
---------------------------
-ISE ERS Enabled
-Correct/Updated group id strings from respective ISE node/cluster
-Proper variable usage/input
-Updated ISE ERS username/pass & urls

get_ise_endpoint_details.yml : Gets an existing Endpoint group assignment name from ISE
---------------------------
Playbook overview:
-Get existing MAC endpoint ID string from ISE db
-Print returned data from ISE
-Extract endpoint id string using json_query & store as variable
-Extract the id string from nested list & store as variable
-Get endpoint details from ISE using endpoint id string
-Print returned data from ISE
-Extract endpoint group id string using json_query & store as variable
-Extract the group id string from nested list & store as variable
-Print returned group name to screen

ise_endpoint_group_update.yml : Updates an existing Endpoint group assignment based on user variables
---------------------------
Playbook overview:
-Create variable based on user input conditional
-Get existing MAC endpoint ID string from ISE db
-Print returned data from ISE
-Extract endpoint id string using json_query & store as variable
-Extract the id string from nested list & store as variable
-Print endpoint ID
-Update Endpoint group assignment in ISE
-Get updated Endpoint details from ISE
-Extract endpoint group id string using json_query & store as variable
-Extract the group id string from nested list & store as variable
-Get Endpoint Updated group name from ISE
-Print group name
-Extract group name from nested list & store as variable
-Print updated Endpoint group name from ISE

