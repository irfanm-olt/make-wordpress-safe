Things to make wordpress secure
-------------------------------

1) Install a wordpress security plugin - Sucuri.net
2) Use strong password
3) Disable file editing
	- Add define(‘DISALLOW_FILE_EDIT’, true); in wp-config.php
4) Install SSL Certificat
5) Change your WP-login URL
	-  2-factor authentication plugin 
6) Limit Login Attempts
	- limit-login-attempts-reloaded
7) Hide wp-config.php and .htaccess files
	- 	<Files wp-config.php>
			order allow,deny
			deny from all
		</Files>
	- Add this to wp-config.php

	<Files .htaccess>
		order allow,deny
		deny from all
	</Files>

	- Add this to .htaccess