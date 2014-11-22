# About
Humans is an experiment in standardizing and distributing social beings. Just like real life, we are all objects, so we can all be represented in code. If enough people create themselves in a standard object format, we can begin to interact in a meaningful way by writing our own interfaces. To see a sample human, take a look at johnDoe.json. There will also be a constructor object to aid people in creating their own self objects.

# Privacy
Because we won’t want to share everything about ourselves, a simple privacy index is added to each object. 0 is public; .5 is half public, half private; 1 is private. Objects inherit the privacy level of their parents, unless specified explicitly. For example, John Doe Shares His name and basic information with everyone, but his date of birth is reserved for people who he knows better. By indexing privacy in a percentage, it can be possible for different people to have access to different levels of personal information. While John shares any privacy:0 data with the whole world, maybe only family or close friends would have access to his object on a level above .7 privacy.

#Participating
The first step to participating in the humans project is to begin creating your self.json. For now, just model it after johnDoe.json. Since names aren’t unique identifiers, though, using “self.json” as the filename should suffice temporarily. A suggested naming convention is up for debate, so head over to [the naming issue](https://github.com/kevincoleman/humans/issues/1) to voice your input.

As you begin to add data to your object, please do send pull requests to modify johnDoe.json with suggestions of how to structure the data, so we end up following a standard format and everyone is on the same page.

## johnDoe.json
John Doe is a sample human. He is one example of how you can structure your data, and is constantly changing based on popular suggestion. Below are some underlying rules to make your life easier when it comes to structuring data:

  + Every object contains a privacy attribute unless it should inherit its parent’s privacy value
  + Numbered values should be stored as numbers, not as number strings
  + Values that need units specified should have separate “units” and “amount” properties.
  + Single properties with unique privacy values should denote their privacy values alongside their property values by using a contained object with properties “privacy” and “value”. See a [sample](https://github.com/kevincoleman/humans/blob/783a65a96119e6f1af4f2b7fa13b35806a65a5e8/johnDoe.json#L31).
