# SpotifyStats

Imported java.io.*; for all input-output related tasks
Imported java.util.*; for the BufferedReader and ArraysLIsts; 

The main function throws IOExcpetion because it'll read an imported file. 

In order to find the info I used the FileReader & BufferedReader to import the file. 
(I tried to enter the data in the 2D Array but I couldn't figure out how to transfer the data into the 2D array- even with a nested loop) If I figure it out I'll update it. 

Instead I used arraylists to store each of the columns: 
  names of ArrayLists: positions, tracks, artists, streams, links.

I used a while loop to get through the imported file and pick up the data when it's not null.

The most streamed song is first on the artists list automatically. 

To sort the artists in alphabetical order I used Collections.Sort to alphabetize. 

To remove the duplicates I used a LinkedHashSet and it removed the duplicates. 

I created a new file called Results which displays both the most streamed artist and the list in alphabetical order. 

