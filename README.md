scrabble
========

Started when I was a sophomore in college.  Posting here as a backup.  


### Board: singleton 
- multi-dimensional list of board positions
- legalBoard: boolean
##### API
- place_tile(tile, position)
	- places the tile in the proper board postion
	- sets legalBoard to true or false, based on:
		- whether a move is fully horizontal or vertical (not both!)
		- whether a move is connected to an existing piece (or played on the star for the first move)
- retrieve_tiles()


### BoardPosition: helper class
- multiplier, an enum: 
	- DOUBLE_WORD 
	- DOUBLE_LETTER
	- TRIPLE_WORD
	- TRIPLE_LETTER
- state, an enum:
	- EMPTY
	- PENDING
	- FULL
	- Note: this enum is not necessary...  we can have a is_permanent boolean and use that in conjunction with the Tile being null to accomplish the same thing as this check, but I think this is cleaner.
- Tile

### Tile:
- letter, points


### TileBag: singleton
- list of tiles 
