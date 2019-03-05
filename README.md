starter-snake-kotlin
===

[![Build Status](https://travis-ci.org/athenian-programming/starter-snake-kotlin.svg?branch=master)](https://travis-ci.org/athenian-programming/starter-snake-kotlin)

A simple [Battlesnake AI](http://battlesnake.io) written in Kotlin.

Visit [https://docs.battlesnake.io](https://docs.battlesnake.io) 
for API documentation and instructions for running your AI.

This snake is built using a lightweight http server Spark framework - [http://sparkjava.com/documentation](http://sparkjava.com/documentation)

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

Requirements
---

- Install JDK 8 [http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- Install Kotlin [https://kotlinlang.org](https://kotlinlang.org)
- Install Gradle [https://gradle.org/install/](https://gradle.org/install/)

Running the snake
---

```bash
./gradlew run
```

Snake will start up on port 8080

This snake can run from within Intellij using [ngrok](https://ngrok.com). 

Run the tests
---

```bash
./gradlew test
```


Executable Jar
---

```bash
./gradlew stage
```

Will result in a jar file in `build/libs` called `starter-snake-kotlin.jar`

You can then run this file with the command

```bash
java -jar build/libs/starter-snake-kotlin.jar
```


Deploying to Heroku
---

1) Create a new Heroku app:
```
heroku create [APP_NAME]
```

2) Deploy code to Heroku servers:
```
git push heroku master
```

3) Open Heroku app in browser:
```
heroku open
```
or visit [http://APP_NAME.herokuapp.com](http://APP_NAME.herokuapp.com).

4) View server logs with the `heroku logs` command:
```
heroku logs --tail
```
