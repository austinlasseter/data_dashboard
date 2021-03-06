# World Bank Example

Video: World Bank API https://youtu.be/nygWkgUQNfo
Video: Code Walk-Thru https://youtu.be/AkqO534YooE

What is an API?
Instead of downloading World Bank data via a csv file, you're going to download the data using the World Bank API.

API is an acronym that stands for application programming interface. API’s provide a standardized way for two applications to talk to each other. For this project, the applications communicating with each other are the server application where World Bank stores data and your web application.

If you wanted to pull data directly from the World Bank’s server, you’d have to know what database system the World Bank was using. You’d also need permission to log in directly to the server, which would be a security risk for the World Bank. And if the World Bank ever migrated its data to a new system, you would have to rewrite all of your code again.

The API sits between your web app and the World Bank server. And the API allows you to execute code on the World Bank server without getting direct access.

All sorts of companies have public facing APIs including Facebook, Twitter, Google and Pinterest. You can pull data from these companies to create your own applications.

In the next section, you’ll get practice using Python to pull data from the World Bank API. This will set you up for creating the web app with data from the API instead of using data from a csv file.

APIs Besides the World Bank
All types of companies have APIs. Some of these APIs are only for internal company use while other APIs help the public consume data. A few examples of public APIs include the Twitter API, the Google Maps API, the Facebook Graph API, and the US Government Data APIs.

In addition, oftentimes you can find open source libraries or development kits for connecting to an API. For example, here is an open source Python development kit for the Facebook Graph API.

Some APIs might be used for pulling data from a database. But other APIs are for adding data to a database. For example, you might make an application that automatically tweets the current weather. In that case, you would use the Twitter API to post a tweet, which in reality inserts a tweet into Twitter's database.

Using an API
In the next few parts of the lesson, you'll see how to use the World Bank API. This API is relatively straightforward to use. Each API, however, will have a different set up and only allow you to take certain actions. In general, you send a request via a web url that specifies the information you want. You receive data back typically in XML or JSON.

The XML standard was developed in the 1970s and 1980s and soon became a common way to transfer data over the web. JSON was developed in the mid 1990s. Over time, JSON has increased in popularity relative to XML perhaps because JSON is easier to parse.

Some APIs require authentication; essentially the company with the API gives you 'credentials' so that they can track how you are using the API and ensure you have the proper permissions.

Some APIs might let you extract data from a database. Other APIs might even let you insert data into a database depending on the use case. Most APIs include extensive documentation so that you can figure out how to use APIs.

If you ever can’t figure out how to use an API, search online for examples. You can search for something like, “Examples for using the World Bank API” or “Examples for using the Facebook API”.

Move on to the next section to see how to use the World Bank API and incorporate it into a web app.

## Code Walk-Through
Video: Code Walk-Thru https://youtu.be/AkqO534YooE

github: https://github.com/udacity/DSND_Term2/tree/master/lessons/WebDevelopment/AdvancedDataDashboardCode/world_bank_api_dashboard

How the Filter Works
This version of the web app has a filter made with a form. When you check the boxes on the form and click submit, the form gets submitted to the index.html page. It's essentially a circle where the index.html loads, the form gets submitted to index.html itself, and then index.html loads again. With a web form, you could also submit the form to a different web page.

On the back-end, routes.py can access the information that was submitted with the web form; the front-end receives information about which boxes were checked.

Code your Project
Start working on your project! Go back to the "Workspace Portfolio Exercise" with the template code. You'll find it earlier in this Portfolio Exercise lesson. Here are a few APIs that you might find interesting to work with:

World Bank API https://datahelpdesk.worldbank.org/knowledgebase/articles/889386-developer-information-overview
API for Entertainment Industry  http://developer.rovicorp.com/docs
City of Berlin Open Data API https://daten.berlin.de/datensaetze/deutsche-digitale-bibliothek-ddb-api
Many government and city agencies have APIs where you can access city data.
