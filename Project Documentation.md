# LA-1305_MongoDB
This is a program with C# and MongoDB
Author: Lorenzo Lai

# Project Documentation

| Date | Version | Summary                                              |
| ----- | ------- | ------------------------------------------------------------ |
|   3.05.2024    | 0.0.1   | The project has been initiated. C# Project has been created and the MongoDb Compass Database has been made. |
|   10.05.2024   | 0.0.2    | The project in C# has been initiated. Bson has been implemented.                                                            |
|   17.05.2024    | 0.0.2   | The project in C# stayed as it was. I haven't made any progress this day.                                                             |
|   24.05.2024    | 0.0.3    | The project in C# has been worked on. The Bson has been succesfully and complitely been implemented. The Read function has been added.                                                             |
|   31.05.2024    | 0.1.0     | The first project prototype has been made. The Update and delete functions have been implemented. The CRUD operations weren't exactly working as intended.                                                             |
|   7.06.2024   | 0.1.1     | The C# project has been successfully updated. The CRUD funtions are now fully operational. There is a small problem with the Bson file.                                                             |
|   14.06.2024   | 1.0.0     | The Bson file problem has been solved and the project has been terminated.                                                             |

## 1 Inform

### 1.1 Your Project
This project is a console application that interacts with a MongoDB database to perform CRUD operations on a collection of jokes in C#.

### 1.2 User Stories

| US-№ | Priority | Type  | Description                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    | Must               | Functional     | As a user, I want to view jokes of a specific type so that I can enjoy humor that suits my preference.  |
| 2  | Must                | Functional     | As a user, I want to delete jokes so that the collection only contains jokes I like.                                   |
| 3  | Must                | Functional     | As a user, I want to update jokes so that the collection contains corrected or improved jokes.                                   |
| 4  | Must                | Functional     | As a user, I want to exit the application when I am done.                                   |

### 1.3 Test Cases

| TC-№ | Initial Condition | Input | Expected Output |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | The application is running.             | "Inputs an invalid joke type".         | Error. Invalid joke type not accepted, please try again.                  | 
| 1.2  | The application is running.             | "Inputs a valid joke type".        | "A joke of the specified type is displayed".                  |
| 2.1  | A joke is displayed.             | "Inputs an invalid command".        | Error. Invalid command not accepted, please try again.                  |
| 2.2  | A joke is displayed.             | "Inputs delete".        | Joke deleted. "A joke of the specified type is displayed".                   |
| 3.1  | A joke is displayed.             | "Inputs an invalid command"        | Error. Invalid command not accepted, please try again.                  |
| 3.2  | A joke is displayed.             | "Inputs update"        | Please write down the new joke.                  |
| 4.1  | A joke is displayed.             | "Inputs an invalid command"        | Error. Invalid command not accepted, please try again.                  |
| 4.2  | A joke is displayed.            | "Inputs exit"        | "Program closes".                  |

### 1.4 Diagrams

![FunnyJokesPAP](https://github.com/Loreytox/LA-1305_MongoDB/assets/110893594/8a49161d-d584-4d7a-b356-257f06f1d8a1)

## 2 Plan

| AP-№ | Deadline | Responsible | Description | Estimated Time |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |  14.06.2024     |  Lorenzo         | Set up MongoDB and create the database and collection.             | 60'              |
| 1.B  |  14.06.2024     |  Lorenzo         | Implement the Joke class.             | 15'              |
| 1.C  |  14.06.2024     |  Lorenzo         | Implement MongoDB connection in the console app.             | 10'              |
| 1.D  |  14.06.2024     |  Lorenzo         | Implement the method to view jokes by type.             | 120'              |
| 1.E  |  14.06.2024     |  Lorenzo         | Secure the program from error types.             | 120'              |
| 2.A  |  14.06.2024     |  Lorenzo         | Research about the delete functionality.             | 30'              |
| 2.B  |  14.06.2024     |  Lorenzo         | Implement delete joke functionality.             | 120'              |
| 3.A  |  14.06.2024     |  Lorenzo         | Research about the update functionality.             | 60'              |
| 3.B  |  14.06.2024     |  Lorenzo         | Implement update joke functionality.             | 180'              |
| 4.A  |  14.06.2024     |  Lorenzo         | Research about the exit functionality.            | 5'              |
| 4.B  |  14.06.2024     |  Lorenzo         | Implement exit functionality.             | 30'              |

Total: 750'

## 3 Decide
I decided to use MongoDB Compass, since I had to make a project with it in another Modul. I found it to be quite simple but also interesting, since it opened the door to a vast array of possibilities. I chose to make a Joke program, since I felt like it would habe been an adequate use of the DB and C# to show my mastery of it. Of course I still have a lot to learn, but I found this project quite fun and not as simple as I thought.

## 4 Realize

| AP-№ | Date | Responsible | Estimated Time | Actual Time |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  | 3.05.2024       | Lorenzo          | 60'              | 80'                  |
| 1.B  | 10.05.2024      | Lorenzo          | 15'              | 30'                  |
| 1.C  | 10.05.2024      | Lorenzo          | 10'              | 5'                 |
| 1.D  | 24.05.2024      | Lorenzo          | 120'              | 160'                  |
| 1.E  | 14.06.2024      | Lorenzo          | 120'              | 180'                  |
| 2.A  | 31.05.2024 / 7.06.2024      | Lorenzo          | 30'              | 45'                  |
| 2.B  | 31.05.2024 / 7.06.2024      | Lorenzo          | 120'              | 180'                  |
| 3.A  | 31.05.2024 / 7.06.2024      | Lorenzo          | 60'              | 80'                  |
| 3.B  | 31.05.2024 / 7.06.2024      | Lorenzo          | 180'              | 200'                  |
| 4.A  | 31.05.2024 / 7.06.2024      | Lorenzo          | 5'              | 10'                  |
| 4.B  | 31.05.2024 / 7.06.2024      | Lorenzo          | 30'              | 30'                  |

## 5 Control

### 5.1 Test Protocol

| TC-№ | Date | Result | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 17.05.2024     | iO         | Lorenzo       |
| 1.2  | 17.05.2024     | iO         | Lorenzo       |
| 2.1  | 7.06.2024      | iO         | Lorenzo       |
| 2.2  | 7.06.2024      | iO         | Lorenzo       |
| 3.1  | 7.06.2024      | iO         | Lorenzo       |
| 3.2  | 7.06.2024      | iO         | Lorenzo       |
| 4.1  | 7.06.2024      | iO         | Lorenzo       |
| 4.2  | 7.06.2024      | iO         | Lorenzo       |

Conclusion: I was able to implement everything within the given amount of time.
