# VirusTotal-Searches
Tricks to perform searches in VirusTotal premium or free.
The following is a list of searches that can be used in the reconnaissance phase using VT, 
on the other hand if you have access to a paid account it is possible to 
find exposed information during your attack surface analysis.

Some basics, is perform a search with the principal domain related with your 
target, in  VT Hunting module, like:

 --->   *mydomainorganization.com*

With this search in in VTHunting and  the relations tab  you will be able to see all the subdomains associated with a organization,
this search is useful in the free and paid version.

As a result you will get the following:

a.mydomainorganization.com 

b.mydomainorganization.com

c.mydomainorganization.com

d.mydomainorganization.com
.
.
.
g.mydomainorganization.com
h.mydomainorganization.com
i.mydomainorganization.com


and more...

From here the paid version can help you get more information.

If you pivot on some of the domains, like

--> *b.mydomainorganization.com*

You will be able to find all the urls associated with that domain, some of these urls can be juicy,
because they are URLSs that are not indexed by internet search engines,
like google or bing.

In my experience hunting all kinds of information, these URLs are indexed in VT because legitimate
users who access certain web applications send them in VT as if it were an antivirus.

***Some of these URLs are only visible when a user enters a platform that requires a username and password. :D***

On other occasions, the security solutions of the organizations upload these URLs, automatically to VT.

let's go back to   --> 
  **b.mydomainorganization.com

If you look in the relationships tab for this subdomain you will find things like.

	**https://b.mydomainorganization.com/Documents?Confidential={documentID}&Date=19/01/2021&IdStore=1&Download=1&Event=6


Or an infinity of URLs that could present interesting parameters for web parameter tampering or XSS etc.





  



