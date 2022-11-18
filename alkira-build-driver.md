# Prerequisites

- Install Python 2.7
https://www.python.org/downloads/

- Download EWDK 
https://learn.microsoft.com/en-us/windows-hardware/drivers/other-wdk-downloads?source=recommendations

Step 1:

![Screenshot_1](https://user-images.githubusercontent.com/103962345/202692050-797b6809-1f77-4ee4-bd52-7824c1ef731d.png)

Step 2:

![Screenshot_2](https://user-images.githubusercontent.com/103962345/202692065-01483a29-f606-4805-a2db-e7244c89da43.png)

The file must be named **EWDK_vb_release_svc_prod1_19041_201201-2105.iso**

# Prepare environment
- Mount or extract iso file
- Edit file **paths.py** in repository, set path to iso file content, fo example ``EWDK = "E:"``

# Build

Open cmd at root repository dir and run command

``python.exe buildtap.py --sdk=ewdk -b``

Result of successfully build

![image](https://user-images.githubusercontent.com/103962345/202693412-1bcb567d-a94e-44c3-8c19-83d842b1bfab.png)

You can find drivers at **dist** folder

![image](https://user-images.githubusercontent.com/103962345/202693744-5b2ef760-71ba-43dd-9419-12f1aacd3e91.png)
