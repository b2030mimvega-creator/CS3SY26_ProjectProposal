# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template:
cvbbbc
### Project Title or Name of the Application	:
### Section			   	      :9-Cesium
### Group Members			    :DE BELEN, HUMARANG, VEGA
### Date (Proposal Date)  : Nov 12, 2026
fdfhdfhfshsdhfhhtrthdfh
### Project Description:

Nowadays, high school students have to prepare for countless exams: Mid-quarter exams and finals over many different subjects. So finding effective studying methods are important to perform well. One example is the use of flashcards, this provides the student with an interactive aspect to help them better understand and remember what they are studying as opposed to static studying like reading notes or textbooks. However, physical flashcards can get misplaced or cluttered, our project aims to create a digital version that retains all the studying benefits of regular flashcards while removing the uncertainties of the physical counterpart.

Our digital flashcard quizbot is a python-based object-oriented application meant to help students of all ages study for their upcoming requirements. Users can customize their own flashcards and decks to use for personal review sessions. These review sessions can be timed or untimed and will provide a score summary at the end.

Target Demographic:
Students preparing for exams



System Components (classes, methods, object interactions)

Class 1: Flashcard

Attributes:

- Question: The prompt/question displayed to the user

- Answer: The correct answer to the given question

- Subject: The subject where the question falls under

- Difficulty: A scale to determine the difficulty of the question (Easy, Medium, Hard)

- Question_type: The type of question given on the flashcard (Multiple Choice, True or False, Short Response)


Methods:

- check_answer(input)
  
Compares a user input to the flashcard’s answer attribute and returns True if it matches and False if not

- get_hint()
  
Returns a letter/segment of the expected answer to provide a hint to the user




Class 2: Deck


Attributes:

- Name: The name of the deck for future reference

- Cards: A list containing the contents or the individual flashcard classes in the deck


Methods:
- add_card(card)

Appends another given flashcard class to the Cards attribute of the deck

- remove_card(index)

Removes a card from the Cards attribute of the deck with the specific given index

- shuffle_deck()

Randomly arranges the contents of the Cards attribute of the deck before a review session begins

- get_total_cards()

Returns the total number of cards in the deck

- get_subjects()

Returns the subjects in the subject attribute of the cards in the Cards attribute of the deck to find out what subjects the review session will cover

- get_difficulty()

Returns the difficulty level of each card in the deck to show how difficult the cards are in the quiz

- get_type()

Returns the question type of the cards in the deck to show what types of questions are in the quiz



Class 3: Quiz

Attributes:

- User: The name of the user taking the quiz/review session

- Decks: the deck/s going to be used for the quiz

- Score: the tally of correct answers the user was able to give

- Missed: A list containing all the flashcards that the user answered incorrectly for future use

- Time_taken: a float variable to determine how long the quiz has been going on

- Time_limit: the time limit where the quiz has to be completed. If zero, then the quiz is untimed


Methods:

- deck_summary()

Displays the summary of the deck chosen to the user (number of cards, subjects included, types of questions included, and difficulty level)

- start_quiz()

Loops through Deck_used.Cards and displays all the prompts and questions on the flashcards, calls the check_answer method of the flashcards, then updates the score and missed attributes of the Quiz class

- percent_score()

Returns a calculated percent score of the user based on their correct answers

- display_summary()

Shows the user the summary of that review session, their score, their percent score, their time taken, and a list of all the things they got wrong and the proper answers to them

- end_quiz()

Stops the quiz and the loop after the review session is completed





Class Interactions:

- The Deck class uses aggregation to store and different Flashcard objects to be used for the review sessions

- The Quiz class directly uses and interacts with the Deck class by retrieving cards from it and shuffling it. The Quiz class also repeatedly calls methods of the Flashcard class to check the user’s answer.



**Sample class Diagram from https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png:**

![Sample Diagram](https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png)

### Goals:

Describe the long term outcomes of your project followed by a couple of objectives to meet the goals stated in this paragraph

- Objective 1:
- Objective 2:
- Objective n:

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
