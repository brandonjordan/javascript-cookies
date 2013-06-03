javascript-cookies
==================

This is a tutorial on how to use JavaScript cookies easily and efficiently


<h1>What's a Cookie?</h1>
A cookie is a variable that is stored on the visitor's computer. Each time the same computer requests a page with a browser, it will send the cookie too. With JavaScript, you can both create and retrieve cookie values.

Examples of cookies:

<li>Name cookie - The first time a visitor arrives to your web page, he or she must fill in her/his name. The name is then stored in a cookie. Next time the visitor arrives at your page, he or she could get a welcome message like "Welcome John Doe!" The name is retrieved from the stored cookie
<br/><li>Date cookie - The first time a visitor arrives to your web page, the current date is stored in a cookie. Next time the visitor arrives at your page, he or she could get a message like "Your last visit was on Tuesday August 11, 2005!" The date is retrieved from the stored cookie</li>

<h1>How to use</h1>

just put:

<code>&lt;script src="jscookies.js"&gt;&lt;/script&gt;</code>

in the <code>&lt;head&gt;</code> area of your code.

<h1>Create a Cookie</h1>

<code>setCookie("name of cookie","cookie value",365)</code>

<h1>Get a Cookie Value</h1>

<code>getCookie("name of cookie")</code>

You can use this like...

<code>var username = getCookie("username");</code>

<h1>Check for a Cookie</h1>

<code>function checkCookie()
{
var username=getCookie("username");
  if (username!=null && username!="")
  {
  alert("Welcome again " + username);
  }
else 
  {
  username=prompt("Please enter your name:","");
  if (username!=null && username!="")
    {
    setCookie("username",username,365);
    }
  }
}</code>

<h3>This requires no jQuery</h3>
