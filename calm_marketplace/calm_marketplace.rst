.. _calm_marketplace:

-----------------
Marketplace
-----------------

Overview
++++++++


  Estimated time to complete: **35 MINUTES**

  In this exercise you will learn how to manage Calm Blueprints within the Nutanix Marketplace. As part of the exercise you will publish a pre-configured Blueprint to the local Marketplace, clone the Blueprint from the Marketplace for editing, and launch the application.


Calm Marketplace 
+++++++++++++++++


Publishing Blueprints from Marketplace Manager
..............................................

By default, Calm comes pre-seeded with validated Blueprints for multiple open source and enterprise applications. Marketplace Manager acts as a staging area for publishing default and user-created Blueprints to your local Marketplace. The Marketplace acts as an application store, providing end users with a catalog of available applications.

#. From **Prism Central > Apps**, select **Marketplace Manager** from the sidebar.

#. Under **Marketplace Blueprints**, on the top right conner search for *MongoDB Single Node* select **MongoDB Single Node**.

   .. figure:: images/marketplace_p1_mongo.png

   .. note::
   The Blueprint description contains key information including licensing, hardware requirements, OS, supported platforms, and limitations.

#. Select the **Default** project from the right-hand side drop down and Click **Apply** and then click **Publish**.

   .. figure:: images/marketplace_p1_1.png

   Wait for the Blueprint **Status** to appear as **Published**.


Cloning Blueprints from Marketplace
...................................

#. From **Prism Central > Apps**, select **Marketplace** from the sidebar. All Blueprints published in Marketplace Manager are visible here.

#. Select the **MongoDB Single Node** Blueprint and click **Clone**.

   .. note::

     Selecting **Actions Included** for a Blueprint will display the actions that have been implemented for a given Blueprint, such as Create, Start, Stop, Delete, Update, Scale Up, Scale Down, etc.

   .. figure:: images/marketplace_p1_5.png

#. Fill out the following fields and click **Clone**:

   - **Blueprint Name** - *<INITIALS>*-MongoDB
  - **Project** - Default

Editing Cloned Blueprint
........................

#. Navigate to **Virtual Infrastructure** click **Images**, click **Add Images**. Select **URL** as Image resource, fill out download address *https://s3.amazonaws.com/get-ahv-images/CentOS7.qcow2* and click **Upload file**, **Next** and **Save**.

   .. figure:: images/marketplace_p1_51.png

#. After uploading successfully, go back to Calm page and select **Blueprints** from the sidebar and click your **<INITIALS>-MongoDB** Blueprint to open the Blueprint Editor.

   .. figure:: images/marketplace_p1_6.png

#. Click :fa:`exclamation-circle` to review the list of errors that would prevent a successful deployment of the Blueprint.

   .. figure:: images/marketplace_p1_7.png

#. Click **Credentials** and select **CENTOS (Default)**.

#. Fill out the following fields and click **Save** and **Back**:

    - **Credential Name** - centos
    - **Secret Type** - ssh private key
    - **Key** - Paste in your own private key, or use:
      ::
        -----BEGIN RSA PRIVATE KEY-----
        MIIEowIBAAKCAQEAii7qFDhVadLx5lULAG/ooCUTA/ATSmXbArs+GdHxbUWd/bNG
        ZCXnaQ2L1mSVVGDxfTbSaTJ3En3tVlMtD2RjZPdhqWESCaoj2kXLYSiNDS9qz3SK
        6h822je/f9O9CzCTrw2XGhnDVwmNraUvO5wmQObCDthTXc72PcBOd6oa4ENsnuY9
        HtiETg29TZXgCYPFXipLBHSZYkBmGgccAeY9dq5ywiywBJLuoSovXkkRJk3cd7Gy
        hCRIwYzqfdgSmiAMYgJLrz/UuLxatPqXts2D8v1xqR9EPNZNzgd4QHK4of1lqsNR
        uz2SxkwqLcXSw0mGcAL8mIwVpzhPzwmENC5OrwIBJQKCAQB++q2WCkCmbtByyrAp
        6ktiukjTL6MGGGhjX/PgYA5IvINX1SvtU0NZnb7FAntiSz7GFrODQyFPQ0jL3bq0
        MrwzRDA6x+cPzMb/7RvBEIGdadfFjbAVaMqfAsul5SpBokKFLxU6lDb2CMdhS67c
        1K2Hv0qKLpHL0vAdEZQ2nFAMWETvVMzl0o1dQmyGzA0GTY8VYdCRsUbwNgvFMvBj
        8T/svzjpASDifa7IXlGaLrXfCH584zt7y+qjJ05O1G0NFslQ9n2wi7F93N8rHxgl
        JDE4OhfyaDyLL1UdBlBpjYPSUbX7D5NExLggWEVFEwx4JRaK6+aDdFDKbSBIidHf
        h45NAoGBANjANRKLBtcxmW4foK5ILTuFkOaowqj+2AIgT1ezCVpErHDFg0bkuvDk
        QVdsAJRX5//luSO30dI0OWWGjgmIUXD7iej0sjAPJjRAv8ai+MYyaLfkdqv1Oj5c
        oDC3KjmSdXTuWSYNvarsW+Uf2v7zlZlWesTnpV6gkZH3tX86iuiZAoGBAKM0mKX0
        EjFkJH65Ym7gIED2CUyuFqq4WsCUD2RakpYZyIBKZGr8MRni3I4z6Hqm+rxVW6Dj
        uFGQe5GhgPvO23UG1Y6nm0VkYgZq81TraZc/oMzignSC95w7OsLaLn6qp32Fje1M
        Ez2Yn0T3dDcu1twY8OoDuvWx5LFMJ3NoRJaHAoGBAJ4rZP+xj17DVElxBo0EPK7k
        7TKygDYhwDjnJSRSN0HfFg0agmQqXucjGuzEbyAkeN1Um9vLU+xrTHqEyIN/Jqxk
        hztKxzfTtBhK7M84p7M5iq+0jfMau8ykdOVHZAB/odHeXLrnbrr/gVQsAKw1NdDC
        kPCNXP/c9JrzB+c4juEVAoGBAJGPxmp/vTL4c5OebIxnCAKWP6VBUnyWliFhdYME
        rECvNkjoZ2ZWjKhijVw8Il+OAjlFNgwJXzP9Z0qJIAMuHa2QeUfhmFKlo4ku9LOF
        2rdUbNJpKD5m+IRsLX1az4W6zLwPVRHp56WjzFJEfGiRjzMBfOxkMSBSjbLjDm3Z
        iUf7AoGBALjvtjapDwlEa5/CFvzOVGFq4L/OJTBEBGx/SA4HUc3TFTtlY2hvTDPZ
        dQr/JBzLBUjCOBVuUuH3uW7hGhW+DnlzrfbfJATaRR8Ht6VU651T+Gbrr8EqNpCP
        gmznERCNf9Kaxl/hlyV5dZBe/2LIK+/jLGNu9EJLoraaCBFshJKF
        -----END RSA PRIVATE KEY-----

      .. figure:: images/centos_credential.png

