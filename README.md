# CISC-121-Sebastian-Capraru-Final-Project

## Chosen Problem: Playlist Vibe Builder

I chose to build this app because it helps you organize a messy list of songs into a perfect playlist by organizing them by genre and sorting them by energy. I decided to use energy and genre to build playlists becasue these two go hand in hand when listening to music and are often related with eachother. It makes sure the "vibe" of the playlist stays consistent from start to finish, and its something that I would use and find very useful as someone who listens to a lot of different types of music.

## Chosen algorithm: Quick Sort

I chose to use quick sort to build this app instead of merge sort becasue I feel that its a better and more efficient sort to understand and build from. It is also a very fast and efficient way to handle a long list of songs without the app slowing down. It works by picking one song as a "pivot" to compare against other, which is also a great way to decide if a song has higher or lower energy or a different genre than the rest of the playlist. Because this algorithm automatically splits the list into smaller and smaller groups, it makes it much easier for the user to follow along as well.

## Preconditions: 

Before the sorting even starts, the app assumes that every song in the list has a valid genre assigned to it and an energy score between 0 and 100. To make sure this works, the app goes through the entire list first to check for any missing energy scores or empty genre labels so the app doesn't break or malfunction. Another advantage using quick sort is the data can be at random and doesn't need to be sorted at the start unlike other sorting algos, in this case it is made to take a completely random pile of songs, match them with user genre and energy preferences and create desirable playlists to listen too.

## Computational Thinking (4 pillars etc..):


Decomposition:
First, the algorithm finds all the unique genres in the list and groups the songs together so that all the genres are sectioned off. Once the songs are grouped by genre, the algorithm then breaks those smaller groups down even more for sorting based on energy. Finally, it takes each genre group as a mini playlist, and goes through the same steps to make sure the whole playlist is perfectly organized from start to finish.

Pattern Recognition:
The algorithm follows a simple, repeating pattern where it always looks for a "reference" song to compare the others with. It checks if a song’s energy is higher or lower than that reference and swaps their positions if they are in the wrong spot. By doing this same pattern over and over, the messy list naturally turns into an organized playlist.

Abstraction:
I chose to show the user the most important visual details, like which song is the current pivot and which two songs are being swapped, so they can see the "vibe" changing in real time. On the other hand, I am getting rid of the complicated background recursive calls that the computer uses to keep track of the sub lists with. These things are left out because they would make the screen look too cluttered and confusing for a person to watch.

Algorithm Design:
The process starts when the user interacts with a button on the app to sort their music by genre or energy. The app then takes the input request and runs my custom quick sort algortihm which move the songs around on the screen. Once the sorting is finished, the app shows the final, perfectly ordered playlist ready for the user to listen too.

Data Structures:
I will be using a list of dictionaries to store the song data. Each dictionary will hold a song's information as a string for the title and genre, and an integer for the energy score, which makes it very easy to find and compare the values during the quick sort process.


## Testing and Edge Cases:

I tested the algorithm using a messy and large variety list of songs with different genres and energy levels to make sure the Quick Sort correctly grouped genres alphabetically and sorted energy from highest to lowest. I also tested edge cases like entering an empty list or a song with a 105 energy score, to make sure my logic noticed, found and fixed the errors instead of crashing the app.

## Hugging Face Link: https://huggingface.co/spaces/sc1x/playlist-vibe-builder/tree/main
## How to run the app:
To run this app on locally on your own computer, first open the terminal or vs code and type pip install -r requirements.txt to download the needed libraries. Once that is done just run the code given in hugging face or github on app.py and click the local URL link that appears to open the Playlist Vibe Builder in your browser.

## I provided my flow chart screenshot where I posted the code running as well in the Visual file in main!!

## AI USAGE: USED AI TO HELP WITH CODING ESPECIALLY THE GRADIO IMPLEMENTATION, THE QUICK SORT CODE NOT SO MUCH AS WE LEARNED THAT IN CLASS! I ALSO USED AI FOR THE SAMPLE IMPUT YOU SEE IN THE VISUAL. I ALSO USED AI TO HELP REFINE/SIMPLIFY AND DEBUG MY CODE!
