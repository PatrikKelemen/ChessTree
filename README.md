# ChessTree

ChessTree is a ChessGUI project that aims to have a different representation of notation to be able to contain large amounts of variation and allow ease of movement between variations.  

The usual way notation is implemented with different moves is by using brackets and large amounts of variations can be lost and it becomes unclear what variations have been analyzed 

In ChessTree the aim is to alleviate this by showing the moves in a tree notation the nodes being your moves and the edges being the other sides moves. Currently ChessTree supports seeing 1 move ahead and behind without updating the position but we aim to allow users to extend how far visually the tree goes. 

With the ChessTree being visualized in a tree this allows us to remove clutter as ChessTree aims to have transpositions go to the same Node as they are the same position. This will decrease the storage size as the outcome of the position is the same if a transposition has occurred and it will visually reduce the size of the data as well. 

We also want to be able to also autocomplete transpositions, for example say you are making an opening tree and you are entering in a response to an opponent's move if there is then a move in response that your opponent can make that will create a board position that you already have entered a move for (aka a transposition to a board state from another move order) then it will add that edge to the node and make it point to the node corresponding to that board position as if it is the same board position it is assumed you make the same move. This will not only fill the tree faster but it will automatically show you the transposition potential and will give you a deeper understanding of the position.

We also want it to be clear that we aim to do more than just openings  as you will be able to enter custome starting positions and create the trees for them thus allowing you to make theoretical positions. We also want a practice feature that will select moves in the tree from the starting position and ask you what the correct moves are. 

With a notation feature as well your trees can easily make puzzles, endgame positions, openings, and middle game plans that you can share with others. 
