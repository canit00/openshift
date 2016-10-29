## OpenShift

This is where I store commands to manage OpenShift or related.

How to login to the intergrated docker registry
>docker login -u admin -e first.last@email.com -p $(oc whoami -t) <ip_address>:5000

Give user privileges to create new projects
>oadm policy add-cluster-role-to-user self-provisioner <username>