#. Select the **Mongo** Service and make the following changes in the **VM Tab**:

    - Update the **VM Configuration > Image** to **CentOS7**.
    - Update the **Network Adapters > NIC** to **Network-01**.
    - Update the **Connection > Credential** to **CENTOS**.

#. Expand the **Linux** section.  Copy the **cloud-init** contents into the **Guest Customization**
  
   .. code-block:: bash
   
    #cloud-config
    users:
    - name: centos
      ssh-authorized-keys:
        - @@{centos_public_key}@@
      sudo: ['ALL=(ALL) NOPASSWD:ALL'] 

#. On the left Side Toolbar, Select **Application Profile** and Click on **Nutanix**.

#. Create a variable based on the following:

    - **Name** - centos_public_key
    - **Data Type** - String
    - **Value** - Paste in your own public key, or use:
      ::
        ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAii7qFDhVadLx5lULAG/ooCUTA/ATSmXbArs+GdHxbUWd/bNGZCXnaQ2L1mSVVGDxfTbSaTJ3En3tVlMtD2RjZPdhqWESCaoj2kXLYSiNDS9qz3SK6h822je/f9O9CzCTrw2XGhnDVwmNraUvO5wmQObCDthTXc72PcBOd6oa4ENsnuY9HtiETg29TZXgCYPFXipLBHSZYkBmGgccAeY9dq5ywiywBJLuoSovXkkRJk3cd7GyhCRIwYzqfdgSmiAMYgJLrz/UuLxatPqXts2D8v1xqR9EPNZNzgd4QHK4of1lqsNRuz2SxkwqLcXSw0mGcAL8mIwVpzhPzwmENC5Orw== rsa-key-20190108

      .. figure:: images/centos_pubkey.png

#. Click **Save**.

#. If there is a warning about account UUID , delete AWS,GCP,Azure and VMWare option at the bottom.

   .. figure:: images/marketplace_p1_71.png

#. Clear all errors and click **Launch**. Specify a unique **Application Name** (e.g. <INITIALS>-MongoDBVM01) and click **Create**.

   .. figure:: images/marketplace_p1_8.png


Takeaways
+++++++++

- By using pre-seeded Blueprints from the Nutanix Marketplace, users can quickly try out new applications.
- Marketplace Blueprints can be cloned and modified to suit a user's needs. For example, the pre-seeded LAMP Blueprint could be a starting point for a developer looking to swap PHP for a Go application server.
- Marketplace Blueprints can use local disk images or automatically download associated disk images. Users can create their own keys and slipstream them into Blueprints (via cloud-init) to control access.
- Developers can publish Blueprints to the Marketplace for fast and easy consumption by users.
- Blueprints can be launched directly from the Marketplace with no additional configuration from users, delivering a public cloud-like SaaS experience for end users.
- Administrators have control over what Blueprints are published to the Marketplace and which projects have access to published Blueprints.
