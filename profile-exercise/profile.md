Profile page exercise
====

This exercise is meant to show a command of the technologies we use, as well as a keen head for problem solving and
attention to detail. We ask to have the challenge returned within **three days** of it being assigned.

It should take approximately 3 hours to finish this task, but let us know if you need more time.

If you do not have time to finish the task, please leave comments describing how you would have implemented the missing
parts, and/or why you have made certain compromises.
### The exercise

In our platform we have staff members that can login and access their profile page.
We want you to recreate this profile page based on the design ([Link to design](https://www.figma.com/file/hfzA73ocJ6gGyB7flia4RZ/front-end-test?type=design&node-id=1-516&mode=design&t=wkFsycnNr6tWvXT6-0)), and make sure that it meets all standards for good code
and implementation.

In the following exercise, certain design elements of the solution are provided via the design in Figma, while other elements of the solution, has been left out of the design for you to come up with an implementation.

The solution should:

* Display the personal info provided by the json data in the "Personal Info" section 
* Provide functionality to edit the personal info, with input validation based on the input field types. The data should be made editable when the "Edit info" button is clicked
* Provide functionality to upload a new profile picture
* Display profile picture provided by the upload functionality
* Provide functionality to remove the profile picture

If there is time left after completing the above:

* Display list of interests in the "Other settings" section
* Provide functionality to add and delete interests. 

The data for the view is coming from and endpoint, which you will mock using the JSON data provided below:

```json
    data: {
        "firstName": "Angus",
        "lastName": "Ward",
        "email": "angus-ward862@hessel-greenfelder.dk",
        "phoneNumber": "+4510203040",
        "profileImage": null,
        "birthday": "1990-10-09",
        "interests": [
            "Soccer",
            "Beer brewing",
            "Bicycling",
            "Wine"
        ]
    }
```

### Requirements:

* Ensure that the profile page is responsive and looks good on both desktop and mobile devices.
* Use any JS framework or vanilla JS for creating the solution (big plus if you are using Vue.js, but it is certainly not a requirement!).
* You can use any CSS frameworks (e.g., Tailwind) or custom CSS to style the page.

### How to hand it in 

Please upload your solution to a git repository (BitBucket, GitLab or GitHub) and provide a README file with
documentation, including how to run your solution, then send us a link to the repo (make sure it's public or otherwise
accessible).
