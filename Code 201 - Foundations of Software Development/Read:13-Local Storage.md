# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS :

* Cookies is used to store littel amount of data for priesent local data .

##  but they have three potentially dealbreaking downsides:
1. they are slowing your web page becaues they nned to be included in each http request and thats mean they need to send data over and over.

2. beacause they need to send your data for each http reqest that meen thet can be hacked and that make asecurity problems.
(unless your entire web application is served over SSL).

3. cookies are not enough to store data and be usfull (4kb) but they are big to show slow effect on your web page.

# What we really want is
* a lot of storage space
* on the client
* that persists beyond a page refresh
* and isn’t transmitted to the server


 * userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.


 # html5 local storage : 
 *“HTML5 Storage”* 
 * is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” 

## So what is HTML5 Storage? 

* Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

# HTML web storage provides two objects for storing data on the client:

1. window.localStorage - stores data with no expiration date
2. window.sessionStorage - stores data for one session (data is lost when the browser tab is closed).

![html5 local storage](https://theburningmonk.com/wp-content/uploads/2010/12/image42.png)

![html5 local storage](https://theburningmonk.com/wp-content/uploads/2010/12/image42.png)