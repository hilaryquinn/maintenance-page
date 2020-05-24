# maintenance-page
HTML5/CSS3 Maintenance Page Template - Responsive

A HTML/CSS maintenance page template for you to use on you and/or your clients projects.
You may not resell this template. This template is given to you free of charge.
You may modify this template as you see fit.
If you choose to use the image included with this template then please leave the copyright notice accompanying it.
You have permission to use this image with the maintenance page template only, and not on other design projects or to re-sell. 
Image copyright is held by Hilary Quinn.

* HTML5 / CSS3
* Content Security Policy meta tags
* Flex based responsive layout
* Gradient background
* Google Fonts and Font Awesome included

Create a folder called maintenance on your web server to serve these files, this prevents complication with your existing code. Insert your analytics code into analytics_maintenance.js. Edit the .htaccess below to include your own domain.

-------- To re-direct all pages to your maintenance page, insert the code below into your .htaccess file --------

<IfModule mod_rewrite.c>
  
    RewriteEngine On
    RewriteCond %{REQUEST_URI} !/maintenance/index\.html$ [NC]
    RewriteCond %{REQUEST_URI} !\.(jpg|jpeg|png|gif|css|ico)$ [NC]
    RewriteRule ^(.*)$ http://www.mydomain.com/maintenance/index.html [R=302,L]
    
</IfModule>

------------------------------------------------------------------------------------------------------------

-------- Replace ip number below with your own for self access, insert the code below into your .htaccess file --------

<IfModule mod_rewrite.c>
  
    RewriteEngine On
    RewriteCond %{REMOTE_ADDR} !=00.000.000.0
    RewriteCond %{REQUEST_URI} !/maintenance/index\.html$ [NC]
    RewriteCond %{REQUEST_URI} !\.(jpg|jpeg|png|gif|css|ico)$ [NC]
    RewriteRule ^(.*)$ http://www.mydomain.com/maintenance/index.html [R=302,L]
    
</IfModule>

------------------------------------------------------------------------------------------------------------

Hope you find it useful!

[Mobile screenshot](maintenance-page_iphone_x.png) 

[Desktop screenshot](maintenance-page_desktop.png)
