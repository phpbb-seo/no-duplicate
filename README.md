# no-duplicate
This extension will get rid of post URLs on phpBB3 Index, forums, and topics and use topic url instead, for the same purpose, but without duplicates. It will as well add a link to the last active topic in the forum index listing, above the regular last post one.


Notes :
Post URLs will now be composed of the topic URL they are posted in, on the correct page, with the html anchor #pxx as a suffix.

Example :
forum-title-fxx/topic-title-fyy.html#pzz

This mean that a message that would be posted in a thread and then moved in another one will see it’s url changing, which thanks to the zero duplicate extension is of no harm SEO wise, but the previous link to the post won’t link to it anymore in such case.

It does not add any SQL, just a LEFT JOIN on a query already being performed, this could still mean a bit more work but should not be a problem for server load.

To keep the post links absolute (postxx.html), you can omit the viewtopic.php code changes.
The last post links on index and forum will still be transformed, and it will be of no harm SEO wise, as long as you properly disallow post ulrs in your robots.txt.

<b>Working on phpBB 3.2 </b>

<b>Support Community:</b>
<br />www.phpbb-seo.org/community/
