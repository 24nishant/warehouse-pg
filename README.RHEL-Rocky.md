## For RHEL/Rocky8

- Install dependencies using README.RHEL-Rocky.bash script.

   ```bash
   ./README.RHEL-Rocky.bash
   ```

  Refer to this link for the detailed system requirements: 

  https://warehouse-pg.io/docs/7x/install_guide/platform-requirements.html


  You need to create a gpadmin user to administer WarehousePG. Refer to this link on how to create a `gpadmin` user and setup ssh keys:

  https://warehouse-pg.io/docs/7x/install_guide/config_os.html#creating-the-warehousepg-administrative-user 

  Make sure you are able to ssh to the host without any password. To achieve that you can run this: 

  ```bash
   ssh-keygen -A
   cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
   chmod 600 ~/.ssh/authorized_keys
  ```

 Set up your system configuration by following the installation guide on [warehousepg.org](https://warehouse-pg.io/docs/7x/)
