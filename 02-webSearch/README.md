
Architecture Of Search Engine
If we talk about the architecture or the framework of a search engine, it can be described in three main components –

• <a href="https://www.geeksforgeeks.org/what-is-a-webcrawler-and-where-is-it-used/">
  Web crawlers</a> – As the name suggests these acts as spiders which crawl all over the 
  web to collect required information. These are special bots that search throughout the 
  internet and accumulates data using various links.

• Database – It is a collection of data which is gathered by the web crawlers after searching 
  throughout the world wide web.

• Search Interface – It provides a medium or interface for users so that they can access 
  and search on the database for required information.

How queries are processed in search engine?
Whenever we search anything on the search engine, it only takes a second or two for the output generation. However, a lot goes on in the backend. Indexing and Querying are two essential components behind the processing of a search engine. They are like the building blocks of search engines. Let’s take a look at these processes -

Indexing
• The indexing process begins with web crawling where the so-called spiders crawl across 
  the world wide web and collect data.

• The data collected is stored in the form of a database for the process of indexing. 
  This is also termed as text acquisition.

• Then the collected data is broken down into tokens or keywords. These tokens are used 
  by the search engine in creating indexes. Each keyword is associated to a particular 
  document and through indexing the data becomes organized and it helps the search 
  engine to quickly retrieve a particular information.

Querying
• When a user searches something on the search engine a query input is generated.

• Then the search engine parses the generated query and searches at the indexes for 
  the matching documents.

• Using a ranking algorithm, the search engine ranks the documents based on their 
  relevance. Finally, the generated list is presented to the user with most relevant 
  results on the top.

Search Engine Advantages:
• Search engines have made it possible to navigate through the internet. Even a person 
  without any technical knowledge is able to use a search engine for solving a query.

• The quick and efficient responses of search engine make it easier for a user to 
  immediately get result for their search.

• A search engine not only supports text results but also results like images, videos, 
  maps, documents and various other formats, hence offering users a one stop solution.

• In today’s time people are using search engines not only for technical purposes but 
  also for researches, educational purposes and even in day-to-day life because of its 
  diversified result generation.

• The user-friendly interface, organized results, customization features and diversity 
  of search results makes search engines one the most essential tool for surfing on internet.

Examples Of Popularly Used Search Engines
In today's time Google is the most widely used search engine, however there are several 
other popular search engines being used. Some of the popular search engines are listed below:

• Google - Founded in 1998 by Larry Page and Sergey Brin, Google is the most popularly 
  and widely used search engine. It has an attractive an user-friendly interface with a 
  versatile library of features which makes it first choice for maximum users when it 
  comes to search engines.

• Bing - Founded in 2009 by Microsoft, Bing is quite similar to other search engines. 
  It also allows users to search through images.

• Yahoo - Founded in 1994 by Jerry Yang and David Filo, Yahoo was among the earliest 
  used search engines. However, its popularity has declined over time. Earlier Yahoo 
  offered a platform called "Yahoo answers" where users could ask or answer various 
  questions.

• Baidu, DuckDuckGo and Yandex are some other popular emerging browsers in today's time.


Web Search Bar Implementation Using Javascript Conditional Flow
Last Updated : 25 Jul, 2024
Given a list of items and the task is to filter through the items and return the best match using the search bar. There are several approaches to implement this but, we will be using a simple if-else statement to implement our search bar.

Approach:
Create a folder called gfgSearchBar.
Open the folder in your desired IDE or IDLE.
Create a html file called approachOne.html
Paste the below code into the html file.

```
<!DOCTYPE html>
<html lang="en">
  
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Search Bar</title>
  <style>
    #searchBar {
      font-size: 20px;
    }
    .movieWrapper {
      display: none;
      text-align: left;
      margin-left: 20%;
    }
    .search {
      text-align: center;
      padding-top: 15%;
      width: 30%;
      margin-left: 35%;
    }
    h1 {
      margin-bottom: 0%;
    }
    p {
      margin-top: 0%;
    }
  </style>
</head>

<body>
  <div class=search>
    <h1>GFG Movie Search</h1>
    <p>item search example</p>
    <input type="text" id="searchBar" placeholder="Search for a movie...">
      <div class="movieWrapper">Inception</div>
      <div class="movieWrapper">Interstellar</div>
      <div class="movieWrapper">The Dark Knight</div>
      <div class="movieWrapper">Memento</div>
      <div class="movieWrapper">Dunkirk</div>
  </div>

  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const getSearchBar = document.querySelector('#searchBar');
      const getAllMovies = document.querySelectorAll('.movieWrapper');

      getSearchBar.addEventListener('keyup', (e) => {
        getAllMovies.forEach(movie => {
          if (movie.innerText.toLowerCase().includes(e.target.value.toLowerCase())) {
            movie.style.display = 'block';
          } else {
            movie.style.display = 'none';
          }
        });
      });
    });
  </script>
</body>
  
</html>
```

Output:

Explanation of the code inside the script tag:

