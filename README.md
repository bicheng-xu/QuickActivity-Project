<h2>QuickActivity</h2>
<h3>Note:</h3>
<p>
In total, since our group consists of four people, we have four contributors. The contributors are Bicheng Xu, Yubo Hu, Xiuyu Wu and Shuyang Dai.
<b>In the contributors, xiuyuw and Nick Wu is actually the same person!</b>
</p>

<h3>Objective:</b>
<p>
To create an online activity posting and attending system where every logged in person can post activities and attend any activities if he/she fits the requirements, especially the age requirement, say, a 15-year-old user cannot view the activity which has an age requirement of 19. Everyone who has not logged in can only search and view the activities which have a minimum age requirement less than or equal to 16 years old.
</p>

<h3>Project description:</p>
<p>
Our project is named as QuickActivity. QuickActivity is a self-service activity-posting and activity-attending platform. Everyone can post and attend activities in this platform. Activity organizers can post and edit their activities with sufficient information and anyone can print the activity detail as a PDF file. Anyone who logs in can choose to participate in any activities if he/she fits the requirements, especially the age requirement. Activity posters can export the information of the participants for a specific activity as a CSV file. Also, QuickActivity can prompt recommended activities according to user’s preference and provides REST API for activity details. Outdated activities can never be joined but still can be bookmarked. 
</p>
<p><b>
Every time when a user has registered, changed password, updated the profile, posted an activity, update an activity and joined an activity, QuickActivity will send an email to the user’s email inbox to confirm the actions that the user has just done.
</b></p>

<h3>A usable pair of username and password for the site:</h3>
<p>Username: qqq</p>
<p>Password: qqq</p>

<h3>Home page:</h3>
<ul>Achieved:
<li>
Use Bootstrap as Frontend framework, and implement the websites with bootstrap style css, js file.
</li>
<li>
Achieved the features of registration with <b>email confirmation</b>, login and logout. Register with username, email, password and birthday. Registration would fail with inappropriate or unformatted information. When the registration succeeds, the system would send a confirmation email to the email address of the new registered user. Login with username and password, login would fail with incorrect username and password.
</li>
<li>
Show the Most popular event, recently pubdated event and the expiring soon event in the carousel of the homepage. The title and brief introduction of each event are shown, and there's also a "View Detail" button links to the detail website of each event. 
</li>
<li>
List the 6 categories, sports, party, music, food&drink, arts, business and corresponding links to the activities of each category for users to look for.
</li>
<li>
A search bar that provides search services allowing users to search events by title and/or location and/or time and/or category. User can view those events in a list or in <b>calendar style</b>.
</li>
<li>
There is an "About Us" link to our about us page which gives information of the system and the developers of our team. The about us page has <b>background music</b>.
</li>
</ul>

<h3>Activity post page:</h3>
<ul>Achieved
<li>
This page is available when a user is logged in. 
</li>
<li>
The input of the information is user friendly. We use google map to help input the location and <b>datetime picker widgets</b> to help user input date time for the start time and end time of the activity.
</li>
<li>
Set several information required, and the event can not be posted without the essential informations.
</li>
</ul>
<ul>Unachieved
<li>
Set whether this activity is a repeated activity, such as repeated weekly, monthly or annually.
</li>
</ul>

<h3>Personal homepage:</h3>
<ul>Achieved:
<li>
This page is enabled when a user is logged in. After a user logs in, the button "Homepage" become available. The personal page would be showed after the user click the "Homepage" button.
</li>
<li>
In the personal homepage, the <b>exclusive recommendation</b> of events are recommended for the user <b>according to user's preference and the pouplarity of the events</b>. 
</li>
<li>
In the personal homepage, the events that the user is supposed to attend of this week are shown to <b>remind the user</b>.
</li>
<li>
View personal profile as well as edit and complete the information that is not recorded when registering such as email, phone number, address, gender and preferred categories.
</li>
<li>
Available to change the password.
</li>
<li>
View engaged activities. The user can view the activities he/she has participated in in list or <b>in calendar style</b>.
</li>
<li>
View posted activities. The user can modify the activities that he/she has posted and <b>which has not started yet</b>. The user can <b>export the participant list of the activity as a CSV file</b>. 
</li>
<li>
View favorited (bookmarked) activities, links to the detail of each of the activity.
</li>
</ul>
<ul>Unachieved
<li>
Set whether the user needs reminders for registered activities, recommended activities through email.
</li>
</ul>

<h3>Activity detail page:</h3>
<ul>Achieved
<li>
Logged-in user can join and bookmark the activity here.
</li>

<li>
Activities with strict requirements only show to appropriate users.<b>(According to the minimun age requirement of the activity)</b>
</li>
<li>
Show the poster of the activity, and total information such as activity name, organizer, time, place <b>(google map)</b>, ticket link, detailed description of the activity.
</li>
<li>
List important requirements for the activity such as <b>age requirement</b>.
</li>
<li>
Show the vacancy and capacity of the activity.
</li>
<li>
Show the name list of the users who decide to attend the activity. A user can set whether his/her name is able to be public in the personal homepage.
</li>
<li>
A user can choose to participate in the activity when he/she is logged in.
</li>
<li>
Users can <b>export the information of the activity in a pdf file</b>. 
</li>
<li>
Users can <b>make comments</b> to the activity.
</li>
<li>
Supports <b>REST API</b>. The REST API can be viewed in two ways. One is through URL, such as http://cmpt470.csil.sfu.ca:8006/final/events/1.json/ , the other way is through terminal, such as the command <code>curl -i -X GET -H "Accept: application/json" http://cmpt470.csil.sfu.ca:8006/final/events/1/ </code>.
</li>
</ul>
<ul>Unachieved
<li>
Users can judge whether a comment is helpful or not. 
</li>
</ul>
<h3>Techniques we use</h3>
<ul>Front-end
<li>
Bootstrap as front end framework
</li>
<li>
Use Javascript and jQuery to control components on the websites
</li>
<li>
Use customized CSS files
</li>
</ul>
<ul>Back-end
<li>
Use Python based Django as back-end
</li>
<li>
Use MySQL as database
</li>
</ul>