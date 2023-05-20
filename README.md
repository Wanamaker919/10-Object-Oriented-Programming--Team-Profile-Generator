# 10 Object-Oriented Programming: Team Profile Generator

## Your Task

Your task is to build a Node.js command-line application that take
about employees on a software engineering team, then generates an 
displays summaries for each person. 

Because this Challenge will require the use of the `Inquirer` pack
you install and use Inquirer version 8.2.4. To do so, use the foll
your project folder: `npm i inquirer@8.2.4`.

Testing is key to making code maintainable, so you’ll also write a
every part of your code and ensure that it passes each test.

Because this application won’t be deployed, you’ll need to provide
walkthrough video that demonstrates its functionality and all of t
You’ll need to submit a link to the video AND add it to the readme

> **Note**: There is no starter code for this assignment.

## User Story

```md
AS A manager
I WANT to generate a webpage that displays my team's basic info
SO THAT I have quick access to their emails and GitHub profiles
```

## Acceptance Criteria

```md
GIVEN a command-line application that accepts user input
WHEN I am prompted for my team members and their information
THEN an HTML file is generated that displays a nicely formatted te
on user input
WHEN I click on an email address in the HTML
THEN my default email program opens and populates the TO field of 
the address
WHEN I click on the GitHub username
THEN that GitHub profile opens in a new tab
WHEN I start the application
THEN I am prompted to enter the team manager’s name, employee ID, 
and office number
WHEN I enter the team manager’s name, employee ID, email address, 
THEN I am presented with a menu with the option to add an engineer
to finish building my team
WHEN I select the engineer option
THEN I am prompted to enter the engineer’s name, ID, email, and Gi
and I am taken back to the menu
WHEN I select the intern option
THEN I am prompted to enter the intern’s name, ID, email, and scho
taken back to the menu
WHEN I decide to finish building my team
THEN I exit the application, and the HTML is generated
```

## Mock-Up

The following image shows a mock-up of the generated HTML’s appear
functionality:

![HTML webpage titled “My Team” features five boxes listing employ
and other key info.](./Assets/10-object-oriented-programming-homew

The styling in the image is just an example, so feel free to add y

## Getting Started

This Challenge will combine many of the skills we've covered so fa
the User Story and Acceptance Criteria, we’ve provided some guidel
started.

Because this Challenge will require a video submission, refer to t
Blog Video Submission Guide](https://coding-boot-camp.github.io/fu
computer-literacy/video-submission-guide) for additional guidance 
video.

Your application should use [Jest](https://www.npmjs.com/package/j
the unit tests and [Inquirer](https://www.npmjs.com/package/inquir
collecting input from the user. The application will be invoked by
following command:

```bash
node index.js
```

It is recommended that you start with a directory structure that l
following example:

```md
.
├── __tests__/             //jest tests
│   ├── Employee.test.js
│   ├── Engineer.test.js
│   ├── Intern.test.js
│   └── Manager.test.js
├── dist/                  // rendered output (HTML) and CSS style
├── lib/                   // classes
├── src/                   // template helper code 
├── .gitignore             // indicates which folders and files Gi
├── index.js               // runs the application
└── package.json           
```

**Important**: Make sure that you remove `dist` from the `.gitigno
Git will track this folder and include it when you push up to your
repository.

The application must include `Employee`, `Manager`, `Engineer`, an
classes. The tests for these classes (in the `_tests_` directory) 

The first class is an `Employee` parent class with the following p
methods:

* `name`

* `id`

* `email`

* `getName()`

* `getId()`

* `getEmail()`

* `getRole()`&mdash;returns `'Employee'`

The other three classes will extend `Employee`.

In addition to `Employee`'s properties and methods, `Manager` will
following:

* `officeNumber`

* `getRole()`&mdash;overridden to return `'Manager'`

In addition to `Employee`'s properties and methods, `Engineer` wil
following:

* `github`&mdash;GitHub username

* `getGithub()`

* `getRole()`&mdash;overridden to return `'Engineer'`

In addition to `Employee`'s properties and methods, `Intern` will 
following:

* `school`

* `getSchool()`

* `getRole()`&mdash;overridden to return `'Intern'`

Finally, although it’s not a requirement, consider adding validati
user input is in the proper format.

## Grading Requirements

> **Note**: If a Challenge assignment submission is marked as “0”,
incomplete and will not count towards your graduation requirements
incomplete submissions include the following:
>
> * A repository that has no code
>
> * A repository that includes a unique name but nothing else
>
> * A repository that includes only a README file but nothing else
>
> * A repository that only includes starter code

This Challenge is graded based on the following criteria:

### Deliverables: 15%

* A sample HTML file generated using the application must be submi

* Your GitHub repository containing your application code.

### Walkthrough Video: 32%

* A walkthrough video that demonstrates the functionality of the T
Generator and passing tests must be submitted, and a link to the v
included in your README file.

* The walkthrough video must show all four tests passing from the 

* The walkthrough video must demonstrate how a user would invoke t
from the command line.

* The walkthrough video must demonstrate how a user would enter re
the prompts in the application.

* The walkthrough video must demonstrate a generated HTML file tha
user input.

### Technical Acceptance Criteria: 40%

* Satisfies all of the preceding acceptance criteria plus the foll

  * Uses the [Inquirer package](https://www.npmjs.com/package/inqu

  * Uses the [Jest package](https://www.npmjs.com/package/jest) fo
tests.

  * The application must have `Employee`, `Manager`, `Engineer`, a
classes.

### Repository Quality: 13%

* Repository has a unique name.

* Repository follows best practices for file structure and naming 

* Repository follows best practices for class/id naming convention
quality comments, etc.

* Repository contains multiple descriptive commit messages.

* Repository contains a high-quality readme with description and a
walkthrough video.

## Review

You are required to submit the following for review:

* A walkthrough video that demonstrates the functionality of the a
passing tests.

* A sample HTML file generated using your application.

* The URL of the GitHub repository, with a unique name and a readm
project.

---
© 2022 edX Boot Camps LLC. Confidential and Proprietary. All Right
