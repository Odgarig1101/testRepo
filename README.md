Ашиглах заавар:

1. Download хийнэ

        Clone https://github.com/Odgarig1101/testRepo.git

2. Visual studtio дээрээ folderoor нь нээнэ :

        file->Open Folder-->lifenote

3. Terminal дээр npm install гэж бичнэ.

        Open Terminal-->npm i

4. My Sql дээр DataBase үүсгэнэ.

       Датабасэээ үүсгэхдээ үүнийг бичихэд болно.

         CREATE DATABASE IF NOT EXISTS `nodelogin` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
         USE `nodelogin`;

         CREATE TABLE IF NOT EXISTS `blogPost` (
         `id` int(11) NOT NULL,
         `title` varchar(50) NOT NULL,
         `desTitle` varchar(50) NOT NULL,
         `description` varchar(255) NOT NULL,
         `blogPhoto` varchar(255) NOT NULL,
         `date` varchar(255),
         `user` varchar(255) NOT NULL,
         `category` varchar(50)
        ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;


        ALTER TABLE `blogPost` ADD PRIMARY KEY (`id`);
        ALTER TABLE `blogPost` MODIFY `id` int(11) NOT NULL AUTO_INCREMENT,AUTO_INCREMENT=2;
        CREATE TABLE IF NOT EXISTS `accounts` (
         `id` int(11) NOT NULL,
         `username` varchar(50) NOT NULL,
         `password` varchar(255) NOT NULL,
         `email` varchar(255) NOT NULL,
         `profilePicture` varchar(255)
        ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;

        ALTER TABLE `accounts` ADD PRIMARY KEY (`id`);
        ALTER TABLE `accounts` MODIFY `id` int(11) NOT NULL AUTO_INCREMENT,AUTO_INCREMENT=2; 

          Бичээд run дарна.
 
5. Visual studio ороод “.env” file үүсгээд доорх кодыг бичнэ. (DB_PASSWORD дээр өөрийнхөө password-ийг хийж өгнө)

        DB_HOST  = 'localhost'
        DB_USERNAME  = 'root'
        DB_PASSWORD = ''
        DB_NAME = 'nodelogin'
        SERVER_PORT = 3000
        
6. Visual studio дээрээ terminal гарган доорх кодыг бичэн Enter дарна.

        npm start

7. Browser нээж хайх хэсэгт доорх  кодыг бичэн блог хуудсаа нээнэ:

        Localhost:3000
