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

✍️ Hier können Sie PAPs, Use Case- und Gantt-Diagramme oder Ähnliches einfügen.

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

Total: 

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
