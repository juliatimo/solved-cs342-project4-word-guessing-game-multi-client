Download Link: https://assignmentchef.com/product/solved-cs342-project4-word-guessing-game-multi-client
<br>
This is your official team project. You will create a server that plays a word guessing game with each client that connects to that server (similar to Wheel of Fortune or Hangman). Each client that logs into the server must guess 3 different words in 3 different categories to win. First, the client picks a category. The server will send the client the number of letters in a word from that category to guess. The client gets to guess a total of six letters, one at a time.

The client will guess a letter and send it to the server. The server will respond with either: the letter is in the word and where that letter is located or the letter is not in the word and how many guesses are left.

If the client guesses the word within 6 letter guesses, they can not guess at another word in the same category but must chose from the two remaining. If they do not guess the word correctly, they are free to choose from any of the three categories for another word. Clients may guess at a maximum of three words per category. If they do not make a correct guess within three attempts, the game is over. The game is won when the client successfully guesses one word in each category. When the game is over, the client can either play again or quit.

<strong>Implementation Details:</strong>

You will create two separate programs, each with a GUI created in JavaFX, one for the server and one for the client. Use the Maven templates provided.

All networking must be done utilizing Java Sockets (as shown in class). <strong>The server must run on its own thread and handle each client on a separate thread. Each client must connect and communicate with the server on a separate thread.</strong> You may not use libraries or classes not included in the standard Java 8 release.

<strong>The server:</strong>

When the server program starts, you must be able to enter in the port number to listen to and start the server. The server will NOT limit the number of clients connected at one time. For instance, if there are 8 clients connected to the server, then there will be eight individual games being played on eight separate threads.

The server will maintain a list of words in 3 different categories( for example: Animals, U.S. States, Superheroes, Foods …..etc).

The server will NEVER send the word to the client, only the number of letters, respond to guesses and keep track of remaining guesses, keep track of categories and words guessed as well as winning and losing of the game.

The server will not send the client the same word twice in any one game.

You will utilize a serializable class as the only means of passing information between the server and each client.

<strong>The serverGUI:</strong>

You must provide a way to enter the port to listen to and start the server.

You must provide a server log that reports on what the server is doing (similar to your last project)

You may add anything else you feel is appropriate or needed.

<strong>The Client GUI:</strong>

You must provide a way for the client to log into the server

You must create an interface, utilizing the design principles discussed in class that is intuitive and allows the client to play and understand the progress of the game. There will be <strong>5 points extra credit</strong> for exceptional and creative UI and UX design.

<strong>Use of templates found on the web: </strong>

You may use ideas from GUI templates( fxml, css, images or other) for styling your programs found on the web. You may not import those templates and pass them off as your own work. If you use an idea or part of such template, include a reference to that work in the header of the file where used. Failure to do this will result in academic misconduct charges.

<strong>All other logic must be your original work.</strong>

<strong>Testing Code: </strong>

A minimum of 10 unit tests are required. They can be in either the server or client program or in both.

<strong>Documentation:</strong>

You will provide the following documentation of your project in a single PDF with a cover sheet including the team number and names of all team members

<ul>

 <li><strong>UML Class, Activity Diagrams and Wireframe: </strong></li>

</ul>

You are required to include a UML Class Diagram and Wireframes for the client and server programs as well as an Activity Diagram for the client program.

<ul>

 <li><strong>Report</strong>

  <ul>

   <li>Give a general description of the server and client logic. This description should highlight and discuss algorithms and design choices made.</li>

   <li>Explain how you developed the UI and UX of the project and what/how you implemented certain design principles.</li>

   <li>Discuss how you chose to work together on this project:</li>

   <li>how you divided up the work</li>

   <li>how you collaborated</li>

   <li>what worked and what did not</li>

   <li>each teammate should describe in their own words what they contributed.</li>

  </ul></li>

</ul>

<strong>We will test all projects on the command line using Maven 3.6.1. You may develop in any IDE you chose but make sure your project can be run on the command line using Maven commands. Any project that does not run will result in a zero. If you are unsure about using Maven, come see your TA or Professor. </strong>

<strong><em>This is a team project. You may share and communicate at will with your teammates but are forbidden from collaboration with other teams. </em></strong>

Unless stated otherwise, all work submitted for grading *must* be done individually.  While we encourage you to talk to your peers and learn from them, this interaction must be superficial with regards to all work submitted for grading.  This means you *cannot* work in teams, you cannot work side-by-side, you cannot submit someone else’s work (partial or complete) as your own.  The University’s policy is available here:

<a href="https://dos.uic.edu/conductforstudents.shtml">https://dos.uic.edu/conductforstudents.shtml</a>.

In particular, note that you are guilty of academic dishonesty if you extend or receive any kind of unauthorized assistance.  Absolutely no transfer of program code between students is permitted (paper or electronic), and you may not solicit code from family, friends, or online forums.  Other examples of academic dishonesty include emailing

your program to another student, copying-pasting code from the internet, working in a group on a homework assignment, and allowing a tutor, TA, or another individual to write an answer for you.  It is also considered academic dishonesty if you click someone

else’s iClicker with the intent of answering for that student, whether for a quiz, exam, or class participation.  Academic dishonesty is unacceptable, and penalties range from a letter grade drop to expulsion from the university; cases are handled via the official student conduct process described at <a href="https://dos.uic.edu/conductforstudents.shtml">https://dos.uic.edu/conductforstudents.shtml</a><a href="https://dos.uic.edu/conductforstudents.shtml">.</a>