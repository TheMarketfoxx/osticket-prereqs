<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
- ## This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>How osTicket works for you</h2>

- ## Users create tickets via your website, email, or phone
- ## Incoming tickets are saved and assigned to agents
- ## Agents help your users resolve their issues
- ## osTicket is an attractive alternative to higher-cost and complex customer support systems; simple, lightweight, reliable, open source, web-based and easy to setup and use. The best part is, it's completely free.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

HTTP server running Microsoft® IIS or Apache
PHP version 8.1 - 8.2 (8.2 recommended)
mysqli extension for PHP
MySQL database version 5.5 (or greater)
<h2>Installation Steps</h2>

<p>
</p>
<p>
osTicket now supports bleeding-edge installations. The easiest way to install the software and track updates is to clone the public repository. Create a folder on you web server (using whatever method makes sense for you) and cd into it. Then clone the repository (the folder must be empty!):

git clone https://github.com/osTicket/osTicket
And deploy the code into somewhere in your server's www root folder, for instance

cd osTicket
php manage.php deploy --setup /var/www/htdocs/osticket/
Then you can configure your server if necessary to serve that folder, and visit the page and install osTicket as usual. Go ahead and even delete setup/ folder out of the deployment location when you’re finished. Then, later, you can fetch updates and deploy them (from the folder where you cloned the git repo into)

git pull
php manage.php deploy -v /var/www/htdocs/osticket/
