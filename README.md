# Sysdig SDK integration for CP4MCM 1.3

## Pre-reqs

- Create a sysdig SAAS account https://sysdig.com/sign-up/

- Verify login to sysdig SECURE SAAS:

   https://secure.sysdig.com/#/login

- Verify login to sysdig MONITOR SAAS:

   https://app.sysdigcloud.com/#/login
   

## Deploy the sysdig agent

Currently the sysdig secure and monitor agent have the same steps. 

1. Log into hub cluster via `oc login` or `cloudctl login`

2. Run `create-agent.sh` which will create the agent in secure mode. 

3. Log into the SECURE SAAS and verify the cluster is in the view.


## Enable the service ID

This needs to be done so that sysdig can detect events in the cluster

1. Create a service api key off of the existing service id grafeas-admin-service-id in Foundation IAM

TODO





