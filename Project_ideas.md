Word guessing game

Summary: 2 player hangman type game where one player submits a word, and the second player guesses letters until they run out of guesses or correctly guess the word. It then swaps roles. Points are awarded for the number of guesses left when the word is correctly guessed (example: You had 3 guesses left, and got the word right, you get 3 points; you don’t correctly guess the word you get 0 points. 

Commands to server:

connect(char *username, char *password): Server assigns first log in as player 1 and asks for a secret word, then waits. Once another user uses the connect command it assigns them as player 2 and starts the guessing game. Once player 2 correctly guesses or runs out of attempts, it then asks player 2 for a word, and lets player 1 start guessing.

submitLetter(char c): Player guessing the word submits a letter guess to the server. Server returns a string with the correctly guessed letters or a null string if the letter doesn’t exist in the word

guessWord(string s): Guessing player guesses the full word, server returns true for accurate guess else false

score(): server returns player 1 and players 2 scores.

end(): ends the game, telling each player their final score and if they won or lost, then disconnects both players.

Others?

Summary:Our project is a hangman style game where the user guesses letters until the word is revealed or they run out of attempts. Points are awarded for the number of attempts left when the word is correctly identified. For example: if the word was “cat”, the round started with 3 points, and the user guessed the letter “r” they would lose a point and be prompted to guess again. If they then guessed “a” they would be shown “_ a _” and would not lose a point. If they then guessed the whole word “cat” they would be awarded 2 points for the round. Points will be based on the length of the word being guessed. 

Ideally this will be a 2-player game, where 1 player submits the word to be guessed, player 2 guesses, and after player 2 uses all their guesses or correctly guesses the word, the roles reverse and player 1 guesses the word player 2 submits. After a set number of rounds the point totals will determine a winner of the 2 players.

***space reserved for any additional info about our code (stretch goals accomplished etc.)***