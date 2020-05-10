# GoogleDriveMount
- GoogleDrive is Mounted as the local file system.
-  Google API is used in the application.It provides features to use google products in our application, Rather than creating newone.For similar reason here we have used GoogleDrive API.
- The first step is authentication, once authentication is done it returns a token that is used to access GoogleDrive again        without furthur authentication.
- Oauth2 is used for authentication.
- The second step includes- 
  - creating a mountpoint, and
  - libfuse library is used to create a temporary image of our google drive.
- various functionalities Supported(### Only linux supported commands)
  - listing and viewing files.(ls command)
  - create a directory.(mkdir)
  - renaming a file/folder.(mv command)
  - moving a file.(uploading in the drive)
  - deleting a file/folder.
- Synchronisation between local enviroment and remote GoogleDrive
  - All those functionalities mentioned above are synchronised with google drive, any operation carried out in local drive willbe reflected in googleDrive and vice-versa.
   
### NOTE
- only when ls command is used than only downloading of files from googledrive is performed, In this way unnecessary files are  not downloaded and memory is saved.
- Application is supported only in Linux Flavours. Ex- Ubuntu, kali etc.
- after running application in terminal, only standard commands of terminal gives desired result.
- any operations performed using GUI in local mountpoint willnot be reflected in google drive. Only commands through terminal are synchronised.
#### Technologies
- python3
- Ubuntu OS
