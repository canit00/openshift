## OpenShift

This is where I store commands to manage OpenShift or related.

How to login to the intergrated docker registry
>docker login -u admin -e first.last@email.com -p $(oc whoami -t) ip_address:5000

Give user privileges to create new projects
>oadm policy add-cluster-role-to-user self-provisioner username

Warnings:
  * dc/autoscaling has no readiness probe to verify pods are ready to accept traffic or ensure deployment is successful.
    try: oc set probe dc/autoscaling --readiness ...
  * dc/eaptest has no readiness probe to verify pods are ready to accept traffic or ensure deployment is successful.
    try: oc set probe dc/eaptest --readiness ...

View details with 'oc describe <resource>/<name>' or list everything with 'oc get all'.
