USE taulu;

CREATE TABLE IF NOT EXISTS `Shortening` (
`id` int(11) NOT NULL,
`url` varchar(1000) NOT NULL,
`osio` varchar(15) NOT NULL,
`ip` varchar(25) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;


ALTER TABLE `Shortening`
ADD PRIMARY KEY (`id`), ADD UNIQUE KEY `osio` (`osio`);

ALTER TABLE `Shortening`
MODIFY `id` int(11) NOT NULL AUTO_INCREMENT;
