.. _karbon_enable:

-----------------------
Enable Karbon and Upload Image
-----------------------

Overview
++++++++

.. note::

  Estimated time to complete: 20 Minutes

In this lab we will enable Karbon and then we will prepare network for Karbon.

Enable Karbon (Optional-If Karbon is not Enabled)
+++++++++++++

#. Navigate to **Administrator** -> **LCM** to see current Karbon version, if it is not 2.1.0, upgrade to the latest version. (Optional)

   .. image:: images/karbon_deploy_cvm_8.png

#. Navigate to **Service** -> **Karbon**

   .. image:: images/karbon_deploy_cvm_2.png

#. Click **Enable Carbon**

   .. image:: images/karbon_deploy_cvm_3.png

#. Upon enabling Karbon, launch the console

   .. image:: images/karbon_deploy_cvm_4.png

#. To download host OS image, click **Download CenOS**

   .. image:: images/karbon_deploy_cvm_5.png

#. Wait until you see the status changed to downloaded

   .. image:: images/karbon_deploy_cvm_6.png


NTP and Network for Karbon
++++++++++++++++++++++++++
#. Karbon authentication is time sensetive; make sure NTP is configured correctly.

#. Navigate to **Prism Central Settings** -> **NTP Servers**.

#. Verify that NTP Servers is already configured.

#. Else, Key in *0.pool.ntp.org* and click **+Add**.

   .. image:: images/karbon_enable_9.png

#. Open \https://*<POCxx-ABC Cluster IP>*:9440 (\https://10.42.xx.37:9440) in your browser and log in with the following credentials:

   - **Username** - admin
   - **Password** - Provided in Lab details

#. Karbon Deployment required Network Interface with Nutanix IPAM enable.

#. In **Prism > Settings > Network Configuration**, Click on The Edit Button under **Network-01**.

#. Verify that IPAM is enabled for **Network-01**.

   .. image:: images/karbon_enable_ipam.png

#. Click **Cancel**.
















