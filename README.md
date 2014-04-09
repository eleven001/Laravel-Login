Laravel-Login
=============

A basic membership system made with Laravel. Functionalities include Sign In, Sign Out, Forgot password, Sign Up, and Email activation. The design is responsive and made with Bootstrap v3.1.1.

Configure
=========

To configure you need to open:

- app/config/database.php
- app/config/mail.php

Also, install a users table of this kind:

```
CREATE TABLE `users` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `email` varchar(50) NOT NULL,
  `name` varchar(50) NOT NULL,
  `password` varchar(60) NOT NULL,
  `password_temp` varchar(60) NOT NULL,
  `code` varchar(60) NOT NULL,
  `active` int(11) NOT NULL,
  `created_at` datetime NOT NULL,
  `updated_at` datetime NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=latin1 AUTO_INCREMENT=1 ;
```

And you will be good to go.
