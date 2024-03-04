# blokusbot
A python implementation of the game Blokus. 




# TODO

- implement Board class. The Board is nxn grid. Each index in the grid is specified by a state enum. The state enum is empty, red, green, yellow, or blue. 
The board keeps track of previous moves and potentially which pieces are used. 
The board should have the folling methods
    - get_all_valid_origins(colour) -> returns all valid idxs for new moves of the supplied colour
    - find_valid_moves(colour, piece_list = []) -> finds all valid moves of colour, if no piece list is supplied will use all avaiable pieces.
    - checks_move(move) -> checks if move is valid

- move class (colour, piece, idxs). This needs a builder from a piece and origin

- piece representation
  - piece has potential origins
  - pieces have 4 rotations and 2 flips -> 8 states.
  - each state has potential valid origins.
  - piece has "name", placement dict, which maps rotation + flip. Each of these 
