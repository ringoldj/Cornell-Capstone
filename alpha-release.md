# Purpose
Through my project, I wish to learn about how to build a larger project by myself. I want to learn how to use a variety of resources that I have not used before, including swift, swiftUI, CoreData, and Xcode. Additionally, I hope to learn a little bit about UI design and intergrating the frontend with the backend.

# Working Features
As of the point of the time of writing this, I have finished almost everything needed for the notes portion of this project. Notes can be made, selected from a list, edited, and deleted. Updates to notes can the order they are displayed in the selectable list, and users can start a new note while viewing a note or viewing the list of notes. Some of what is needed for tags has been added as well. The basic backend structure for tags has been completed, and the UI for tag creation has also been finished.

# Code Organization
In terms of how the code is organized, I have multiple folders for holding similar code files together. For instance, I have models folder for holding code files depicting how to handle models of the entities within the database. Similarly, there is a views folders for UI files, and a formatter folder for files depicting how to format results fetched from the database. Aside from the folders, there are some files that exist freely. These include an app file to start the app, a manager file for handling the interaction between front and back ends, and a persitance file, for setting up a way to store data throughout the app. Lastly, there is a database for the entities used in the app. 

# Function of Interest
One import function is the function for updating notes that have been changed. It takes the data that will be used to replace the old values and uses it to retrieve a specific note from its id. After safely retrieving the note, it updates the values of the note and saves the changes. This is done with some safety precautions such that if a note can't be retrieved or saved properly, nothing will happen instead of throwing an error.

# Challenges
Some problems I faced in this process were how to make a new note and add it to the stored data at the same time, as well as how to stop notes from updating when they are selected. I solved the first problem by moving the place where the note is added to the stored data to when the note is loaded. When switching to seeing the note, an optional parameter was added for the purpose of saying this note needs to be added to the stored data. For the second problem, I added additional boolean variables that guarded against updating the note if the values had not been initialized yet.

# What's Next
There are still a number of things I need to work on or would like to work on. I need to finish the UI elements for the tags, finish the backend for the tags (which means adding tags, editing them, and deleting them), and connect the tags and the notes. I would also like to add options for user customization, undo and redo buttons, a search bar, and other quality of life features if I can.
