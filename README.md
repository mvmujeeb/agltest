# agltest

Dependancy: jquery -  https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js

Technologies Used: jquery and JavaScript

Since this is a simple application I  did not used any JavaScript frameworks like angular, Backbone, etc. As I discussed in the meeting I am very passionate about the pure JavaScript here I am following conventional HTML, JavaScript and for the REST integration I used jQuery.


AGL service mentioned in the instruction is in different domain so there will be cross domain error in the REST call.

You will be able to  run the code by doing any of the following options.

Option 1: Run the code in safari by making following settings
    1. safari -> preference -> advanced -> check "show develop menu in menu bar"
    2. safari -> develop -> check "disable local file restrictions"
See safari-settings.png for further details

Option 2: Run the index.html in chrome browser by disabling chrome web security. To disable web security need to locat chrome application and run the following command
C:\Program Files (x86)\Google\Chrome\Application>chrome.exe --user-data-dir="C:/Chrome dev session" --disable-web-security

Option 3: Run the code by doing a workaround in the ajax request, this is not recommended one.
replace dataType: "json",  
by dataType: "jsonp",

Option 4: Run the service locally (use data.json), for this index.html should be updated like below 

//var serviceUrl = "http://agl-developer-test.azurewebsites.net/people.json"; // serive Url 
var serviceUrl = "data.json";
