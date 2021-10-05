# Backend - Database - Basics - Let's MonGO

## Let's monGO

Add your answers directly into this README file.

1. Explain ObjectIDs in MongoDB; what are they?
2. You have a collection called "users" with a document like this: `{ _id: 1, name: "Veera" }`. What query would you use to update the name to "Princess Veera Silkenfur"?
3. How do you make a collection?
4. So the (old) mongo shell is kind of like a JavaScript REPL. What is a REPL? Which other REPL have we used?
5. So the (old) mongo shell is kind of like a JavaScript REPL. You can use things like variables, try...catch  statements and loops. Experiment with it and find at least three other JavaScript things that we have used that work in the (old) shell. If you can, try to find even more!
6. (Research) So the old shell is pretty cool. How is the new shell better?
7. (Research) How can you insert multiple documents at the same time?
8. (Research) You have a collection called `cats` with a documents like this: `{ name: "Veera" }, { name: "Rauli" }, { name: "BenBen" }` - How can you insert the field `cute: true` into all of them with one command?
9. (Task) Start a timer for 30 minutes. Spend all that time getting to know and reading https://docs.mongodb.com/manual/introduction/ - how far did you get? What was the most cool or interesting thing you learned?
10. Find one SQL Cheatsheet and one MongoDB Cheatsheet and add links to them here.

------------------------------------------------------------------------------------------------

my Answers;
1- objectIDs in MongoDB are ids Numbers to define evrey object so with that can we update our items thre like (Name or id or any thing other).

2- we have two options to do this , but here we don't have the id:objectID ,so im gonna use the default method:
db.users.updateOne({"name":"veera"},{$set:{"name":"Princess Veera Silkenfur"}});

3- db.createCollection("ABDUL");

4- Perl, is an expressive language. You get your work done with just a few lines of code.like u wanna print ("Hallo World "), u can just write ----->    print ("Hallo World");
we used other mehtods in perl like forEach, for loop ,catch(e).

5- like we have collection called user we wanna to print the name (object name )so we can give a variable like :
   let X=db.user.findOne();
   print(X.name);
we can use forEach two like this Example:
db.user.find().forEach(doc => print(doc.name));
to catch Error we write this command:
try { this.will.fail() } catch(e) { print(e); };
we used this Example below to inserting more data:
db.user.insertOne({id:984758956,name:"ronaldo",favourit:"football"});

6-  new shell is better cuz we write less codes and easier way than old 1.

7- we can use this command to insert multiple documents:
    db.user.insertMany({id:984758956,name:"banana",price:766},{id:984758956,name:"apple",price:999},{id:984758956,name:"food",price:666});

8- here we have to use forEach Method:
    db.food.updateMany({},{$set:{cute:true}});

9-  

10- SQL Cheatsheet:select from *(--tableName--) ,
Link:
https://learnsql.com/blog/sql-basics-cheat-sheet/

    **MongoDB Cheatsheet: show collections, and in this link we find alot of them: https://www.mongodb.com/developer/quickstart/cheat-sheet/







































🌿
