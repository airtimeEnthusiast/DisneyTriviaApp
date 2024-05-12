# DisneyTriviaApp

### Features
- An interactive trivia app that allows a single or multiple users to answer Disney-related trivia questions.
- Implemented a scoring mechanism to assess user performance based on answer accuracy.
- Allows users to add and remove teams to save high scores.
![Features](images/image1.png?raw=true "")

### Video Demostration. 
[Video Link](https://www.youtube.com/watch?v=56Y46ykC6vg)

### Database Schema 
![Schema Version 1](images/image22.png?raw=true "Version 1")

## Table Layout

### Question
| question_id |  answer_id | question_pool_id | question_text |

### Answer: 
| answer_id | answer_text |

### Quiz:
| quiz_id | question_pool_id | type | number_of_questions | time |
 
### Trivia:
| trivia_id | quiz_id | theme |

### Team:
| team_id | quiz_id | name |

### Score:
score_id | team_id | highest_score | recent_score

### Setup Instructions 
In order to run the trivia application, the tester must set up the database — which is an integral part of the backend — so that the application will be able to properly query and retrieve the data. We have provided the instructions on how to do this below.

#### Configure inside of connection.js
Open the **API_Interface** Modify the _user_, _port_, _database_ parameters inside of connection.js so that they match your system's username, port number, and database name respectively.
![Schema Version 1](images/image9.png?raw=true "connection.js")

### Confirm in PGAdmin4 
Insures your database is connected and configured with the appropriate parameters.
![PGAdmin4](images/image3.png?raw=true "PGAdmin4 Runtime")

### Run and test the API_Interface
Use `node api.js` and run the application.
![Express.js App](images/image16.png?raw=true "API Interface")
Confirm using a web browser or [Postman](https://www.postman.com/downloads/) that the API is retrieving appropriate data.
![Schema Version 1](images/image5.png?raw=true "connection.js")



