# quizzer
A simple standalone application to conduct and score Quizzes: MCQ evaluator and result genrator.


In order to solve the digital quizzing problem, I have designed a Java based desktop application using JSwing that provides an interactive interface to an instructor for generating a quiz and to a student for attempting those quizzes.

Instructors after logging in, are allowed to create a Quiz by providing a short title and description for the quiz. Once a quiz has been created, the application then allows the instructor to add a question (of type multiple choice, true false or numeric). For each question the instructor must add a text for the question, options (4 for MCQs, 2 for True False and none for numeric), expected correct answer (watch out for long expected answers. On successful creation of the quiz, It is stored its state by using serialization for persistent storage. Every time the application starts, the quizzes are deserialized to reload the application state.

For students, a view is created to display all quizzes that allows the user to take a particular quiz. The user attempts the quiz by providing his answers, which are matched against the correct answers and a score is calculated. At the end of the quiz, simple the score for the user are displayed in this attempt.
