# Nginx Web Server

## Project Overview
This README provides an overview of the three main criteria involved in the project, which includes setting up a web server, configuring NGINX as a reverse proxy server, and implementing access limits on NGINX for enhanced security.

## Table of Contents
- [Nginx Web Server](#nginx-web-server)
  - [Project Overview](#project-overview)
  - [Table of Contents](#table-of-contents)
  - [Project Criteria](#project-criteria)
    - [Criterion 1: Setting up the Web Server](#criterion-1-setting-up-the-web-server)
    - [Criterion 2: Configure NGINX as a Reverse Proxy Server](#criterion-2-configure-nginx-as-a-reverse-proxy-server)
    - [Criterion 3: Implement Access Limits on NGINX](#criterion-3-implement-access-limits-on-nginx)
  - [Tips and Configuration Changes](#tips-and-configuration-changes)


## Project Criteria
The project comprises the following key criteria:

### Criterion 1: Setting up the Web Server
Begin by making necessary preparations for setting up the web server. This involves the following steps:
1. Clone the GitHub repository provided by Dicoding at https://github.com/dicodingacademy/a387-jarkom-labs.git.
2. Install NGINX.
3. Ensure proper accessibility for both Node.js and NGINX web servers.

### Criterion 2: Configure NGINX as a Reverse Proxy Server
Following the successful completion of Criterion 1, proceed to configure NGINX as a reverse proxy server. This step enables requests to be forwarded to the web server when accessed via port 80, the port used by NGINX.

### Criterion 3: Implement Access Limits on NGINX
After completing Criterion 2, continue by implementing access limits on NGINX, effectively functioning as a reverse proxy server. This step is crucial for applying access or rate limits, thus enhancing security on the web server.


## Tips and Configuration Changes
Here are some additional tips and configuration changes to consider:
1. Ensure Node.js and NPM are installed, preferably using NVM, with a minimum version of Node.js v14.15.4.
2. Adjust NGINX to listen on port 3000 instead of the default port 80.
3. Modify NGINX rate limit settings to allow 6 requests per minute (1 request every 10 seconds).
4. Update the Node.js web server response from "Hello world!" to a full name.
5. If encountering issues with systemctl, use the "service" command. For example, to check NGINX's status, run `sudo service nginx status`.
6. If Apache2 was previously installed and issues arise, stop the Apache2 service using `sudo service apache2 stop`. If issues persist, remove Apache2 with `sudo apt remove apache2`.
7. If necessary, navigate back to the previous folder in the console or terminal using the "cd .." command.
8. To copy the contents of a file in the Ubuntu console or terminal to a notepad, use the `cat <file_location>` command to display the file's content, then select the text, copy it with CTRL+C, and paste it into Notepad with CTRL+V.
9. When creating a new configuration, activate the local server in NGINX as described [here](https://stackoverflow.com/questions/68576682/nginx-this-site-can-t-be-reached).