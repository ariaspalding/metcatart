# metcatart

For my Programming for Cultural Heritage final project, I was interested in exploring the representation of cats in artwork over time. 
This generator will show the user a random artwork from the Metropolitan Museum of Art's collections that features cats. 
I found it really fun to explore the various ways cats have shown up in art throughout human history, time and space. 

About my process ~
To create this generator, I used the Met's Open Access CSV file containing data on much of their collections' objects to identify objects that were tagged 
with 'Cats.' I tried a couple other methods, like using the API to query "cats," but I found the results were inconsistent and not all relevant; searching 
the CSV file for objects specifically tagged "Cats" yielded much more accurate results. I then gathered the Object IDs associated with these cat-tagged 
artworks and fed them into the Met's API, which has a search by Object ID function. This allowed me to create a for loop that returned full data for each 
cat-related artwork, incuding artist, medium, culture, date, etc, and I stored all of this data in a JSON file. Because of the importance of artwork images 
to this generator, I excluded any objects that did not contain image links in their metadata. 

I used HTML and JavaScript to create the random generator itself (with Prof. Matt's very gracious help lol). I used the Math.Random() function to randomly 
select an artwork and its data to display whenever the button is clicked. I chose to display the artwork's title, artist, culture, date, and medium along with 
its image, and excluded the rest of the objects' metedata (but of course not every artwork has all of this data available). Lastly, I simply embedded the random 
generator code into this Google site!

The website can be found at: https://sites.google.com/pratt.edu/met-cat-art/home

Enjoy!!
