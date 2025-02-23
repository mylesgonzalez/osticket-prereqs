<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Installation Walkthrough </h1>
This tutorial will guide you through the osTicket installation process and help you configure the necessary prerequisites.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Internet Information Services
- PHP
- MySQL
- Microsoft Visual C++
- HeidiSQL

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/ZYigv69.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To get started with installing osTicket you're going to need Internet Information Services(IIS), so that we can host the ticketing webpage and store the required data for that page to operate on a database. IIS can be located on the program page of the control panel and from there you can locate the tab that specifies adding or removing window features. From there you can install IIS and CGI which are both required for the web server to operate.
</p>
<br />

<p>
<img src="https://i.imgur.com/zG4ByMS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next we’re going to need PHP which acts as a server side scripting language that allows websites to interact with databases and generate custom web content such as user profiles. Essentially PHP(Hypertext Preprocessor) runs on the server in the background and will output information to the webpage for the user to interact with. Installing php is relatively simple as you just have to follow the steps located on https://www.php.net/downloads. After installation, it is imperative to register the PHP from within the IIS. 
</p>
<br />

<p>
<img src="https://i.imgur.com/8BihBk9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After installing PHP and registering it into IIS, we can now begin the installation of MySQL. MySQL will house the database that will store all the information needed for the ticketing service to operate, such as agents, administrators, and user accounts. MySQL requires Microsoft Visual C++ to operate, which can be installed here (MVC++). Lastly, the official MySQL download page can be found here: https://dev.mysql.com/downloads/installer/. Make sure when going through your standard installation procedure to write down your root password so that you won't lose access to the server that will manage all the information within the database.
</p>
<br />

<p>
<img src="https://i.imgur.com/VCi5CBz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lastly, we are going to need to install HeidiSQL, which will be used to interact with and manage our databases created in SQL. Once you have installed HeidiSQL and launched the software, you will need to type in the account details for the admin account you created when making a server in MySQL so that HeidiSQL has the permissions to manage the data held by the database on MySQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/WklFTBi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we have all the prerequisites installed, we can type the server domain in any browser and open the osTicket startup page. From there, you'll see that we will need to enable some extensions, which can be done through IIS. Simply locate the osTicket database in IIS, click on PHP Manager, and enable the extensions required for osTicket to run properly.
</p>
<br />
