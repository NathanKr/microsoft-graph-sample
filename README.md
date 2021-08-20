<h2>Motivation</h2>
Play with microsoft graph API uisng .Net core SDK

<h2>Setup</h2>
The setup is done according to the credit below. Here are the main points
<ui>
<li>create an app in Azure portal - check figs/applications.png. I have chosen the name ".Net Core Graph Tutorial 1" for it but you can choose what ever you like</li>
<li>relate .Net core console app and ".Net Core Graph Tutorial 1" - the app in the Azure portal by means of Application ID - check figs/application_id_connection.png</li>
<li>the setup here uses dotnet user-secrets check <a href='https://docs.microsoft.com/en-us/graph/tutorials/dotnet-core?tutorial-step=3'>here</a>. This put sensitive info : app id and scopes locally on secets.json file , it does not change anything on azure. dotnet user-secrets is used in development ONLY !!!!!</li>
</ui>


<h2>Points of interest</h2>
<ul>
<li>I took gitignore file from <a href='https://github.com/dotnet/core/blob/main/.gitignore'>here</a></li>
<li>permissions are set nicely via 'dotnet user-secrets set scopes'</li>
<li>the user is asked to sign in and enter a code thus it does not fit machine to machine scenario</li>
</ul>


<h2>Working parts</h2>
<ul>
<li>i am able to get the token i.e choice 1</li>
<li>i am able to get Me with property DisplayName</li>
</ul>

<h2>not Working parts</h2>
<ul>
<li>i am NOT able to get Me with property MailboxSettings thus remark</li>
<li>i get exception on choice 2 (i did not continue to choice 3)</li>
</ul>


<h2>Credit</h2>
The code is based on <a href='https://docs.microsoft.com/en-us/graph/tutorials/dotnet-core'>this</a>