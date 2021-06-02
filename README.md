<H1>README</H1>
<H1>Repo Name: package</H1>
<P>Purpose: To demonstrate how to create an Application EC2 AMI using Packer within a Jenkinsfile. This job is run after each successful build. The Base image was created manually with an Amazon Linux Image and a TOMCAT installation. Packer uses that Base image to create the final Application AMI as part of the pipeline. This allows for a faster AMI build, because the pipeline is not re-creating the same base image (tomcat) after each successful application build</P>

<H1>Before running this repo, update the following items to reflect your repo information and envrionment</H1>

<UL>
<LI>(optional) Update Webhooks on Git Hub to reflect your Jenkins URL or IP
<LI>Update the GIT URL to reflect your own Git Hub Repository
<LI>Verify that the download script download-artifacts.sh is located in /usr/local/bin on the Jenkins EC2 Instance server and that is set to your own Nexus URL or IP (1 location) and credentials
<LI>Update the AMI ID (ami-0ef8f1f9d2093fe56) on ami.json file with your own AMI Tomcat ID (ami-xxxx) you created
</UL>

