# Production Deployments

## Workflow

### Webapp

* Staging release has passed the webapp deployment [checklist](https://stylelounge.atlassian.net/wiki/spaces/PROD/pages/190906369/Checklist+for+Webapp+deployments)
* No downtime  expected
* Message with included features has been posted to deployment-clearance channel
* Deploy and action webapp deployment checklist for production

**Exeception**:

If downtime is expected or the deployment contains a risky feature, the workflow also **has** to include the following steps:

* Outline expected downtime/risk to your PO
* PO sent message to \#marketing that outlined expected downtime/risk
* Agreement whether to turn marketing off in advance or to accept the risk
* Deploy and action webapp deployment checklist for production
* If everything works like intendend, inform marketing to turn marketing on again

Also it should be avoided to have those deployments on the afternoon/evening and especially Friday evenings.

## Incidents

In case a deployment breaks the website, a message has to be sent immediately to incidents-1 outlining what the impact is, what the next steps are and if marketing has to be turned off.

This also requires that we move all uptime checks to incidents-1

