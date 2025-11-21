# Mānoa RoomieMatch

---

## Table of contents

* [Overview](#overview)
* [Team](#team)
* [Our Github](#our-github)
* [Deployment](#deployment)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Continuous Integration](#continuous-integration)
* [Example enhancements](#example-enhancements)

---

## Overview

Mānoa RoomieMatch is a web application that provides UH students with a personalized, AI-enhanced roommate matching experience. Students log in and create a lifestyle profile covering sleep routines, cleanliness standards, study habits, noise tolerance, guest expectations, cooking frequency, personality traits, and budget/space preferences. The system compares profiles to generate a compatibility score, along with an AI-generated explanation describing areas of alignment and potential conflict. Students can browse matches, view detailed comparisons, and reach out to peers they’re compatible with. In addition, the system can generate AI-assisted communication templates, personalized housing advice, and conflict-prevention tips based on the student’s preferences.

It illustrates various technologies useful to ICS software engineering students, including:

* HTML and CSS
* Nextjs
* React
* React Bootstrap

### The problem:
Every semester, hundreds of UH Mānoa students struggle to find compatible roommates—whether in the dorms (Hale Aloha, Gateway, Frear) or in off-campus apartments. This issue is amplified by the fact that approximately 31% to 36% of the UH Mānoa student population comes from out of state, meaning a large portion of students arrive in Hawaiʻi without established local connections or housing arrangements. Students commonly report conflicts due to mismatched sleep schedules, noise preferences, cleanliness expectations, guest habits, or study routines. Without a structured way to evaluate compatibility, students rely on random Snapchat and posts, word-of-mouth searching, or even dating apps, often resulting in stressful living situations, roommate conflicts, and frequent room switches.

There is currently no UH-focused platform that helps students understand whether they are compatible *before* committing to live together.

### The solution:
Mānoa RoomieMatch will provide a convenient roommate search for UH students. It will reduce roommate conflicts through compatibility insights, and give a clear preview and expectations of potential roommates.

---

## Team

Mānoa RoomieMatch is designed, implemented, and maintained by [Kyla Kanemoto](https://kylakanemoto.github.io/), [Katelynn Crouch](https://kkcrouch808.github.io/), [Anh Minh Nguyen](https://anhminhnguyen2.github.io/), [Adones Morales](https://reditgem3581.github.io/), [Kincade Morimoto ](https://kincademorimoto.github.io/) and [Bryan Kikugawa](https://brkiku.github.io/).

### Team Contract

Our code of conduct can be found [here](https://docs.google.com/document/d/1NyC7RrhGOPZXYOhnl6m2bFdEJb18yUVXbsEGcyLYXpI/edit?tab=t.0)

---

## Our GitHub
* [Mānoa RoomieMatch Organization](https://github.com/manoaroomiematch)
* [Mānoa RoomieMatch Home Page](https://manoaroomiematch.github.io)
* [Mānoa RoomieMatch Application](https://github.com/manoaroomiematch/manoaroomiematch.git)
* [Mānoa RoomieMatch Organization](https://github.com/orgs/manoaroomiematch/projects/2/views/1)
---

## Deployment

Mānoa RoomieMatch is currently being deployed [here](https://github.com/manoaroomiematch/manoaroomiematch.git)

---

## Approach

Once a student creates their lifestyle and housing profile, the system stores their preferences and makes them available for matching.

### User Flow
1. **Login and Profile Setup:**  
   Students log in using UH email authentication and complete a structured lifestyle questionnaire. Preferences include sleep schedule, cleanliness level, social habits, noise tolerance, personality, study style, daily routines, and housing goals.

2. **Match Browsing:**  
   Students browse potential roommates filtered by preferences such as major, budget, dorm choice, lifestyle habits, and shared interests.

3. **AI Compatibility Evaluation:**  
   The system uses AI to:
   - Analyze two profiles  
   - Generate a compatibility score  
   - Provide strengths, conflicts, and suggestions  
   - Create tailored “first message” templates to contact matches  

4. **Notifications (optional stretch):**  
   Students can receive notifications when new profiles appear that meet their criteria.

5. **Admin Functions:**  
   Admins can:
   - Flag inappropriate content  
   - Create new lifestyle categories  
   - Manage and review profiles  
   - Adjust system presets (e.g., default survey questions)

---

## User Guide

This section provides a walkthrough of the Mānoa RoomieMatch user interface and its capabilities.

### Landing Page

The landing page is displayed when users visit the main RoomieMatch site. It introduces the platform’s purpose and key features.

<div class="text-center p-4">
  <img width="500px" src="../img/landing_page_mock.png" class="img-thumbnail" >
</div>

- Explanation of the platform  
- “Start Matching” call-to-action  
- Summary of AI features  

### Profile Setup Page

After logging in through UH email authentication, new users are directed to the profile setup page to complete a multi-step lifestyle questionnaire.

<div class="text-center p-4">
  <img width="300px" src="../img/profile_setup_mock.png" class="img-thumbnail" >
</div>

- Multi-step lifestyle survey  
- Progress indicator  
- Save-as-you-go  

### User Home Page

Once a profile is completed, users are taken to their personalized home page.

<div class="text-center p-4">
  <img width="500px" src="../img/user_home_page_mock.png" class="img-thumbnail" >
</div>

- Overview of user’s profile  
- Compatibility highlights  
- Quick access to matches  
- Notifications  

### Browse Matches Page

Users can explore potential roommates on the Browse Matches page.

<div class="text-center p-4">
  <img width="500px" src="../img/browser_matches_mock.png" class="img-thumbnail" >
</div>

- List or grid of potential roommates  
- Match percentages  
- Preview of key traits  
- “View Details” button  

### Match Details Page

Selecting a match brings the user to a detailed comparison page.

<div class="text-center p-4">
  <img width="300px" src="../img/match_details_mock.png" class="img-thumbnail" >
</div>

- Side-by-side comparison  
- AI-generated compatibility report  
- Suggested conversation prompts  

### Admin Home Page

The Admin Home Page provides tools for managing the platform and maintaining content quality.

<div class="text-center p-4">
  <img width="300px" src="../img/admin_home_page_mock.png" class="img-thumbnail" >
</div>

- Manage users  
- Moderate flagged content  
- Add/edit lifestyle categories  

**All mockup images were generated by ChatGPT.**

---

## Use Case Ideas

### 1. New student signs up and sets up their profile 
* Student visits the landing page
* Reads about how RoomieMatch works
* Logs in using UH authentication
* Completes the lifestyle survey
* Arrives at their home page
* Reviews recommended matches
* Learns how compatibility scoring works

### 2. Student searches for compatible roommates
* Logs in
* Navigates to “Browse Matches”
* Filters by dorm, budget, lifestyle traits
* Selects a high-scoring match
* Reads AI-generated compatibility explanation
* Uses AI message template to reach out

### 3. Admin monitors and manages the platform
* Admin logs in
* Goes to Admin Home Page
* Reviews flagged profiles
* Updates lifestyle categories
* Manages user accounts

---

## Community Feedback

We are interested in your experience using Mānoa RoomieMatch!

---

## Developer Guide

This section provides information for developers wishing to use this code base as a basis for their own development tasks.

### Installation

First, [install PostgreSQL](https://www.postgresql.org/download/). Then create a database for your application.

Second, go to [https://github.com/RateMyTool/RateMyTools_SC](https://github.com/RateMyTool/RateMyTools_SC), and click the "Use this template" button. Complete the dialog box to create a new repository that you own that is initialized with this template's files.

Third, go to your newly created repository, and click the "Clone or download" button to download your new GitHub repo to your local file system. Using [GitHub Desktop](https://desktop.github.com/) is a great choice if you use MacOS or Windows.

Fourth, cd into the directory of your local copy of the repo, and install third party libraries with:

```
$ npm install
```

Fifth, create a .env file from the sample.env file. Edit the .env file to set the DATABASE_URL to point to your PostgreSQL database.

### Running the system

Once the libraries are installed and the database is configured, you can run the application by invoking:

```
$ npm run dev
```

The first time you run the app, it will create default data in the database.

### Viewing the running app

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000).

### ESLint

You can verify that the code obeys our coding standards by running ESLint over the code in the src/ directory with:

```
$ npm run lint
```

### Application Design
TBD

### Data model
TBD

---

## Initialization
TBD

---

## Development History

The development process for BowFolios conformed to [Issue Driven Project Management](https://courses.ics.hawaii.edu/ics314f25/morea/project-management/reading-guidelines-idpm.html) practices. In a nutshell:

- Development consists of a sequence of Milestones.
- Each Milestone is specified as a set of tasks.
- Each task is described using a GitHub Issue, and is assigned to a single developer to complete.
- Tasks should typically consist of work that can be completed in 2-4 days.
- The work for each task is accomplished with a git branch named “issue-XX”, where XX is replaced by the issue number.
- When a task is complete, its corresponding issue is closed and its corresponding git branch is merged into master.
- The state (todo, in progress, complete) of each task for a milestone is managed using a GitHub Project Board.
- The following sections document the development history of ManoaRoomieMatch.

### Milestone 1: Mockup pages development
The goal of Milestone 1 was to create AI-Generated photos of the UI for this project. Then, implement mockup pages to the website.

Milestone 1 was managed using [Manoā RoomieMatch GitHub Project Board M1](https://github.com/orgs/manoaroomiematch/projects/2/views/1):

![](img/m1_issues.png)

<div class="text-center p-4">
  <img width="500px" src="../img/landing_page_mock.png" class="img-thumbnail" >
</div>

<div class="text-center p-4">
  <img width="300px" src="../img/profile_setup_mock.png" class="img-thumbnail" >
</div>

<div class="text-center p-4">
  <img width="500px" src="../img/user_home_page_mock.png" class="img-thumbnail" >
</div>

<div class="text-center p-4">
  <img width="500px" src="../img/browser_matches_mock.png" class="img-thumbnail" >
</div>

<div class="text-center p-4">
  <img width="300px" src="../img/match_details_mock.png" class="img-thumbnail" >
</div>

<div class="text-center p-4">
  <img width="300px" src="../img/admin_home_page_mock.png" class="img-thumbnail" >
</div>


### Milestone 2
The goal of Milestone 2 was to use the completed front-end pages and improve the functionality. In this Milestone we will be focusing on the back-end components (e.g database, page linking, API, etc.).

Milestone 2 was managed using [Manoā RoomieMatch GitHub Project Board M2](https://github.com/orgs/manoaroomiematch/projects/5/views/1?visibleFields=%5B%22Title%22%2C%22Status%22%2C%22Assignees%22%2C239381711%2C239381747%2C239381801%2C239381851%5D):

<!-- ![](img/m1_issues.png) -->

### Milestone 3
TBD

---

## Continuous Integration
TBD

---

## Example enhancements

After building the core features, the following advanced options can enhance the platform:

* Dorm Recommendation System – Implement AI-based suggestions for UH dorms based on user preferences such as noise level, budget, room type (double, suite, apartment), and AC availability.
* Language Translation for International Students – Add automatic translation of profiles, bios, and messages to help international students communicate and encourage cross-cultural roommate matching.
* UH Authentication for Verification – Integrate UH Single Sign-On to verify that all users are current UH students, improving trust and campus safety.
* Advanced Matching Insights – Display analytics such as compatibility heatmaps, potential conflict alerts, and personalized compromise suggestions to help users make informed roommate choices.
* Roommate Agreement Generator – Create an AI-driven roommate agreement that outlines expectations for cleaning schedules, guests, quiet hours, shared spaces, and privacy.
* Schedule Compatibility Sync – Sync users’ UH class schedules to highlight overlapping free hours, sleep routines (morning vs. night), and optimal times for shared facilities.
* Household Planner – Build shared tools for roommates to manage chore rotations, track expenses, and coordinate grocery lists.
