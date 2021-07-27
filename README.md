# php-url-shortener
A URL shortener using PHP, for things like News Articles etc

A short PHP script to automatically generate smaller URL's once submitted.

Generate a database named "url_shorten" to start and add the following tables

CREATE TABLE IF NOT EXISTS `url_shorten` (
  `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `url` tinytext NOT NULL,
  `short_code` varchar(50) NOT NULL,
  `hits` int(11) NOT NULL,
  `added_date` timestamp NULL DEFAULT CURRENT_TIMESTAMP
) ENGINE = InnoDB AUTO_INCREMENT = 1 DEFAULT CHARSET = latin1;
