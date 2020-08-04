.. title:: Calm and Karbon 101

.. toctree::
  :maxdepth: 2
  :caption: Calm 101
  :name: _calm
  :hidden:

  calm_enable_projects/calm_enable_projects
  calm_marketplace/calm_marketplace
  calm_windows_blueprint/calm_windows_blueprint
  
 
.. toctree::
  :maxdepth: 2
  :caption: Karbon 101
  :name: _Karbon
  :hidden:
  
  karbon_enable/karbon_enable
  karbon_deploy_vm /karbon_deploy_vm
  karbon_create_cluster/karbon_create_cluster
  karbon_deploy_application/karbon_deploy_application
  karbon_delete_application/karbon_delete_application


.. _getting_started:

Getting Started
===============

.. raw:: html

  <strong><font color="red">Do not start any labs before being told to do so by your
  instructor.</font></strong><br><br>

Welcome to Nutanix Calm and Karbon bootcamp! 


Cluster Access
++++++++++++++

The Nutanix Hosted POC environment can only be accessed via VPN or virtual desktop. **It is recommended that the VPN be used to complete these labs.**

Virtual Desktop Access
.......................
  
| 20 x VDI/VPN User Accounts: PHX-POC0XX-User01, PHX-POC0XX-User02 … PHX-POC0XX-User20 etc.
| VDI/VPN User Password: *To be provided by your lab instructor*
| XX is your cluster ID

**Parallels VDI**

1. Login to https://xld-uswest1.nutanix.com (for PHX) or https://xld-useast1.nutanix.com (for RTP) using your supplied credentials
2. Select HTML5 (web browser) OR Install the Parallels Client
3. Select a desktop or application of your choice.
  
**Frame VDI**

1. Login to https://frame.nutanix.com/x/labs using your supplied credentials
2. Select the most applicable datacenter launchpad for the clusters you will be accessing or modify an existing selection using the breadcrumb menu at the top-center of the page
3. Launch desktop

**Pulse Secure VPN Client**

1. If client already installed skip to step 5
2. To download the client, login to https://xlv-uswest1.nutanix.com or https://xlv-useast1.nutanix.com using the supplied user credentials
3. Download and install client
4. Logout of the Web UI
5. Open client and ADD a connection with the following details:

  |  Type: Policy Secure (UAC) or Connection Server(VPN)
  |  Name: X-Labs - PHX
  |  Server URL: xlv-uswest1.nutanix.com

  **OR**

  |  Type: Policy Secure (UAC) or Connection Server(VPN)
  |  Name: X-Labs - RTP
  |  Server URL: xlv-useast1.nutanix.com

6. Once setup, login with the supplied credentials

