# Mission to Mars

## Web Scraping with splinter and mongoDB 
### Week 13 USC Viterbi Data Analytics Bootcamp
### Student:  Tsering Sherpa
### Date:  05/11/2018 

<h3>Abstract:</h3>
<p>The purpose of this project is to scrape planet Mars information from five different websites to get a comprehensive and upto date understanding of  Mars.</p>
<p>Each of the site is used to gather information on different aspect of Mars which is then collectively presented as html</p>

<h3>Data Sources:</h3>
#### [Latest Mars News]https://mars.nasa.gov/news/
#### [Featured Image]https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars
#### [Latest Mars Weather]https://twitter.com/marswxreport?lang=en
#### [Mars Facts]https://space-facts.com/mars/
#### [Mars Hemispheres]https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars

<h3>Technology  Employed:</h3>
<ul>
<li><b>Python:</b>Python is used as the base language to manipulatae and interpreter between other technologies</li>
<li><b>MongoDB:</b>Database used as persistent storage of the scraping data</li>
<li><b>Splinter:</b>Tool used for scraping, (chromedriver) splinter driver for chrome utilized for this particular project</li>
<li><b>Flask:</b>Flask is used to create API endpoints that render html templates on user request</li>
<li><b>HTML/CSS/Bootsrap:</b>Used to create responsive front end that renders the scrape data</li>
</ul>

<h3>Summary:</h3>
<p>On first run the data is scraped from the above websites and then stored to MongoDB. After successful first scraping the information is rendered as html.</p>
<p>In case there is already a data present API endpoint renders html and has option to scrape new data. If we choose to scrape new data the data will be scraped and on success a succes html is renderd with link to render new information.</p>
<p>Only one set of data is stored in MongoDB and on each new retrival the old data is deleted so that the API endpoint always renders latest set of information scraped.</p>
