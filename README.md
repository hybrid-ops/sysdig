# Sysdig SDK integration for CP4MCM 1.3


    spoke with Brett and Alvero on zoom. The integration is mainly two steps
    deploy the agent, make sure we can see the cluster in secure.
    enable service id , so sysdig can detect events in our cluster.
    sysdig integration team has scripts and tools that we can use to generate the events, that would trigger the events monitored by sysdig.


    deploy the kube/ocp sysdig agent ( manually | helm chart ) using the api key associated to your account above.
    create a service api key off of the existing service id grafeas-admin-service-id in Foundation IAM, and convey to SYSDIG team.

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









