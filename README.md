# Google Dorking (Google Hacking)

- Google Dorking is a technique used for specific search queries that use Google’s search operators, combined with targeted parameters to find specific information.

- It is used by hackers to find the information exposed accidentally to the internet. For example, log files with usernames and passwords or cameras, etc.

- Google Dorking is not hacking itself. Google Dorking is a technique that comes in handy in one of the phases of hacking, i.e., Information Gathering, and this is the most important phase of hacking. There are five phases of hacking, i.e., reconnaissance, scanning, gaining access, maintaining access, and clearing tracks. Google Dorking is used in the starting phases where hackers try to get all the information linked to any specific organization or an individual. After getting all information then hackers pick out the information they need for the next phases.


## How it works

Dorking can be employed across various search engines like Google, Bing and Yahoo. They accept a search term  and return matching results. But search engines are also programmed to accept more advanced operators that refine those search terms. An operator is a key word or phrase that has particular meaning for the search engine. Operators include things like “inurl”, “intext”, “site”, and so on.

## Syntax 

`operator:search_term`

- Notice that there is no space between the operator, the colon and the search term. If a space is used before the colon, Google will use your intended operator as a search term.

- If the search term contains multiple words, they should be surrounded by quotation marks.

---------------------------------------------------

# Basic Search Operators

|Operator|Description|Example|
|--|--|--|
|**"	"**|Limit the results to the ones containing the **exact phrase** in their title, description or body.|`“Google dorks"`|
|**+**|Force an exact-match search on a single word or phrase. You can do the same thing by using double quotes around your search.|`logic +gates`|
|**OR** <br> **\|**|This will show results for keyword1 or keyword2 or both. |`mango OR banana` <br> `mango \| banana`|
|**AND** <br> **&**|This will show results for keyword1 and keyword2. It doesn’t really make much difference for regular searches, as Google defaults to “AND” anyway. But it’s very useful when paired with other operators.|`apple & iphone`|
|**NOT** <br> **-**|Exclude the term (or a whole operator) by putting the minus symbol in front of it.|`python -animal`|
|**\***|Acts as a wild-card character that will match any word or phrase.|`How to * sites` will show you all the results like “how to…” design/create/hack, etc… “sites”|
|**.**|Used to include single character wirldcards.|`.eb`|
|**( )**|Group multiple operators.|`elon musk (site:www.facebook.com \| site:www.twitter.com )`|
|**~**|Include synonyms. Doesn’t work, because Google now includes synonyms by default.|`~apple`|

----------------------------------------

# Advanced Search Operators

|Operator|Description|Example|
|--|--|--|
|**define**|Provides the definition of a term as a result|`define:git`|
|**filetype**|Searches for certain file type.|`filetype:pdf` will search for all the pdf files in the websites.|
|**ext**|It works similar to filetype.|`ext:pdf` finds pdf extension files.|
|**site**|This limits the search to a **specific site only**. Example: site:abc@d.com will limit search to only abc@d.com.|`site:www.github.com`|
|**link**|Searches for **external links** to pages.|`link:www.asu.edu`|
|**related**|Finds web pages that are similar to the specified web page.|`related:www.github.com`|
|**intitle**|Shows results that include the searched words in the title.| `intitle:keyword tools` will return results with 'keyword' in the title, but 'tools' can be anywhere else on the page - including the title. If 'tools' is not mentioned on the page or in the title but 'keyword' is in the title, then it will still return that page.|
|**allintitle**|Similar to “intitle,” but only results containing all of the specified words in the title tag will be returned.|`allintitle:keyword tools`  will return results with both words used in the page titles. It's like an exact phrase match search for page titles.|
|**intext**|This will search content of the page. This works somewhat like plain google search.|`intext:apple`|
|**allintext**|Returns only those pages which include the exact phrase in the text on the page.|`allintext:apple iphone 11 pro`|
|**inurl**|Searches for specified term in the URL.|`inurl:hackingarticles`|
|**allinurl**|Only shows results that include all the searched words in the URL.|`allinurl:flappyBird`|
|**daterange**|Find results from a certain date range. Uses the [Julian date format](http://www.longpelaexpertise.com/toolsJulian.php)|`daterange:11278-13278`|
|**numrange**|Locates specific numbers in your searches.|`numrange:1-20`|
|**before/after**|Finds results from a certain date range (YYYY-MM-DD).|`before:2000-01-01  after:2001-01-01` <br> `top 10 * after:2018-12-31`|
|**location**|Returns only pages from the location you specify.|`queen location:egypt`|
|**map**|Forces Google to show map results for a locational search.|`map:egypt`|
|**in**|Converts one unit to another. Works with currencies, weights, temperatures, etc.|`$50 in egp `|



> Google changes its search operators from time to time; it's likely that some of these won't work.


--------------------------------------------------------

# Examples of Google Dorking

- `filetype:xls “house prices” and “London”` —— This dork will bring you all xls files that contain the words “house prices” and “London”.

- `site:github.com filetype:pdf` —— This dork will bring you all publicly-accessible PDF files on the github website.

- `report site:github.com filetype:pdf` —— This dork will bring you all publicly-accessible pdfs with the word “report” on the github website.

-----------------------------------------------------------
 
# GHDB (Google Hacking Database)

- In order to understand advanced implementation of these dorks, see the [GHDB](https://www.exploit-db.com/google-hacking-database). 

- GHDB is an open-source project that provides an index of all known dorks. The project started in 2002 and is currently maintained by Exploit-DB.
---------------------------------------------------------------------

**Resources :**
- https://www.hackingloops.com/google-dorks/
- https://exposingtheinvisible.org/en/guides/google-dorking/
