# agltest

Technology Used: jquery and Javascript

Since this is a simple application I  did not used any Javascript frameworks like AngularJS, Backbone, etc. As I discussed in the meeting I am very passionate about the pure Javascript here I am following conventional HTML, Javascript and for the REST integration I used jQuery.



Note that: I kept data.json if anybody want to run it locally to avoid crossdomain issue, for this index.html should be updated like below 
//var serviceUrl = "http://agl-developer-test.azurewebsites.net/people.json"; // serive Url 
var serviceUrl = "data.json";

Or wil be able to run in chrome browser by disabling chrome web security by locating chrome application and run the following command
C:\Program Files (x86)\Google\Chrome\Application>chrome.exe --user-data-dir="C:/
Chrome dev session" --disable-web-security
