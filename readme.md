<!--
Creator: Alex White
Market: SF
Adapted By: Zeb Girouard
Market: DEN
-->

<!-- Next time, I should explicitly mention limit, where/like and demo the first query together -->

![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)

<!--Actually 11:35 -->
<!---WDI3 11:31, 11:43 turning over to devs -->
<!--11:20 15 minutes  Go through directions and clue #1-->

<!--Actually finished 11:48 -->

# Where in the World Is Carmen Sandiego?

![](http://i.giphy.com/13n8txR8c9UDHG.gif)

## Introduction

> ***Note:*** _This will be a pair programming activity._

#### Use SQL to find Carmen Sandiego

We're going to use what we've learned already about searching with SQL commands, and apply it to chase down and capture an elusive and world-reknowned thief, Carmen Sandiego. Follow the clues, use the interweb - write down both the SQL commands /queries you used and your answers to the clues - and figure out where Carmen is headed, so we can catch her and bring her in.

## Exercise

#### Starter code

- Fork and clone the repo.
- Check out the [starter-code](starter-code/world.sql)

#### Requirements

- Use the ``clues.sql`` file as your "answer sheet"
- From the command line, create a new database called ```carmen``` and populate it with the SQL found in ```world.sql```

```
# Enter psql
psql

# Create database
CREATE DATABASE carmen;

# Connect to carmen
\c carmen
\i world.SQL
```

**Pro Tip:** You can do this in one step with the command:

```bash
createdb carmen; psql -d carmen -f /your/path/to/this/file/starter-code/world.sql
```

Then, use the clues below to create the appropriate SQL queries to help you find Carmen and then, tell us where she's heading!!

In order to check your progress, you can run your answers in your answer sheet by

1. Entering ```psql``` in the command line
2. Switching to the ```carmen``` database you just created
3. Executing the SQL query
4. Saving the result and query that works in ```clues.sql```

### The Clues

  - **Clue #1:** We recently got word that someone fitting Carmen Sandiego's description has been traveling through Southern Europe. She's most likely traveling someplace where she won't be noticed, so find the least populated country in Southern Europe, and we'll start looking for her there.

  - **Clue #2:** Now that we're here, we have insight that Carmen was seen attending language classes in this country's officially recognized language. Check our databases and find out what language is spoken in this country, so we can call in a translator to work with you.

  - **Clue #3:** We have new news on the classes Carmen attended: our gumshoes tell us she's moved on to a different country, a country where people speak *only* the language she was learning. Find out which nearby country speaks nothing but that language.

  - **Clue #4:** We're booking the first flight out: maybe we've actually got a chance to catch her this time. There are only two cities she could be flying to in the country. One is named the *same* as the country – that would be too obvious. We're following our gut on this one; find out what other city in that country she might be flying to.

  - **Clue #5:** Oh no, she pulled a switch: there are two cities with very similar names, but in totally different parts of the globe! She's headed to South America as we speak; go find a city whose name is *like* the one we were headed to, but doesn't end the same. Find out the city, and do another search for what country it's in. Hurry!

  - **Clue #6:** We're close! Our South American agent says she just got a taxi at the airport, and is headed towards the capital! Look up the country's capital, and get there pronto! Send us the name of where you're headed and we'll follow right behind you!

  - **Clue #7:** She knows we're on to her: her taxi dropped her off at the international airport, and she beat us to the boarding gates. We have one chance to catch her, we just have to know where she's heading and beat her to the landing dock.

  - **Clue #8** Lucky for us, she's getting cocky. She left us a note, and I'm sure she thinks she's very clever, but if we can crack it, we can finally put her where she belongs – behind bars.

```
  Our playdate of late has been unusually fun –
  As an agent, I'll say, you've been a joy to outrun.
  And while the food here is great, and the people – so nice!
  I need a little more sunshine with my slice of life.
  So I'm off to add one to the population I find
  In a city of ninety-one thousand and now, eighty five.
```


#### Starter code

Again, be sure to grab the .sql file from the [starter-code](starter-code/world.sql) and run it in your PostgreSQL terminal using the commands above.

#### Deliverable

Use the clues.sql file to write in the SQL queries that correspond with each clue and tell us where she's heading at the bottom:

<p align="center">
  <img src ="http://s3.postimg.org/8386vdt43/Screen_Shot_2015_07_08_at_8_11_25_PM.png">
</p>


## Additional Resources

- [PostgreSQL tutorial](http://www.tutorialspoint.com/postgresql/)
- [PostgreSQL official documentation](http://www.postgresql.org/docs/)

## Licensing
All content is licensed under a CC­BY­NC­SA 4.0 license.
All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
