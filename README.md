In the center of the great lake Nozama, there is a treasure chest. The quest is to swim across the lake Nozama to
get the treasure chest. Whoever reaches the treasure chest first becomes the winner. A set of warriors go to swim
across this lake. Each warrior is wearing a pair of swim fins that helps him to swim. There are different types of fish
in this lake. Some fish are innocent, they just swim around the lake. Some fish love to eat rubber, so they pull out
the swimming fins of warriors. If a warrior loses a fin, he cannot swim. Killer fish is the most dangerous; they can
kill the warriors. In lake Nozama, there are magic lotus flowers. Each lotus flower has 100 petals. If a warrior
plucks out a lotus petal, he becomes immortal. The warriors are also of two types. Each super warrior has
binoculars. They can look for any lotus flowers in the vicinity. Normal warriors cannot see a flower unless he
bumps into one.




==================================further elaboration====================================
Lake Nozama can be thought of as a simple 10*10 grid as shown in Figure 1 (you do NOT have to implement the
GUI for this). The warriors, fish, and lotus flowers are located only at line crossings (see the red dot in Figure 1).
Note that if you count in terms of line crossings, it is 11*11. Coordinates of treasure chest are (5,5). Warriors know
this location. There are four warriors in the game. These warriors should always start moving from the border of
the grid (e.g. (0,0), (5,0)). Six fish (two from each type) and five lotus flowers should be randomly placed in the grid 
before the game starts. For simplicity, assume that fish is staying in one location (any fish does not move). When a
warrior is swimming, in one go, he moves from one line crossing to the other along the lines (e.g. he can move
from (0,0) to (0,1) but not to (1,1)). In one go, he can take only a single jump to the nearest line crossing.
No two warriors can occupy the same line crossing. Therefore before moving to a line crossing, a warrior should
check whether the line crossing is already occupied by another warrior. The warrior can check this only in the
nearest line crossings, along the lines (e.g. if the warrior is in (0,0) he can see (0,1), but not (1,1)). However,
warriors cannot see whether there is any fish in the vicinity. Normal warriors cannot even see lotus flowers in the
vicinity. When looking for lotus flowers using binoculars, a super warrior can see the flowers in the nearest line
crossings, along the lines (e.g. if the warrior is in (0,0) he can see (0,1), but not (1,1)).
When a warrior starts swimming, he first notifies this to the treasure chest. When the first warrior reaches the
treasure chest, it notifies all the other warriors that there is a winner. Other warriors should stop moving upon the
receipt of this message. This is the end of the game, and the information of the winner should be recorded in the
permanent storage, along with the finishing time.



Clone this reposistory and run the game demo class.
