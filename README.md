- 👋 Hi, I’m @ameer1004- Ameer Emran- Well-organized person, with high attention to detail.
- 👀 I’m interested in web development and design systems. 
      I Like to share my skills and knowledge and to learn from others as well.
 - 🌱 I’m currently learning fullstack development course. 
- 📫 How to reach me:
- Email: ameer.em.89@gmail.com
- linkedin: https://www.linkedin.com/in/ameer-emran-437a54206/





<!---
ameer1004/ameer1004 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


create table Cars(
  car_number varchar(8),
  car_company text not null,
  car_model text not null, 
  car_color text not null ,
  car_test boolean not null,
  car_report boolean not null, 
  PRIMARY KEY (car_number)
  );

  insert into Cars values
("80912201","Toyota","Corolla","Red","true","true"),
("25987361","BMW","X5","White","true","false"),
("22356944","Mercedes","E-Class","black","true","true"),
("69874523","Mazda","CX50","Red","false","false"),
("74729533","Nissan","Micra","black","true","true"),
("29568547","Audi","A4","blue","true","true"),
("23695877","Hyndai","Elantra","black","false","false"),
("36589459","Hyndai","i35","Red","true","true"),
("69823451","Volsfaigen","Passat","Grey","false","false"),
("13654889","Toyota","Camry","White","true","true");
select * from Cars;
select * from Cars where car_color="White";
select * from Cars where car_test="true";
select * from Cars where  car_report="true" and car_color="Red";
select * from Cars where car_number="29568547";

create table products(
  product_barcode varchar(3),
  product_name text not null,
  product_price numeric not null, 
  product_company text not null ,
  product_expiry boolean not null ,
  PRIMARY KEY ( product_barcode)
  );
  insert into products values
  ("910","xyz",9,"aaa","true"),
  ("920","abc",40,"bbb","false"),
  ("930","ghg",20,"ccc","true"),
  ("940","ket",12,"ddd","true"),
  ("950","yza",25,"eee","false"),
  ("960","milka",22,"fff","true"),
  ("970","terma",50,"ggg","false"),
  ("980","nutella",18,"hhh","true"),
  ("990","nbvkd",8,"kkk","false"),
  ("991","lfkhdo",35,"fff","true");
  select * from products;
  select * from products where product_price<15;
  select * from products where product_price>10 and product_price<30;
  select * from products where product_expiry="true";
  select COUNT(product_barcode) FROM products;
  SELECT AVG(product_price)FROM products;

