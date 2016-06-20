# Word-Count-Challenge
Write a program that given a phrase can count the occurrences of each word in that phrase.” My code needs to return an object that has one  property for each word in the phrase, and each property’s value should contain  the word count.
// input: "one fish two fish red fish blue fish"
// output should be: var expectedCounts = { one: 1, fish: 4, two: 1, red: 1, blue: 1 };


    var input = "one fish two fish red fish blue fish";

    var wordArray = input.split(/\s+/);
    var wordCounts = {};

    for(var i = 0; i < wordArray.length; i++){
       var word = wordArray[i];

    // ! returns whether the statement can evaluate to false
    // if word is not already a property in wordCounts object, add 1
     if(!wordCounts[word]) {
         wordCounts[word] = 1;
         } else { 
         wordCounts[word]++;
	   }
    }
      console.log(wordCounts);
