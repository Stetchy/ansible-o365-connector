# Ansible O365 Connector

This is a simple way to send cards to Office 365 connectors (MS Teams, Outlook).


## About
This was created to be used within a Jenkins pipeline for sending production deployment approval requests to MS Teams channel's where people with the correct authorisation could approve/deny a release to production.
It's intended to work alongside the Jenkins pipeline input step plugin by using the card actions to post to the endpoint in Jenkins.

## Usage

In the [templates](roles/post-to-connector/templates) directory, there's a sample Card that can be used with the playbook, but you can add your own templates, variables etc by extending the playbook.

## Variables

**o365_connector_url**: The webhook URL that was created when setting up your connector.

**o365_card**: The name of your card template file (without json file extension).




