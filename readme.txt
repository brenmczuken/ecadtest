newsreader

we can do redirects on wpengine so I would suggest redirecting from http://www.services.zuken.com/news_reader/cadstar.asp to http://www.services.zuken.com/news-reader
I've just noticed that I have a redirection plugin installed which enables me to redirect anyway, so I don't need o do it with wpengine - althoguh having checked it it seems to be redirecting from localhost to wpengine so check whats going on here

I then need to add some pages news-reader and homepage and change home page settings - from dashboard click customise button. Make the current home page a static page. Make the news reader page the posts page and point the homepage to my new homepage which uses an empty page template

when the dns is changed for the sub domain we should then find that the site shows up under http://www.services.zuken.com/news-reader and the old url will redirect to there and include any arguments.

Add the number of posts change page to a plugin. This is better than having to go to a page and change it.

deleted the wpengine redirect so to redo it
source: ^/news_reader/testcadstar.asp/?$
destination http://services.zuken.com/

**************************************************************************
left to do
**************************************************************************
check with Roger what else needs to be moved over from the old server services.zuken.com and move it over

when we change the dns and go live with this I need to update the wordpress address and site address in settings to services.zuken.com