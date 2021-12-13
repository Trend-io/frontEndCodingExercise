# Trend Interview Take-home Exercise

This is a coding exercise designed to test UI (User Interface) choices as well as coding skills for common features in a web application.
The entire set of tasks would take most mid-level front developers about 2-4 hours to finish, feel free to spend as much time as you would like. At Trend, we value the quality of the solutions not the scope or the time it takes to accomplish.

Just work through the tasks and see how many you can do in such a way that you are happy with how much you accomplished. You are free to use any library, framework, and previous code to accomplish the tasks. After submission you are free to make edits up and until the time we have agreed to review your code.

**To be totally clear, _THERE IS NO EXPECTATION FOR YOU TO COMPLETE ALL OF THE TASKS_!** It is strongly advised for you to satisfy the requirements of the user story first while keeping in mind the "things to consider during review" section of this exercise. BONUS tasks will differentiate you from other candidates if and only if you have succesfully completed the requirements of the User Story first.

**Please fork the repository and share your version when done via email to luis@trend.io**

Thanks in advance for your time, happy coding!

## Assets Folder
Contains 2 files that have mock data that will be used in the exercise, please import the data into your code.

**influencerData_500.json**
File with less than 500 entries that simulates a DB (database). It is a valid JSON file that was generated with the following structure:

```json
{
  "_id": "619d411b5429558b838c0eeb", // <String> Unique User Id
  "firstName": "Norris", // <String>
  "lastName": "Mcmahon", // <String>
  "imagePostUrl": "https://loremflickr.com/1080/1080", // <String:Url> An image to simulate a content post in Instagram (square dimensions)
  "gender": "male", // <String:Enum [male, female]> only listing 2 genders for simplicity 
  "email": "norrismcmahon@wrapture.com", // <String:Email> 
  "phone": "+1 (993) 458-2000", // <String:USPhoneNumber>
  "about": "Anim magna irure nulla irure eiusmod incididunt laborum aliqua non ea veniam proident ut ad.", // <String> placeholder bio
  "tags": ["fugiat", "eu", "exercitation", "fugiat", "pariatur", "eu", "elit"],// <Array:String> placeholder tags
  "previousPaidExperience": { "video": false, "photography": true, "socialPost": false }, // <Object:Boolean> true means they got paid in the past doing this.
  "skillSet": [ // <Array:Object>
  // label is <String: Enum ["Social Posts", "Video Creation", "Photography", "Graphic Design", "Video Editing", "Paid Ads", "Unboxing Products"]>
  // yearsOfExperience is <Integer> (includes 0)
    { "label": "Social Posts", "yearsOfExperience": 8 }, 
    { "label": "Video Creation", "yearsOfExperience": 5 }  
  ]
}
```

**influencerData_bigger.json**
Same as influencerData_500.json but with a lot more entries

## User Story
As a brand of Trend, I'd like to have a way to find creators that fit my requirements, I would like filter your database based on the following attributes:
- Previous paid experience
- Gender
- Skillsets
- Tags

I would like these filters to work in parallel, such that I can look for a **_male_** creator with **_photography experience_** who has the skillset **_social posts_** and has **_fugiat_** as one of their tags, Mr. Norris Mcmahon should show up with this criteria.

I would also like to have the option to sort (ascending and descending) this data based on **combined years of experience from his/her skillset**, such that Norris Mcmahon (the example above from influencerData_500.json) will have a total experience of 13 years (8 from Social Posts plus 5 from Video Creation). If two records have the same total number of years, we will use firstName as secondary sorting.

## Tasks

- [ ] Create the most optimal UI to accomplish the User Story, once again feel free to use existing libraries to shorten the time.
- [ ] Import the json file (influencerData_500.json) such that the data in it is rendered on your UI.
- [ ] All UI elements for filtering and sorting should refresh the view of the elements being displayed when modified.
- [ ] BONUS - Implement Text Search on all the 4 fields from a new single input element.
- [ ] BONUS - Implement mobile-first approach with a screensize of 375pixels (width) by 812pixels (length).
- [ ] BONUS - Implement the solution for influencerData_bigger and consider how different it is to work with a few hundred elements vs a few thousand.
- [ ] BONUS - Display the image on the list UI and make it clickable such that it expands and uses 80% of the screen vertically and is centered vertically and horizontally.


## Things to consider during your review

- Minimal Complexity
- Beautiful and Modern Design
- File Organization
- Ease of Maintenance
- Extensibility
- Reusability
- Clear Communication during commits
- Best Practices for Rendering

Good luck!
