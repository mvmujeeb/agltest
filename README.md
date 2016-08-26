# agltest

Technology Used: jquery and Javascript

Since this is a simple application I  did not used any Javascript frameworks like AngularJS, Backbone, etc. As I discussed in the meeting I am very passionate about the pure Javascript here I am following conventional HTML, Javascript and for the REST integration I used jQuery.

agl service mentioned in the instruction is in different domain so there will be crossdomain error in the REST call.
Will be able to  run the code by doing following options

Option1: Run the index.html in chrome browser by disabling chrome web security. To disable web security need to locat chrome application and run the following command
C:\Program Files (x86)\Google\Chrome\Application>chrome.exe --user-data-dir="C:/Chrome dev session" --disable-web-security

Option2: Run the code by doing a workaround in the ajax request, this is not recomended one.
replace dataType: "json",  
by dataType: "jsonp",

Option3: Run the service locally (use data.json), for this index.html should be updated like below 
//var serviceUrl = "http://agl-developer-test.azurewebsites.net/people.json"; // serive Url 
var serviceUrl = "data.json";
