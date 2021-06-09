# craftivity-cloud
Create a project and manage project member accounts:
1. Create a project.
2. Set up an account for our team to access the project.

Using Cloud Storage Bucket:
1. Create 2 buckets in Cloud Storage, the first bucket to store the photo files that will be used and the second bucket to store the sql files that have been created in phpmyadmin.
2. Create 5 folders of types of waste (cardboard, glass, metal, paper, plastic) and upload photo files based on the type of waste.
3. Upload the sql file in the second bucket.
4. Editing bucket permissions. In the Access control section, click on the switch to fine-grained.
5. Edit the permissions on each file by adding an entry.
- Entity : Public
- Name : allUsers
- Access : Reader.

Using CloudSQL:
1. Create an instance on Cloud SQL, using mysql with the following specifications:
- Region : asia-southeast2 and check the Multiples Zone
- Machine Type : Shared core and tick 1 vCPU, 0.614 GB or db-f1-micro
- Storage Type: SSD
- Storage Capacity: 10 GB
- Connectivity: select Public IP.
2. After successfully created, identify the public ip connectivity with 0.0.0.0/0.
3. Import the sql file into the created instance.
