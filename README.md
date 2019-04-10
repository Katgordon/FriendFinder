# FriendFinder
homework

Node and Express Servers

Overview
This is a compatibility-based "FriendFinder" application -- basically a dating app. This full-stack site will take in results from your users' surveys, then compare their answers with those from other users. The app will then display the name and picture of the user with the best overall match.

You will use Express to handle routing. Make sure you deploy your app to Heroku so other users can fill it out.

Before You Begin
Check out this demo version of the site. Use this as a model for how we expect your assignment look and operate.
Submission on BCS
Please submit both the deployed Heroku link to your homework AND the link to the Github Repository!
Instructions
Your apiRoutes.js file should contain two routes:

A GET route with the url /api/friends. This will be used to display a JSON of all possible friends.
A POST routes /api/friends. This will be used to handle incoming survey results. This route will also be used to handle the compatibility logic.
You should save your application's data inside of app/data/friends.js as an array of objects. Each of these objects should roughly follow the format below.

{
  "name":"Ahmed",
  "photo":"https://media.licdn.com/mpr/mpr/shrinknp_400_400/p/6/005/064/1bd/3435aa3.jpg",
  "scores":[
      5,
      1,
      4,
      4,
      5,
      1,
      2,
      5,
      4,
      1
    ]
}
Determine the user's most compatible friend using the following as a guide:

Convert each user's results into a simple array of numbers (ex: [5, 1, 4, 4, 5, 1, 2, 5, 4, 1]).
With that done, compare the difference between current user's scores against those from other users, question by question. Add up the differences to calculate the totalDifference.
Example:
User 1: [5, 1, 4, 4, 5, 1, 2, 5, 4, 1]
User 2: [3, 2, 6, 4, 5, 1, 2, 5, 4, 1]
Total Difference: 2 + 1 + 2 = 5
Remember to use the absolute value of the differences. Put another way: no negative solutions! Your app should calculate both 5-3 and 3-5 as 2, and so on.
The closest match will be the user with the least amount of difference.
Once you've found the current user's most compatible friend, display the result as a modal pop-up.

The modal should display both the name and picture of the closest match.
Reminder: Submission on BCS
Please submit both the deployed Heroku link to your homework AND the link to the Github Repository!
Add To Your Portfolio
After completing the homework please add the piece to your portfolio. Make sure to add a link to your updated portfolio in the comments section of your homework so the TAs can easily ensure you completed this step when they are grading the assignment. To receive an 'A' on any assignment, you must link to it from your portfolio.


You find yourself easily distracted by thoughts and ideas.
        You prefer a party over staying inside with a good book.
        You hang out with funny people rather than attractive/popular people.
        You put things off to the last minute.
        You turn to friends when something upsets you.
        Youre in tune with your surroundings.
        You hold grudges
        Truth is always more important than feelings
        You would rather stay in and cook rather than go out.
        You would drop everything and go see your friend if they needed you.
