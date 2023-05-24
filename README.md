# Automated CI Project for Maven built Using Jenkins Server

### Overview:
A maven project that automatically triggers a remote Jenkins server when changes are pushed to github.

### Steps Followed:
* Create an Ubuntu EC2 instance on AWS
* Connect to the virtual cloud machine via SSH, and install required dependencies
* Install and run jenkins server on a virtual cloud machine
* Activate github webhooks for automated build triggering
* Creating the automated pipeline for Continuous Integration
* Testing the pipeline via a test push/commit
