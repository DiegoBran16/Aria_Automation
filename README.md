# Aria_Automation

## Cloud-Init setup for Red Hat distributions 

**Step 1** Instal the clou-init package 

`yum cloud-init`

**Step 2** Comment all the lines except the ones related to the cloud init modules in the cloud.cfg file


**Step 3** Create the 90_dpkg.cfg file with the folowwing content 

`datasource_list: [ Nocloud, ConfigDrive, OpenNebula, DigitalOcean, Azure, AltCloud, OVF, MAAS, GCE, OpenStack, CloudSigma, SmartOS, Bigstep,Scaleway, AliYun, Ec2, CloudStack, Hetzner, IBMCloud, Oracle, Exoscale, Rbxcloud, Upcloud, VMware, vultr, LXD, NWCS, None ]`

