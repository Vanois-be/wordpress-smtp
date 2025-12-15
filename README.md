# wordpress-smtp
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
