In the SRC file below create resource folder 
-> in resource folder create 
1. application.properties
   -> Write the code
   spring.datasource.url=jdbc:h2:file:~/goodreads/src/main/goodreads
   spring.h2.console.enabled=true
   spring.h2.console.settings.web-allow-others=true
   spring.sql.init.mode=never
2. And create another file in src folder -  "data.sql" file
   -> Write the code
   insert into book(name, imageUrl) values('Life of Pi', 'life_of_pi.jpg');
   insert into book(name, imageUrl) values('One Night at the Call Center','one_night_acc.jpg');
   insert into book(name, imageUrl) values('Half Girlfriend', 'half_gf.jpg');
  insert into book(name, imageUrl) values('The Secret', 'secret.jpg');
  insert into book(name, imageUrl) values('Rise', 'rise.jpg');

3. And create another file in src folder -  "schema.sql" file
   -> Write the code
    create table if not exists book (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name varchar(255),
    imageUrl varchar(255)
  );
