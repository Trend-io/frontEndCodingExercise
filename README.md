# Trend Interview Take-home Challenge

This is a coding challenge designed to test user interface choices as well as coding skills for common features in a web application.
The entire set of tasks would take most mid-level front developers about 2-4 hours to finish, feel free to spend as much time as you would like. At Trend, we value the quality of the solutions not the scope or the time it takes to accomplish.

Just work through the tasks and see how many you can do in such a way that you are happy with how much you accomplished. You are free to use any library, framework, and previous code to accomplish the tasks. After submission you are free to make edits up and until the time we have agreed to review your code.

**Please fork the repository and share your version when done via email to luis@trend.io**

To be totally clear, _there is no expectation for you to complete all of the tasks_!

Thanks in advance for your time!

## Assets Folder

**influencerData_500.json**
File with less than 500 entries that simulates a DB. It has a valid JSON file that was generated with the following structure:

```json
{
  "_id": "619d411b5429558b838c0eeb", //unique identifier
  "firstName": "Norris", //first name
  "lastName": "Mcmahon", //last name
  "imagePostUrl": "https://loremflickr.com/1080/1080", //an image to simulate a content post in instagram
  "gender": "male", //gender
  "email": "norrismcmahon@wrapture.com", //email
  "phone": "+1 (993) 458-2000", //phone number
  "about": "Anim magna irure nulla irure eiusmod incididunt laborum aliqua non ea veniam proident ut ad.", //placehoder bio
  "tags": ["fugiat", "eu", "exercitation", "fugiat", "pariatur", "eu", "elit"],//placeholder tags
  "previousPaidExperience": { "video": false, "photography": true, "socialPost": false }, //if they have experience dealing with this type of content
  "skillSet": [
    { "label": "Social Posts", "yearsOfExperience": 8 }, //enum for labels Social Posts, Video Creation, Photography, Graphic Design, Video Editing, Paid Ads, Unboxing Products. and years of experience on Integers,including zero for no-experience.
    { "label": "Video Creation", "yearsOfExperience": 5 }
  ]
}
```

**influencerData_bigger.json**
Same as influencerData_500.json but with a lot more entries

## User Story
As a brand of Trend, I'd like to have a way to sort through your content creators such that I can filter the results based on the following attributes:
- Skillsets
- Gender
- Previous paid experience
- Tags

I would also like to have the option to sort this data based on **total years of experience combined from his/her skillset**, such that the example above will have a total experience of 13 years (8 from Social Posts plus 5 from Video Creation). If two records are the same we will use firstName as secondary sorting.

## Tasks

- Create the most minimal UI to accomplish this task, once again feel free to use existing libraries to shorten the time.
- All UI elements for filtering and sorting should refresh the view of the elements being displayed.
- BONUS - Implement Text Search on all the 4 fields, such that I can find creators based on keywords.
- BONUS - Implement the solution for influencerData_bigger and consider how different it is to work with a few hundred elements vs a few thousand.
- BONUS - Display the image on the list UI and make it clickable such that it expands and uses 80% of the screen vertically and is centered vertically and horizontally.

## Things to consider during your review

- Minimal Complexity
- File Organization and clear communication during commits
- Ease of maintenance
- Extensibility
- Reusability
- Best Practices for Rendering.

Good luck!
