##### Step 1B - Array 
Create an array.

- Create a variable called `noiseArray` and assign it to an array literal. Place at least one element in the array.

Using a native array method…

- Add a noise to the beginning of the `noiseArray`.
- Add another noise to the end of the `noiseArray`.


Using Bracket Notation…

- add another noise to the end.

Inspect the `noiseArray`

- What is the length?
- What is the last index? How is it different than the length?
- Inspect your handiwork! What does it look like?


##### Step 1C - Nest the Array in the Object
Put the `noiseArray` inside the animal object

- Create a variable called noizes and assign it the string 'noises'.
- Use the noizes variable to access the value 'null' on your animal object.
- Now use the noizes variable with the `noiseArray` to replace the value null with your `noiseArray`.
- Inspect your data structure, it should look something like this:

  `{ username: 'duck', tagline: 'Afflack', noises: ['quack', 'honk', 'sneeze'] }`
  
- Congrats! You just made a nested data structure :)  


##### Review
Let's go over some concepts:

- What are the different ways you can add properties and values to objects? 
- What about arrays?
- What if you wanted to add a property to an object that had a weird symbol?
- What about if it is a variable, how does that change the syntax?

---


### [Step 2: Animal Collection](id:collection)
A collection is an array of objects. 

- Create a variable called animals and set it equal to an empty array
  - Note that this variable is animals (plural) while the variable in step 1 is animal (singular)
- Using any method you prefer, add your animal from step 1 to the animals array.
- Create a variable called quackers and assign it to the example object that I created above:
  - `{ username: 'duck', tagline: 'Afflack', noises: ['quack', 'honk', 'sneeze', 'growl'] }`
  
- Add quackers to the animal array using a different method than before.
- Inspect your animals array to ensure you have two objects inside.
- Create two more animal objects with these properties and your choice of values: 
  - username (with a string value) 
  - tagline (with a string value)
  - noises (with an array of values)
- Check the length property of your array. It should give you 4.

---
### [Step 3: Create relationships between animals](id:relationships)
Let's think about the best data structure to represent a relationship between two animals in our collection. Imagine that our app has a 'friendslist' on an animal's profile which lists out all of the animal's friends. What do you think is the best way to represent this? Would you use an array or an object or some combination of both? Let's walk through the process together
##### 3a: Create a Friendslist
- Choose a data structure for the list of friends.
- Justify your decision.
- Create a variable called friends and assign it to the empty data structure.
- Using your animals array, add two usernames to the friends data structure.
  - ensure that you are just putting the username name, not the entire object
  - be careful not to use a destructive method like pop() that will remove the whole value from the animals array.
- Inspect your friends data structure. What does it look like?

##### 3b Create a Relationships object

Imagine now that we have more than one kind of relationship in our app, we have friends and then we have romantic matches. Let's create an object to organize these different relationships!

- Create a variable called relationships assign it to an empty object.
- Add your friends data structure to the relationships object.
- Inspect your object. What is it's length?
- Create a variable called matches and assign it to an empty array.
- Add the matches array to the relationships object. It should look like this:
  - `relationships = { friends: ['duck', 'camel'], matches: []}`
- Using the relationships object, add some username to the matches array
  - Hint: the matches array is now nested inside the relationships object!
- Inspect your object. Is the matches array now populated with some lucky username?
- Loop through your animals collection, adding the relationships object to each animal. Name the property relationships.
  - Note: it is ok that these are all the same relationship object.
