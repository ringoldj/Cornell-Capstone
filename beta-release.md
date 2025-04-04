## Requirements Met or Not:

When I look back at what I set out to do with my project in my proposal, I have finished almost everything I said I would. I have made it so that I can make, update, and delete notes. The notes can have tags, which can also be made, updated, and deleted. The only thing that I have not done is add a search feature for notes and tags.

## Methods:

When building my project, I used Xcode as my IDE, the language swift, the swiftUI framework for my user interface, and CoreData as my database. My code was structured such that I had multiple folders for holding files with separate purposes. I had a folder for holding views, or everything user interface related, a folder for holding models (which were a way for me to make my own representation of data from the database for easier handling), and a folder for holding formatters, which allowed my to get and organize data for the models. In my views folder, there were three particularly important files depicting the three main screens a user would be seeing. They were for listing tags the user defined, listing notes made, and interacting with a note. When a user taps on a listed tag, they are taken to a list of notes with that tag. Similarly, when a user taps on a note, they are taken to the note to interact with it.

## Project Management:

For my daily routine, I first Identified the task I was going to work on. Next, I would plan how I was going to complete this task; what should the display look like, how should the data be managed, and so on. If I needed to learn something for this task, I would then go and figure out what I needed. When I felt I could achieve the task, I would work on it and take note of any new tasks I thought of in the process. While working, I would constantly test the code to see if it worked or not and would make adjustments accordingly. When I finished, I would go on to the next task. I tracked my progress through this work by the features I had completed.

## What I Learned:

I learned a number of skills throughout this project. I learned a little about how to use Xcode as an IDE, how to write code in swift, how to use swiftUI to display elements, and how to store and access data with CoreData. For some things I learned in particular, I got an understanding of optionals in swift. Before this project, I knew nothings of optionals, and now I know they are a way of telling the program this may hold a value, or it may be nil. They are declared with a question mark and can be handled by putting an exclamation point behind the optional when you know it will hold a value. I also learned that swiftUI uses views, which display something on the screen, whether it be visual or some invisible form of interaction or organization.

## Problems and Solutions:

While making the program, I had difficulty passing data not stored in the database between different screens. This was especially so since the screens only sometimes needed the ability to pass data to another screen when they were shown. I eventually learned I needed to use a binding, a way of linking a variable between two separate structures, to pass data, but this did not solve the problem in not needing to pass data every time. I solved that problem by using an init statement telling the program to just accept a binding if one was given and to essentially ignore it otherwise. Unfortunately, even after this, I still had problems since it did not appear that the value was being passed back correctly. In actuality, I had just prevented the data that had been passed back from doing anything with an incorrect guard statement. After adjusting the guard statement, everything worked fine.  

## What’s Next?:

There are many things I would like to do with my project still. I would like to add the ability to search for tags and notes when viewing a list of them. Additionally, I want to add the ability to filter by multiple tags at the same time. Furthermore, when viewing tags or notes, I want a way to view them not in a list, but through a group of windows. User customization would also be nice to allow for changes in text size or a dark mode. Lastly, adding the ability to further change the text through colors, bolding, highlighting, and so on would be good.
