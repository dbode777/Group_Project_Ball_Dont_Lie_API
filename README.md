# Group_Project_Ball_Dont_Lie_API

This was a group project that created data classes based on data scraped from the Ball Don't Lie public API. The other people that worked on the project were Justin Bartell and Colin Beveridge.

In the code, 5 data classes are created for each of the categories within the API. These included Players, Teams, Games, Stats, and Season Averages. The program reads in the text of each of these webpages, converts them into JSON, and then saves them to a list. The limit of how many data values could be collected at once led to the necessity of iteration and the time module. The request limit was 60 requests per minute, which is why we chose to use the sleep() method to wait for 60 seconds to execute the next lines of code. In hindsight, we could probably input ?limit= to extract every data value, but for the scope of this project (and due to GitHub's file size limitations), we decided to skip the creation of a stats object and/or multiple objects for each data class. There are also several instances that could be optimized (i.e. including try/except clauses, skipping the seasons that have no players, etc.), but these demonstrate if the correct information populates these objects, the data classes are constructed correctly to provide the objects' their attributes/properties.
