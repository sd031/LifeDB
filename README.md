LifeDB
======

Lightweight database targeting mobile, tablet devices.

This is the source code for LifeDB. This small lightweight lightning first database is for mobile apps. I have tested the database with my Moto E 
and the famouse world city database. The output speed and other performence study is just jawDropping.

Inintially I used PHP for development but also this easy algorythm can be implemented in any language i believe.

I'm using a page based locking system for executing the database transaction like MyISAM database engine. Further documentation is coming soon


basic test cases are here
  $instance = new LifeDB("jsondb_1.json");
  $instance->insert("student","{\"name\":\"arindam\",\"title\":\"karmokar\"}");
  $instance->insert("student","{\"name\":\"piklu\"}");
  $instance->insert("teacher","{\"name\":\"shyamal\"}");
  $instance->insert("teacher","{\"name\":\"aritrik\"}");
  $instance->insert("student","[{\"name\":\"arindam1\"},{\"name\":\"piklu1\"}]");
