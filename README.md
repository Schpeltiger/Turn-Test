# Turn-Test

Generate the solution using the uproject file.

A simple implementation of handling 'turns.' Implemented in the gamemode blueprint, it basically gets all of the characters in the level and 
sorts them according to their initiative value.

Once sorted, the player is given possession of the first / fastest entity. Once the turn end event is fired, the possession is moved to the next entity in the sorted array.
Once the end of the array is reached, the active characters get sorted again (the initiatives can change but the ordering is fixed on single turn).

The initiative is accessible in the editor or via some function when implemented. Possession may also be skipped through some condition if for example, we wish to let an AI control the said pawn.
