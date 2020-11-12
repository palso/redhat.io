# Get started with ownCloud

## Introduction

ownCloud is a flexible open source file synchronization and sharing solution. As a user you can access the ownCloud server, client application for MS Windows, Mac OS X and Linux and mobile clients for Android and iOS.
This guide helps users to quickly install an ownCloud server and configure it from a client, add user and connect ownCloud server using mobile client. 
For detailed documentation of ownCloud,  refer to [ownCloud documentations](doc.ownCloud.com).

## Installing an ownCloud server

### System requirements

| Platform         | Options                                                      |
| ---------------- | ------------------------------------------------------------ |
| Operating System | Ubuntu 18.04 LTS                                             |
| Database         | MariaDB 10+                                                  |
| Web server       | Apache 2.4 with [`prefork and mod_php`](https://doc.owncloud.com/server/10.5/admin_manual/installation/manual_installation.html#multi-processing-module-mpm) |
| PHP Runtime      | 7.4                                                          |

**NOTE**: For more information on supported environments, deployment considerations and recommendations, Server, Hypervisors, Web Browsers, Desktop Sync Client, Mobile Apps, Database, and Memory, refer to [ownCloud Admin Guide](doc.ownCloud.com).

There are two installation options for ownCloud:

- Installing with Docker
- Installing manually

### Installing with Docker

1. Get *the official ownCloud docker* image.
2. Run the image on the client.
3. Evaluate the file with `docker run -p8080:8080 ownCloud/server`.
4. Expose ports `8080`and allow HTTP connections.
5. Mount the MySQL data directories on the host for persistent storage. 

For detail installation information on Installing with Docker and enable users to connect to the ownCloud server using the server's IP address and port 8080, refer to [ownCloud Admin Guide](doc.ownCloud.com)

### Installing manually

1. Install the required packages - These are stable distrbutions channels which are not updated immediately post release.
2. Install ownCloud (Refer the[ownCloud Admin Guide](doc.ownCloud.com) ).
3. Configure the Web Server.
4. Run the installation wizard.
5. Set the directory permissions.
6. Manage the trusted domains by whitelisting the URLs you use.

## Adding a user in ownCloud

You can add users or group to your ownCloud installation with the help of UCS (Univention Corporate Server) UI. 
Refer to the *Adding Users and Groups in UCS for ownCloud* in [ownCloud Admin Guide](doc.ownCloud.com)

## Connecting to the ownCloud server with desktop

The *ownCloud Desktop Sync* connects to the ownCloud server from your Windows, Mac OS, Linux desktop clients. You can specify one or more directories in the sync client on your computer to synchronize with the ownCloud server. For details on how to configure the *ownCloud Desktop Sync* , refer to [ownCloud Desktop Client Guide](doc.ownCloud.com). Users can also access the ownCloud server from the *ownCloud WebUI*. For more details, refer to [ownCloud User Guide](doc.ownCloud.com)

## Connecting to the ownCloud server with mobile

ownCloud provides individual applications for Android and iOS mobile phones. 
The ownCloud Android/ iOs app offers some advantages over the Web interface:

- A simplified interface that fits nicely on a tablet or smartphone
- Automatic synchronization of your files
- Share files with other ownCloud users and groups, and create multiple public share links
- Upload of photos and videos recorded on your Android device
- Easily add files from your device to ownCloud
- Two-factor authentication or an optional PIN for stronger security

For more details on how to configure the Android or iOS apps, refer to [ownCloud Android/iOS App Guide](
