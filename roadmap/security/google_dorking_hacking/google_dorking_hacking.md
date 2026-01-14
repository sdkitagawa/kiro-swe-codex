## Google Dorking/Hacking

**Translations**

- [EN-US](./google_dorking_hacking.md)
- [PT-BR](./pt_br/google_dorking_hacking.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [What is Google Dorking/Hacking](#what-is-google-dorkinghacking)
- [What is it used for?](#what-is-it-used-for)
- [What are the filters?](#what-are-the-filters)
- [How does it work?](#how-does-it-work)
- [Homework](#homework)
    - [12 - Search for the map of Santa Catarina.](#12---search-for-the-map-of-santa-catarina)
    - [14 - Search for things to do in São Paulo.](#14---search-for-things-to-do-in-são-paulo)
- [Credits](#credits)
</details>

<br />

# What is Google Dorking/Hacking

Google Dorking/Hacking is basically a technique that consists of commands, or operators, that allow search results to be modified according to the type of data being searched for.
<br /><br />

# What is it used for?

Google Dorking/Hacking tem como objetivo atuar como um filtro detalhado de pesquisa que quando usando o [Google](https://www.google.com/), a própria ferramenta não trás acesso as esses recursos de forma fácil através da sua interface.

Through this technique, you can find specific things in different parts of a Google search result.

By looking at the image below, note the properties that a Google search result can present.
<br /><br />
<center>
        <img src="./assets/google_search_assets.png" alt="Properties of a Google search
" width="700" align="center" />
</center>
<br /><br />

# What are the filters?

There are several filters for carrying out Google Dorking/Hacking techniques, so before we start using them, let's understand what the filters are and how they work.

| **Parameters / Operators** | **Values** | **How to use** | **Usage Details** | **Effect** |
|---------------------------|-----------|---------------|-------------------|-----------|
| **Word 1 Word 2 Word 3** | **White House President** | `Thing Subject Object` | Enter the words you want to search side by side, separated by spaces | Finds the words **separately** in the same search result |
| **filetype**, **ext** | **filetype:PDF** | `filetype:Extension` or `ext:Extension` | Specify a file extension | Finds files of the specified type that Google can index |
| **intitle**, **allintitle** | **intitle:Nintendo** | `intitle:Thing` or `allintitle:Thing` | Search text in page titles | Returns pages whose titles match the text |
| **inurl** | **inurl:contact.php** | `inurl:Text` | Search text in URLs | Returns pages containing the text in the URL |
| **allinurl** | **allinurl:Cheap Games** | `allinurl:Words` | Search multiple words in URLs | Returns pages whose URLs contain all words |
| **intext** | **intext:Loves water** | `intext:Text` | Search exact text in content | Finds the text within page content |
| **allintext** | **allintext:I like juice** | `allintext:Text` | Search text across the whole query | Finds text in content, titles, and more |
| **site** | **site:facebook.com** | `Query site:Domain` | Restrict search to a site | Searches only within the specified site |
| **stocks** | **stocks:Amazon** | `stocks:Company` | Search company financial info | Returns public stock and finance data |
| **in**, **to** | **10 usd in brl** | `Value Currency in/to Currency` | Convert currencies | Converts one currency into another |
| **movie** | **movie:Kung Fu Panda** | `movie:MovieName` | Search movie info | Returns information related to the movie |
| **source** | **source:CNN** | `source:Publisher` | Search news sources | Returns results from Google News |
| **cache** | **cache:msn.com** | `cache:Site` | View cached page | Shows Google’s cached version |
| **location**, **loc** | **location:NY Tourist Spots** | `location:Place Query` | Search by location | Returns results for a specific location |
| **map** | **map:São Paulo** | `map:City` | Show a map | Displays a map of the city |
| **weather** | **weather:São Paulo** | `weather:City` | Check weather | Shows weather info |
| **link** | **link:facebook.com** | `link:Site` | Search backlinks | Returns pages related to the domain |
| **related** | **related:harvard.edu** | `related:Site` | Find similar sites | Shows related websites |
| **info**, **id** | **info:"Twitter"** | `info:"SiteName"` | Get site info | Shows information about a site |
| **AND**, **&** | **Jennifer Lopez AND Ja Rule** | `Thing1 AND Thing2` | Combine terms | Finds both terms together |
| **OR** | **Alyne OR Allyne** | `Thing1 OR Thing2` | Alternate terms | Finds either term |
| **+** | **Fast Furious +Tokyo** | `Thing +Thing` | Add a term | Similar to **AND**; also adds numbers |
| **-** | **Mark Zuckerberg -Facebook** | `Thing -Thing` | Exclude a term | Removes results containing the term |
| **\*** | **mac * OS** | `Word * Word` | Wildcard between words | Finds words with one word in between |
| **/** | **14 / 2** | `Number / Number` | Division | Divides numbers |
| **sin, cos, tan** | **sin(pi/6)** | `Operator(Value)` | Trigonometric functions | Calculates trig values |
| **sqrt()** | **sqrt(4)** | `sqrt(Number)` | Square root | Returns the square root |
| **% of** | **17% of 500** | `Percent% of Value` | Percentage calculation | Returns percentage |
| **~** | **Angelina Jolie ~beautiful** | `Subject ~Keywords` | Synonym search | Searches for related terms |
| **""** | **"Exactly this"** | `"Exact phrase"` | Exact match | Finds the exact phrase |
| **()** | **(A) AND (B)** | `(Query) Operator (Query)` | Group searches | Improves accuracy |
| **X..Y** | **2010..2024** | `Start..End` | Range search | Filters by numeric range |
| **define** | **define:Crux** | `define:Word` | Word definitions | Returns definitions |
| **@** | **@youtube Astro Politics** | `@platform query` | Social search | Searches content on platforms |
| **Currency symbols** | **PlayStation 2 ¥** | `Product CurrencySymbol` | Price lookup | Finds prices in the currency |
| **filter** | **filter:1** | `filter:0 or 1` | Duplicate control | Includes/excludes duplicates |
| **AROUND()** | **AROUND(2) family** | `AROUND(N) Term` | Proximity search | Finds nearby terms |
| **timer** | **timer for 30 minutes** | `timer for Time` | Countdown | Creates a timer |
| **flip a coin** | **flip a coin** | Phrase | Coin flip | Flips a coin |
| **roll a dice** | **roll a dice** | Phrase | Dice roll | Rolls a die |
| **random number** | **random number 10 to 120** | Phrase | Random generator | Shows a random number |
| **as_epq** | **phrase as_epq** | `Text as_epq` | Exact phrase query | Forces exact matching |
| **as_filetype** | **as_filetype:PDF** | `Search as_filetype:ext` | File filtering | Same as `filetype` |
| **as_ft** | **as_ft:i** | `as_ft:i/e` | Include/exclude | Controls file inclusion |
| **as_occt** | **as_occt:title** | `as_occt:part` | Page section | Searches specific site parts |
| **as_sitesearch** | **as_sitesearch:facebook.com** | `as_sitesearch:Site` | Site filtering | Same as `site` |
| **as_dt** | **as_dt:e** | `as_dt:i/e` | Domain filtering | Include/exclude domains |
| **as_qdr** | **as_qdr:m3** | `as_qdr:Time` | Date filter | Filters by last update |

<br /><br />


# How does it work?

Google Dorking/Hacking works through search filters that are given as commands, for example, let's imagine a hypothetical scenario where you want to find information about `Larry Page` and `Sergey Brin` the founders of Google, but you want to find information about them on a specific site, the site we're going to use as an example is Futurism, which is a digital media company that brings constant news about science and technology.

So, let's think about it this way:

**1 -** Let's identify our subjects or "targets";

**2 -** Let's think about where we want to find information about our subjects/targets;

**3 -** Let's build a logical sentence using logical commands similar to programming, using Google Dorking/Hacking filters;.

**Note:**
> Keeping these steps in mind, I will give an example of how we can achieve what we want

<br />

**Question 1:** Who is/are my subject(s)/target(s)?  
**Answer 1:** Sergey Brin and Larry Page (together, not just one and not just the other);

**Question 2:** Where do I want to search for information about my subject(s)/target(s)?  
**Answer 2:** On the site `https://futurism.com/`;

**Question 3:** How to build this logically using Google Dorking/Hacking filters.  
**Answer 3:** "sergey brin" AND "larry page" site:https://futurism.com/
<br /><br />

# Homework

**All exercises below must be done using the Google search tool**.

**1** - Search for information about the series iCarly in a filtered way, finding results that come only from the official distributor of the series (Paramount Plus).  
**A:**  

**2** - Using Google's image tab, search for images of the series Hannah Montana that are in the `PNG` format:  
**A:**  

**3** - Search for the user "iruletheworldmo" within the Twitter platform without using the `site` operator.  
**A:**  

**4** - Search for the definition of the following words "Noctis", "Lucis", "Caelum" and "Nox"  
**A:**  

**5** - Check how the financial summary of the stocks of the companies NVIDIA, AMD, Intel and Microsoft is doing.  
**A:**  

**6** - Search for the movie "The Da Vinci Code"  
**A:**  

**7** - Search for information sources with this news title "Microsoft 365 anti-phishing feature can be bypassed with CSS" on the BleepingComputer platform without using the `site` operator.  
**A:**  

**8** - Search for the current price of the iPhone 17 in Euro, Yen and Dollar.  
**A:**  

**9** - Try to search in Google Cache for the page "narutoproject.com".  
**A:**  

**10** - Search for pages linked to the domain `thatsthefinger.com`.  
**A:**  

**11** - Search for pages related to the Facebook domain (`facebook.com`).  
**A:**  

### 12 - Search for the map of Santa Catarina.
**A:**  

**13** - Search for the weather in Toyokawa.  
**A:**  

### 14 - Search for things to do in São Paulo.
**A:**  

**15** - Search for information about the company `GRAVITY Interactive` within some site.  
**A:**  

**16** - Search for pages that contain the words `Ted's caving journal` in their title.  
**A:**  

**17** - Search for pages that have a page called `contact` with the `php` extension on their site.  
**A:**  

**18** - Search for pages that contain the following phrase in their text `get in touch`.  
**A:**  

**19** - Search in a general way (any part of a search result, which can be title, description, etc) for EXACTLY this phrase `Never argue with an ignorant person. He will drag you down to his level and beat you with experience.`.
**A:**  

**20** - Search for Jéssica Canedo, we want results related to Digital Bank or Mynd and report what you found.  
**A:**  

**21** - Search for Intel processors that are not from the i3 and i7 generation.  
**A:**  

**22** - Do a search for everything you can about A858 from 2011 to 2024.  
**A:**  

**23** - Perform math operations of `addition`, `subtraction`, `multiplication`, `division` and `square root` using Google.  
**A:**  

**24** - Convert R$ 300 (reais) into $ (US dollar).  
**A:**  

**25** - Search for your name and look for documents with the extensions `PDF`, `DOCX`, `DOC`, `PPTX`, `PPT`, `XLS`, `XLSX` and `TXT`.  
**A:**  

**26** - Search for the movie `The Butterfly Effect`.  
**A:**  

<br />

# Credits

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
