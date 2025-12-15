# Wordpress smtp and Microsoft 365 plugin
Use the customer's SMTP server or Microsoft 365 server for sending mail securely.

# How to use?

Constants are defined in wp-config.php

	// Server
	define( 'SMTP_HOST',     	'mail.infomaniak.com' );
	define( 'SMTP_PORT',     	'465' );
	define( 'SMTP_AUTH',     	true );
	define( 'SMTP_SECURE',   	'ssl' );

	// Authentification
	define( 'SMTP_USER',     	'noreply@website.be' );
	define( 'SMTP_PASSWORD', 	'password' ); 

	// Headers
	define( 'SMTP_FROM',     	'noreply@website.be' );
	define( 'SMTP_FROMNAME', 	'From name' );

	// Optionnal
	define( 'SMTP_REPLYTO',  	'reply@website.be' );
	define( 'SMTP_REPLYTONAME', 'ReplyTo name' );

  If you use Contact Form 7, you can skip these two constant SMTP_REPLYTO, SMTP_REPLYTONAME as you can define the paramter "Reply-To: my@email.com" in the "Header" field of the email template.

  Once constants are defined in you wp-config.php file, upload the plugin, activate it, go to Settings > Vanois SMTP. 
  There you can :
  - test your configuration by sending a test email
  - configure Microsoft 365 : via Microsoft 365 OAuth 2.0 authentication functionality. Follow the guided setup wizard.


# Disclaimer

All files, scripts, including WordPress themes and plugins is covered by this disclaimer:

While I make every effort to deliver high quality products, I do not guarantee that my files are free from defects. All files, scripts, assets are provided “AS IS,” and you use them at your own risk. I make no warranties as to performance, merchantability, fitness for a particular purpose, or any other warranties whether expressed or implied. No oral or written communication from me or information provided by me shall create a warranty. Under no circumstances shall I be liable for direct, indirect, special, incidental, or consequential damages resulting from the use, misuse, or inability to use theses files, scripts, assets, even if I has been advised of the possibility of such damages. These exclusions and limitations may not apply in all jurisdictions. You may have additional rights and some of these limitations may not apply to you. NOTE: I do not offer support for any files, script, themes, and plugin being offered on this github.

