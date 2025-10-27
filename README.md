🧠 Tic Tac Toe — SWI-Prolog Web Application

A fully interactive Tic Tac Toe game built entirely using SWI-Prolog’s HTTP libraries.
You can play in Two Player Mode or challenge an AI bot powered by the Minimax algorithm — all through a simple web interface.

🚀 Features

Two Game Modes

Two Player Mode – play locally with a friend.

Play vs Bot – challenge an intelligent Prolog-based AI.

AI Intelligence – uses the Minimax algorithm for unbeatable logic.

Modern Web UI – dynamic HTML/CSS interface with animations.

Game Sessions – powered by Prolog’s session management.

Instant Reset – restart the game anytime with one click.

🏗️ Technologies Used

This project is powered entirely by SWI-Prolog, leveraging its powerful logic programming capabilities and built-in web libraries.

Language: SWI-Prolog

Core Libraries:

http/thread_httpd – runs the built-in web server

http/html_write – dynamically generates HTML content

http/http_dispatch – handles route requests

http/http_session – maintains player sessions and game state

http/http_parameters – processes URL and form parameters

Frontend: Pure HTML and CSS generated directly from Prolog predicates

AI Logic: Implemented using the Minimax algorithm with scoring heuristics

⚙️ Installation & Setup
1. Install SWI-Prolog

Download and install SWI-Prolog from the official site:
👉 https://www.swi-prolog.org/Download.html

2. Clone This Repository
git clone https://github.com/<your-username>/tic-tac-toe-prolog.git
cd tic-tac-toe-prolog

3. Run the Server

Open SWI-Prolog and load the project file:

?- [tic_tac_toe].


Start the web server:

?- start_server.


You should see:

Server started at http://localhost:8082

4. Play the Game 🎮

Open your browser and go to:

http://localhost:8082


Then:

Choose a Game Type (Two Player or Play vs Bot)

Select your side (X or O)

Enjoy the game!

🧩 Game Logic Overview

game_type_page/1 – Displays and processes the game type selection.

choose_player/1 – Lets the player choose between X and O.

display_game_board/0 – Renders the current game board dynamically.

make_move/1 – Handles player moves and updates the board state.

ai_move_and_display/1 – Controls the AI move logic using Minimax.

winner/2, tie/1, and switch_player/2 – Implement the main game rules.

winning_line/3 – Identifies and highlights the winning cells.

🤖 AI Logic (Minimax Algorithm)

The bot evaluates all possible future moves using the Minimax algorithm to always make the optimal choice:

+10 for an AI win

–10 for a human win

0 for a draw

The AI explores all possibilities recursively, ensuring it never loses — though you might be able to force a draw.

💅 User Interface

The interface is simple, responsive, and animated for a pleasant experience:

Glowing winner cells with pulsing effects ✨

Animated winner text when the game ends

Clean grid layout and hover transitions

Subtle color palette and rounded design

🧠 Future Enhancements

Add sound effects and move animations

Implement online multiplayer support

Track player statistics and high scores

Deploy using Docker or a cloud Prolog server

🏁 Author

Sutha S
Engineering Student — Computer Science and Business Systems
🎯 Passionate about logic programming, AI, and web development.

💬 Feedback & Contributions

If you like this project, please ⭐ it on GitHub!
Feel free to open issues or submit pull requests to improve the game.
