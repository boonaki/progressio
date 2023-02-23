﻿# PROGRESSIO
A place to track and organize the progress one makes in any hobby or activity they have interest in.

**Link to project:** http://progress.cyclic.app

<!-- ![alt tag](http://placecorgi.com/1200/650) -->

## Tools Used:
HTML5, CSS3, JavaScript, MongoDB, Mongoose, Passport, EJS, Express, Multer, Node.JS 

## How It's Made:

Users can create accounts and login. When logged in, they can edit their profile, create progress reels and create captures within those reels. The idea is that anyone would be able to see the progress of anyone and their hobbies, if the user so wishes to share that progress. Signup requires unique usernames and emails, but sign-in with their e-mail. Users can also follow each other and view the followers they have.

<img src="imgs/pio1">

## Organizing your progress with the Progress Reel

To start, first you would need to create a reel, which can be seen as a folder for your progress. To do so, navigate to your profile page, then click the "create reel" button on the left hand side (desktop) or at the top of the page (mobile). From there, a popup will appear and you can title your interest/hobby then write a short description for the reel.

<img src="imgs/pio2">

## Edit User Profile

To edit your profile, simply navigate to your profile page and click the edit profile button. From there, you can change your displayed name, change your profile description, add a external link and change your profile picture. Usernames and Emails are considered to be unique, thus cannot be changed. Profiles can be made private so users that aren't following you won't be able to see your posts.

<img src="imgs/pio3">

## Info about your Captures

Within the reel view, you can like the reels, like specific captures within the reel, or check out specific captures. Within each captures, users can add comments to those captures and share what they want to share. Captures can either be an image upload, a plain text upload, or a link upload. All captures are formatted to be responsive for a large majority of devices.

<img src="imgs/pio4">

## Social and the Feed

Within the feed, you can see all captures made by people you currently follow. From there you can like, comment and soon be able to bookmark posts. Users can search for their own hobbies or interests to find captures and reels made by other people with those same hobbies or interests. If nothing found, why not start it?

<img src="imgs/pio5">

## Privacy

Being able to find the progress of others to act as a reference for your own journey is one of the many goals I wanted to reach with this project, but I do understand some may not want their progress to be shared to the world. So to help overcome that, users can hide their profile and progress from public view, where only friends can see the progress. This option has also been extended to individual progress reels, so incase you want a public account but private reels, that is also possible.

No matter what option you pick, personal information on the site is encrypted.

## Optimizations:

Many optimizations have been made throughout the course of development, most notably being the switch from arrays to objects. The feed page had multiple `includes()` array methods nested within eachother. This caused the render-time, for the page featuring the most data, to be `O(n^3)`. Switching from an array to an object to store data gave me the ability to look up properties in the object in constant time, effectively making the worse-case runtime simply be `O(n)` rather than `O(n^3)`. Although it's still not ideal, it is far better than what was implemented before.

Additionally, I was able to rewrite the styling from CSS3 to Tailwind, for easier modification to the project and to improve reusability. The entire project was previously entirely styled using CSS3, but Tailwind's ease-of-use was very persuasive in the decision to switch.

Heres a list of some of the next planned updates:
- ~~Search Functionality~~
- ~~Implement Tailwind for reusuable styles~~
- ~~Password Reset~~
- ~~Private Accounts~~
- ~~Private Reels~~
- ~~Placeholder for image links~~
- Make app Section 508 compliant
- Rich Text Editor
- Video clip/gif upload
- Bookmarks

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**NASA APOD:** https://github.com/boonaki/nasaAPODapp

**Tea API:** https://github.com/boonaki/boonakis-tea-api

**Portfolio:** https://github.com/boonaki/PortfolioV2

