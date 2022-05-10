---
title: Peer Review Finder
---

# Table of Contents

* [About Peer Review Finder](#about-peer-review-finder)
* [Deployment](#deployment)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Project Team](#project-team)


# About Peer Review Finder

* [Live Demo](https://peer-review-finder.xyz)
* [GitHub Organization](https://github.com/peer-review-finder)
* [Team Contract](https://docs.google.com/document/d/129I7p6RzvGBnGv6KCANo64H4_rCuaIOBxddQX1s_jI8/edit?usp=sharing)
* [Project Board Milestone 1 (Completed)](https://github.com/peer-review-finder/Source-Code/projects/1)
* [Project Board Milestone 2 (Completed)](https://github.com/peer-review-finder/Source-Code/projects/2)
* [Project Board Milestone 3 (Completed)](https://github.com/peer-review-finder/Source-Code/projects/3)

## The Problem

Journal editors and conference chairs find it increasingly difficult to find reviewers for publication manuscripts. At the same time, researchers receive an overwhelming number of invitations to review papers.


## The Solution

We propose a platform that better matches papers for review with potential reviewers by pooling researchers with similar interests together. Editors/chairs can post abstracts in need of review and researchers can select abstracts of papers they'd like to review.


# Deployment

We are using DigitalOcean for deployment of this application.

[Live Demo](https://peer-review-finder.xyz)


# User Guide

The following sections describe the main features of this application as of Milestone 3.


## Landing Page

New users are first taken to a landing page.  Here users see a brief description of features within the application.  A Login link is provided on the top right of the page to allow existing users to login with their profile or for new users to register and setup a profile page.

![](images/m3/landing.png)


## Login Page

Clicking on the Login link and then on the Sign In menu item, you will be directed to the page pictured below. On this page, users can log in to Peer Review Finder to access the web application.

![](images/m3/signin.png)


## Register Page

Clicking on the Login link and then on the Sign Up menu item, you will be directed to the page pictured below. On this page, new users can sign up and create a Peer Review Finder account. 

![](images/m3/signup.png)


## Landing Page After Login (General User)

A successful login brings users to the following page below. Here, users have access to the many different functionalities as explained in the sections below.

![](images/m3/landing-user.png)


## Landing Page After Login (Admin User)

An admin user has an additional item in the navigation bar for administrative tasks.

![](images/m3/landing-admin.png)


## Profile Page

After logging in to your Peer Review Finder account, clicking on your email in the navbar on the top right of the page prompts a dropdown to show up. If you click on View Profile, you will be redirected to your profile page. From here, you can view your profile and you can also edit your profile by clicking on the Edit Profile button.

![](images/m3/profile.png)


### Edit Profile Page

After clicking on the Edit Profile button, you will be redirected to the page below where you can edit your Peer Review Finder profile which consists of your name, your profile image, and your interests. After you have finished, you can press submit to save your changes and from there, you will be redirected to your profile page.

![](images/m3/edit-profile.png)


## Paper Listing Page (All Users)

By clicking "View Papers" on the [Landing page after login](#landing-page-after-login-general-user), users are able to see papers that are available to review.  Papers available are listed with a brief abstract along with a link to view each paper.

![](images/m3/list-papers.png)

### Filtering Papers

Users can filter the papers displayed by searching based on areas of interest.

![](images/m3/list-papers-search.png)


## Add Paper Page (All Users)

Clicking "Upload Paper" in the navbar allows users to add a new paper to the Peer Review Finder database to allow other users to view and review the paper.  Uploading a paper requires 3 tokens.

![](images/m3/add-paper.png)

### Not Enough Tokens

If the user does not have enough tokens to upload a paper, a helpful message is displayed explaining why and how to earn tokens, as well as a button to find papers to review.

![](images/m3/add-paper-not-enough-tokens.png)


## View Paper Page (All Users)

Clicking the "View Paper" button on the [Paper Listing page](#paper-listing-page-all-users) for a specific paper allows users to see a full abstract of that paper along with a link to download the full paper. 

![](images/m3/view-paper.png)

This page also allows users to review the particular paper by typing in the review textbox and then pressing the submit button to submit the review to the database.

![](images/m3/view-paper-submited-review.png)

After submitting the review, users are also allowed to edit the review, should they feel the need to make changes to their review for a certain paper.

![](images/m3/view-paper-edit-review.png)


## My Papers (All Users)

By clicking "My Papers" on the [Landing page after login](#landing-page-after-login-general-user), users are able to see their own papers.  Users can also view and edit their papers.

![](images/m3/my-papers.png)

### No Papers

If the user has no papers yet, a helpful message is displayed explaining why no papers are displayed, as well as a button to upload a paper.

![](images/m3/my-papers-none.png)


## My Reviews (All Users)

By clicking "My Reviews" on the [Landing page after login](#landing-page-after-login-general-user), users are able to see the reviews they have left for others.

![](images/m3/my-reviews.png)


### No Reviews

If the user has left no reviews yet, a helpful message is displayed explaining why no reviews are displayed, as well as a button to find papers to review.

![](images/m3/my-reviews-none.png)


## View Paper Reviews (Paper Owner)

By clicking on the View Paper button on the My Papers page, users are able to view a listing of reviews left on their paper.

![](images/m3/view-paper-list-reviews.png)


## Edit Paper Page (Paper Owner and Admin Users)

By clicking on the edit paper button on the My Papers Page, users are able to edit their papers and upload the changes after they are done.

![](images/m3/edit-paper.png)


## View/Rate Review Page (Paper Owner)

By clicking on the View Review button on the View Paper page, users are able to view the review left on their paper, and rate the quality of the review.  Users will receive 3 tokens for a 5 star review, 2 tokens for a 4 star review, 1 token for a 3 star review and 0 tokens otherwise.

![](images/m3/view-review.png)


## Admin Paper Listing Page (Admin Users)

By clicking "Admin" in the navbar, admin users are able to see all papers.  Admin users can view, edit, and delete any paper.

![](images/m3/admin.png)

### Delete Paper

By clicking the "Delete Paper" button for a particular paper, admin users are able to delete said paper.  Before deleting, a confirmation is displayed to ensure no accidental deletions are made.

![](images/m3/admin-delete-paper.png)


# Community Feedback

We interviewed five UH graduate community members to get their opinions on our project, here's what they said:

### Henri C.
- Landing page: expecting to be able to click on action related heading, such as "Create an Account!"
- User home page: expecting to be able to click on "PAPERS MATCH YOUR INTEREST"
- View papers page: searching does not work
- Add paper page: unexpected behavior when invalid URL provided for "Link of Paper"
- Edit paper page: expected to go back to my papers page when finished
- My reviews page: would be nice to have a link to edit review
- General: suggestion, move "View Papers" button in navbar to user home page

### Chakhon L.
I was able to complete the tasks in a reasonable amount of time. All the tasks were pretty straight forward, but it would be nice if it had auto filling for the author and an abstract like how easyBib can detect the author. Also, maybe allowing users to view the paper in the Your Review page will be convenient instead of searching for the paper in View Papers. I don’t think I will use the application if it goes live since I don’t write much paper and it seems like there is no reward for reviewing.

### Hao W.
The app overall is good. The app is also fast and clean. However, the location for some functionalities could be more intuitive. When you go to the home page, you should have the ability to view other papers, meaning put the view papers navbar item onto the home page. Also on my papers page, it would be nice to have the ability to upload a paper on that page as well. My reviews page could have the ability to edit reviews on the same page for convenience but this is not necessary. I would consider using the application if I wrote more papers and wanted them to be reviewed.

### Katie A.
- Functionality wise it’s fast and simple to use, and it feels like it’d be easy to put any paper on there
- An “About” page might be nice to talk about the site’s intent, but idk how polished this is.
- Is there a way to prevent idea stealing from papers? Like a confidentiality thing or copyright thing? Idk the correct term, but if I were hoping to submit a paper and my data wasn’t proprietary or my own, that would be a concern of mine

Otherwise it looks like a cool site, I hope it goes well for your class!

### Sharon C.
Yes, I was able to complete the task in a reasonable amount of time. Although, I would like a step by step photo or list of what we have to do first to start the process. I realize there is the github.io page, and that is a good example of what I mean, so it would be helpful to new users if that was linked somewhere on the website. Also, a way to upload images and/or papers from your desktop would be a nice feature to have. Possibly being able to add an image for a paper can help entice other users to peer review your paper and bring in more attention to the paper. Maybe also having a popup when you hover over a paper to give users a more detailed overview of the paper before clicking on view paper to view the full paper.


# Developer Guide

This project currently passes the Continuous Integration via Github Actions as shown by this badge: 

![ci-badge](https://github.com/peer-review-finder/Source-Code/workflows/ci-peer-review-finder/badge.svg)

## Backend System

This application was built on meteor-application-template-react.  For information regarding this template, please refer to [https://ics-software-engineering.github.io/meteor-application-template-react/](https://ics-software-engineering.github.io/meteor-application-template-react/)


## Installation

First, [install Meteor](https://www.meteor.com/install).

Second, [download a copy of Peer Review Finder](https://github.com/peer-review-finder/Source-Code).

Third, cd into the app directory and install the required libraries:

```
cd /path/to/peer-review-finder
cd app
meteor npm install
```


## Running the system

Once the libraries are installed, you can run the application by invoking:

```
meteor npm run start
```


## Viewing the running app

If all goes well, the template application will appear at [http://localhost:3000](http://localhost:3000).


## ESLint

You can verify that the code obeys our coding standards by running ESLint over the code in the imports/ directory with:

```
meteor npm run lint
```


# Project Team

- [Yiwen Chen](https://yiwenc22.github.io/)
- [Derrick Luyen](https://derrickluyen.github.io/)
- [Kolwin Dixon](https://k-l-dixon.github.io/)
- [John Dobbs](https://john-dobbs.github.io/)
- [Aditi Jaiswal](https://jaiswal-aditi.github.io/)
