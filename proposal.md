<h2>QuickActivity</h2>
<h3>Idea description:</h3>
<p>
QuickActivity is a self-service activity-posting and activity-attending platform. Everyone can post and attend activities in this platform. Activity posters can create their distinct type of activities, such as sports activity or musical activity. Anyone who logs in can choose to participate in any activities if he/she fits the requirements.  Activity posters can import the information of the participators for a specific activity as an Excel file. Also, QuickActivity can prompt recommended activities according to users’ history, preference and similar users’s history and preference.
</p>

<h3>Home page:</h3>
<ul>
<li>
Appearance is similar to http://cmpt470.csil.sfu.ca:8006/demo/home.html .
</li>
<li>
User registration with email confirmation and login. Register with profile such as email, birthday and preference. Login button will be replaced with a logout button when a user logs in.
</li>
<li>
List the newest, the most popular and the expiring soon activities.
</li>
<li>
List the categories such as sports, parties and foods of activities for users to look for.
</li>
<li>
List top 6 recommended activities for the user when he/she logins in based on the user’s history, preference and similar users’ history and preference. The activities which are already full are never recommended.
</li>
<li>
A link to view all the activities with different sort choices such as sorting by time and place, and with different view choices such as journal and calendar. Activities with strong restrictions such as age only show to appropriate users. A user can favorite (bookmark) the activities he/she interested in.
</li>
<li>
A post activity button is available when a user logs in.
</li>
<li>
Search activities by name, category, date and location.
</li>
</ul>

<h3>Activity post page:</h3>
<ul>
<li>
This page is used when a user wants to post an activity. 
</li>
<li>
Set the information of the activity, i.e., activity name, time, place (with Google map), the name and contact information of the organizer, the capacity and the detailed description of the activity.
</li>
<li>
Set strict requirements such as age requirement for the activity.
</li>
<li>
Set whether this activity is a repeated activity, such as repeated weekly, monthly or annually.
</li>
</ul>

<h3>Personal homepage:</h3>
<ul>
<li>
This page is enabled when a user logs in. After a user logs in, the button "Profile" become available. The personal page would be showed after the user click the "Profile" button.
</li>
<li>
View/Edit personal information such as email, password, phone number, interested locations, preferred categories and gender.
</li>
<li>
View participated activities. The user can rate the activities he/she has participated in.
</li>
<li>
View activities posted by the user. The user can export the information of the participants for the activity as an Excel file. The user can modify the activities that he/she has posted and which is not closed.
</li>
<li>
View favorite (bookmarked) and coming (registered) activities. Activities are in reverse time order. Activities here can be shown both in journal style and calendar style, like SFU Canvas.
</li>
<li>
Set whether the user needs reminders for registered activities, recommend activities or some changes in his/her profile on the personal homepage or through email.
</li>
</ul>
<h3>Activity detail page:</h3>
<ul>
<li>
Appearance is similar to http://cmpt470.csil.sfu.ca:8006/demo/detail.html .
</li>
<li>
Activities with strict requirements only show to appropriate users.
</li>
<li>
Show the poster of the activity, and total information such as activity name, organizer, time, place (google map), fee, detailed description of the activity.
</li>
<li>
List important requirements for the activity such as age requirement.
</li>
<li>
Show the vacancy and capacity of the activity.
</li>
<li>
Show the name list of the users who decide to attend the activity. A user can set whether his/her name is able to be public in the profile.
</li>
<li>
A user can choose to participate in the activity when he/she logs in.
</li>
<li>
Provide the service of printing the activity page.
</li>
<li>
Users can make comments to the activity. (This will be implemented if time allows.)
</li>
<li>
Users can judge whether a comment is helpful or not. (This will be implemented if time allows.)
</li>
</ul>
<h3>Implementation:</h3>
<p>
The architecture for the web site is a 3-tier architecture:
<ul>
<li>
Client (all sorts of browsers including the browsers on mobile, tablet, laptop and desktop): Bootstrap;
</li>
<li>
Middleware: Python-based Django web framework to develop the web applications;
</li>
<li>
Database: MySQL database engine.
</li>
</ul>
</p>
<p>
Some of Django’s applications we are going to use: 
<ul>
<li>
Django.db.models.Model: Define our database model;
</li>
<li>
Django.conf.urls: Design the URLs for the web app;
</li>
<li>
Django.contrib.admin: Use Django admin site to manage users and activity contents.
</li>
</ul>
</p>
<p>Security:  
<ul>
<li>
Django template system to tackle XSS attacks.
</li>
<li>
Django.contrib.csrf package protects against CSRF attacks.
</li>
</ul>
</p>