document.addEventListener(‘DOMContentLoaded’); This is a document event that gets executed 
or triggered immediately the html file gets loaded on your browser. Operations inside this 
event block doesn’t get executed until the html file is completely loaded to the DOM.
const getSearchBar = document.querySelector(‘#searchBar’); We simply got the search bar 
element and pass it to getSearchBar variable.
const getAllMovies = document.querySelectorAll(‘.movieWrapper’); We simply got all the 
movie divs and pass then to getAllMovies variable. Note that getAllMovies is a Nodelist 
of elements which is an Array look alike not an Array.
getSearchBar.addEventListener(): We simply added a keyup event listener to the search bar.

```
getAllMovies.forEach(movie => {
    if (movie.innerText.toLowerCase()
    .includes(e.target.value.toLowerCase())) {
        movie.style.display = 'block';
        return movie;
    }
    else {
        movie.style.display = 'none';
    }
});
```

This block of code simply means the user types into the search bar are present in the 
movie text content, then style that movie box to be displayed in blocks and return all 
of them. Else don’t return any movie block.

Difference between Search Engine and Web Browser
Last Updated : 12 Jul, 2025

<image>

Search Engine: A search engine is a kind of website through which users can search the 
content available on the Internet. For this purpose, users enter the desired keywords 
into the search field. Then the search engine looks through its index for relevant web 
pages and displays them in the form of a list. The Internet is a huge source of information 
& resources and to access the resource from the Internet there are some kinds of software, 
this software is known as a Search Engine. Some of the popular ones are Google, Bing, 
Yahoo, Duckduckgo, Baidu, etc. 

There are three main components of the Search engine:

Crawler: Crawlers are software programs sometimes referred to the bots. It regularly 
scans the websites automatically for URLs, keywords, and links to discover the new 
updates. The crawler can follow the links present on some other webpage.
Index: As we know, the Crawler continuously scans the websites, it develops an index of 
URLs, links, and keywords to make the search results more effective.
Search Algorithm: The search algorithm is the complete mechanism behind the whole 
searching process. It is working by searching for the index and finding the most 
suitable web pages by matching keywords that are searched by the users.
Web Browser: The web browser is an example of application software that is developed 
to retrieve and view the information from web pages or HTML files present on the web 
servers. The first web browser was invented by Sir Tim Berners-Lee in 1990 and the 
very first graphical web browser was developed in 1993 and is named the mosaic. After 
that, various web browsers were developed. Some of them are navigator which is 
developed by Netscape communication, Microsoft Edge, Google Chrome, Mozilla Firefox, 
Opera, and Apple safari. 

The main characteristics of a Web Browser are:

It consists of Graphical User Interface.
It contains the search box where the user can type the address or URL.
Page style can be static or dynamic. It depends upon the interactivity and the formatting.
TCP/IP and HTTP protocols are used by web browsers.
Difference between Search Engine and Web Browser:

<table>
  <thead>
    <tr>
	  <th>S. No.</th>
      <th>Parameters</th>
      <th>Search Engine</th>
	  <th>Web Browser</th>
	</tr>
  </thead>
  <tbody>
	<tr>
	  <td>1.</td>
	  <td>Definition</td>
	  <td>A search engine is used to find the information in the World Wide Web and 
	    displays the results at one place by returning web pages available on internet.</td>
      <td>Web Browser uses the search engine to retrieve and view the information 
	    from web pages present on the web servers.</td>
	</tr>
	<tr>
	  <td>2.</td>
	  <td>Usage</td>
      <td>Search engine is intended to gather Information regarding several URL's and to maintain it.</td>
      <td>Web Browsers are intended to Display the web page of the current URL available at the server.</td>
	</tr>
	<tr>
	  <td>3.</td>
      <td>Installation</td>
	  <td>Search Engine need not to be installed on our system (i.e. comes as default).</td>
	  <td>Many Web Browsers can be installed on our system.</td>
	</tr>
	<tr>
      <td>4.</td>
	  <td>Accessibility</td>
	  <td>The search engine is accessed through a web browser.</td>
	  <td>Typically, all devices are supported.</td>
	</tr>
	<tr>
      <td>5.</td>
	  <td>Components</td>
	  <td>The Search Indexer, Crawler, and Database are the three essential components of 
	    a search engine.</td>
	  <td>A web browser uses a graphical user interface to help users have an interactive 
	    online session on the Internet.</td>
	</tr>
	<tr>
      <td>6.</td>
	  <td>Database</td>
	  <td>A search engine contains its own database.</td>
	  <td>No database is required in Web browser. It contains only cache memory to store 
	    cookies as well as browsing history until we remove it from our system.</td>
	</tr>
	<tr>
      <td>7.</td>
	  <td>Dependency</td>
	  <td>A search engine is not required to open the browser. This means that the search 
	    engine is reliant on the browser.</td>
      <td>A browser is required to open a search engine. This means that the browser is 
	    not reliant on the search engine.</td>
	</tr>
	<tr>
      <td>8.</td>
      <td>History</td>
      <td>Unless you actively clear this data or use a private browsing mode, browsers 
	    will retain your browsing history, cookies, and cache in memory.</td>
      <td>Typically, search engines acquire information on their users and their search 
	    queries. Some search engines, such as DuckDuckGo, do not gather user information.</td>
	</tr>
	<tr>
      <td>9.</td>
      <td>Advantages</td>
      <td>The major Advantages of using search engines are to Get the Consumer Trust, 
	    Trackable Results, Generates Targeted Traffic, Sustainable Clicks and Grow Your 
		Small Business.</td>
      <td>The major Advantages of using web browser are open standards, security sandbox, 
	    Robust GUI and Simple networking.</td>
	</tr>
	<tr>
      <td>10.</td>
      <td>Disadvantages</td>
      <td>The disadvantages of using search engines are difficult Of Competitive Keywords, 
	    Changing Algorithms and Results are Not Guarantee.</td>
      <td>The disadvantages of using web browsers are slow down with the new version and 
	    no-add on support.</td>
	</tr>
	<tr>
      <td>11.</td>
	  <td>Examples</td>
	  <td>Example of famous search engines are: Google, Yahoo, Bing, DuckDuckgo, Baidu 
	    Internet Explorer.</td>
      <td>Some of the widely used web browsers are: Mozilla Firefox, Netscape Navigator, 
	    and Google Chrome.</td>
	</tr>
  </tbody>
</table>


