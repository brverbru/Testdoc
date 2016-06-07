# Cumul.io User Guide

Welcome to Cumul.io! You’ve definitely made the right choice in signing up! You’re now on your way to having control over your data and being able to gain meaningful insights in a safe, simple and manageable way. That’s a nice feeling, right?
>###These are the user docs! Switch to the [API docs](https://www.google.com)?

>Can’t find what you were looking for in our guidelines? Drop us an email at **support@cumul.io** and we’ll help you out asap. 

>Alternatively you can **live chat** with our support team or leave feedback/report bugs using the square tabs that appear on the left-hand side of the webpage. 


# Getting started
## Quick start


Looking for a quick and easy way to get started (or don't want to read the complete guide) ? Check out of our getting started tutorials! 


## Registering & sign in

Registering is simple, just leave your name, email address and password and we’ll create an account for you. You’ll be redirected to the platform immediately.

Login is pretty straightforward too, just fill in your credentials or sign in with Google, Facebook or Twitter, if you’ve linked these to your profile.

>![Login modal](http://i.imgur.com/1erdGEf.png)

##Navigation

You’ll first arrive at the overview page, which gives a summary of your latest dashboards as well as the hottest datasets available on the the platform. From here, you can navigate to tabs for your datasets and dashboards if you want to start creating visualizations, or you can access your profile using the top right icon to update personal information.
>![Overview screenshot](http://i.imgur.com/m1rpojh.png?1)

Under both the datasets and dashboards tab, there are different options for displaying personal data, data shared with you by others, and data available to the public. You will also find a search function to filter your datasets or dashboards using keywords. 

##Notifications 
At any point in the app, you can receive **notifications** by way of the notifications widget, accessible by the icon in the top right of the page, beside your profile. 
>Notification may include, for example, the status of a dataset upload, or datasets and dashboards that have been shared with you.

>![Notification icon](http://i.imgur.com/bKLLX8I.png)

 
 
##Profile & profile details

On the profile page, you can adjust your personal profile details, add social media accounts, manage your organisation or business, and access your billing plans.
>![profile page](http://i.imgur.com/GxF8CoZ.png?1)
 
Connecting social media accounts in the Social Accounts tab allows you to share your dashboards without the need to login on an external site.
 
Your organisation page provides an overview of contacts in your organisation /////ASK KAREL OR HAROEN
 
The Plans & Billing page allows you to manage your licenses and payment options.

#Datasets Tab
 
##Overview
 
The dataset tabs displays an overview of your uploaded or connected datasets and allows you to add new datasets. You can search for datasets here as well.
>![Dataset tab](http://i.imgur.com/EaMLvz4.png?1)


##Connecting new datasets
 
By clicking the bright blue “new dataset” button, you will open a modal window. In this modal you can select the source of your new dataset, which can be either a local file, a web service or a database connection. 
>![Add dataset button](http://i.imgur.com/4VHtAeg.png)

 
###    Local files
 
You can browse to select local files to upload them unto the platform, or simply drag and drop files into the upload window provided. Supported file types currently include: 

+ CSV 
+ TSV
+ JSON
+ topoJSON
+ geoJSON
+ xls
+ xlsx
+ xlsb
+ csb



###Web services
 
Web services integration allows you to fetch data directly from your personal accounts where data is stored. For example, connect to your Facebook or Google Drive account. The first time you connect to each external account, you will be provided with an initial prompt to login with your credentials. 

//TODO

Explain what happens once you link to the account… Does it connect within the platform and provide a list of files? Or is the user directed to an external link
Unless the process works differently for each type of connection, perhaps it is not really necessary to provide a separate description of each
 
 
####Quandl
####Google drive
####Google Analytics
 
###From a data source

Data source integration enables you to connect to an external data server, such as SQL Server or Oracle. 
More details about how this connection process works?

####Postgres
####SQL server
####DB2
 
###Using the API
·       Redirect to API documentation

Can you give some details on the format/type of API used, then I can give a short summary and provide the right documentation website?

##Dataset page
###Overview of the page
 
Selecting a dataset will direct you to its contents and structure. Each column displayed is a field, and each row represents one record. The charts at the top of each column show the distribution of the data contained in the field. The search function enables you to quickly find specific values. You can change the data type by selecting the data icon displayed to the left of each field name. You can edit the hierarchy, calculate a derived column or delete the row by selecting the options icon at the right of each data distribution display. 
>![Dataset page](http://i.imgur.com/QHDgkNF.png?1)

Furthermore, you can navigate to the dataset detail page, manage datasets links or share the dataset by clicking the respective links in the top right of the screen.

 
##Data types

The cumul.io platform supports several types of data: 

+ **Numeric data** is information of a measurable form. It is always collected in number form, although there are other types of data that can appear in number form. An example of numerical data would be the number of software licenses sold by a company in one month. You can perform almost any mathematical operation on numeric data, you can arrange it in ascending or descending order, and the answers must be able to be represented in fraction or decimal form. 

+ **Hierarchical data** is a set of items that are related to each other by relationships containing hierarchy. Its structure uses a one-to-many relationship for data elements, consisting of a tree structure that links a number of separate elements to one "parent" primary record. As an example, consider a company consisting of individual employees that each report to a given department. The department is then considered the parent record and the individual employees are then secondary records, each one linking back to its respective department, or parent record.

+ **Datetime data** can combine both a date and a time. It stores chronological information such as month, day, year, hours, minutes, and seconds. This consists of numerical data stored in a specific format; for example, 'YYYY-MM-DD HH:MM:SS' to represent the year, month, date, hour, minutes, and seconds, in that order. 

+ **Topography data** includes many types of geographical information that can be found on a map at a specific elevation on Earth’s surface. Cumul.io supports vector data, which can consist points, lines, or polygons. This can include, for example, municipal boundaries, contour lines, rivers, lakes, roads, railroads, towns, land cover boundaries, GPS points, or GPS tracks. 
 
##Derived columns

The Derived Column option basically does what it says: it allows new data fields to be derived from your existing data. This is done by way of a “transformation” that creates new column values by applying expressions to the transformation input columns. This process is similar to most spreadsheet operations. 

To get you started, consider some of the following features of our platform. An expression can contain any combination of variables, functions, operators, and columns from the transformation input. The result may either be added as a new column or may be inserted into an existing column as a replacement value. The Derived Column transformation can define multiple derived columns at once, and any variable or input columns can appear in multiple expressions.

This transformation can be used to perform many tasks, some of which are explained in the following examples. 

It is possible to concatenate data from different columns into a derived column. For example, say you have a column for “first name” and a column for “last name” and you would like to combine them into one field representing a full name. The values from FirstName and LastName columns can be combined into the single derived column of FullName, by using the expression FirstName + " " + LastName.

Mathematical functions can be applied to numeric data and the result can be stored in a derived column. For example, you could change the length and precision of a numeric column, SalesTax, to a number with two decimal places by using the expression ROUND (SalesTax, 2).

Say you would like to convert date strings into a specific format. For example, ‘MM-DD-YY’ should become ‘DD-MM-YY’. This can be done using the specific expression:           Not sure if this is possible in the platform



##Dataset info page
 
Under the Datasets tab you find your list of datasets, and using the icons on the right-hand side of each dataset listed, you can perform simple actions, or you may navigate to the dataset info page. This is where you can find general information on your specific dataset and perform a variety actions. You may see the details of the information stored in the dataset, share it with your team, delete the dataset or upload a newer version. This page also allows you to add tags as well as a description, which is helpful for finding the dataset using the search function. This is especially useful if you decide to publicly publish your dataset, because it enables other users to easily arrive ?? at your data. 

 
##Joins & Links

In order to blend datasets together, you must first specify how different datasets are linked. Therefore, find the links modal option within your dataset view. As with most operations in Cumul.io, you can create a link by dragging the foreign key (of your lookup table) to the primary key (of your master table). Yes, the overall principle is as simple as that! However, let’s talk about some of the details of how the platform performs the links.

Joins and links are done using the LOOKUP principle, which is as straightforward as it sounds: Cumul.io “looks up” a specified value in another dataset. A join therefore occurs when the specified value of a field in dataset A is found in another field from Dataset B. 
There are three different kind of joins in Cumul.io 

+ Exact match: This is possible when a value in dataset A is exactly the same as in dataset B. For example, this could be a customer ID or reference code that is the same in each of your datasets.

+ Fuzzy match: This option is used when a value in dataset A is very similar to the corresponding value in dataset B. For example, if customer names are filled in manually and some typing errors were made, a match can still be found.

+ Time match: This joins datetime values of dataset A to dataset B, with the option of defining the match in different ways. After creating your link in the modal, the following options can be chosen by selecting the icon on your link. 

 + Value A is closest to a datetime Value B
 + Value A is closest to, but occurring after a datetime Value B
 + Value A is closest to, but occurring before a datetime Value B 
 
##Sharing datasets
 
Sharing datasets can be done with users or groups that exist within your organization or business. There are several levels of access that users may have. 
+ “Viewers” are simply able to view the dataset but cannot use it in a dashboard. 
+ “Can use” means the user is able to use the dataset in a dashboard. 
+ “Edit” means the user can view, use and edit the dataset.
+ An “owner” can do all of the above and can also adjust the privileges and roles of each dataset user, specifying whether they can view, use, edit or become the owner of a dataset. 


#Dashboards Tab
##Overview & Navigation

The dashboards tab displays your latest dashboard, dashboards that have been shared with you or dashboards that are shared publicly. This tab is your gateway to the dashboard editor, which what you connect to from the bright blue “New dashboard” button. This is where you can start what you’ve been waiting to do, creating visualizations of your data! Read on in the following sections to find out all about the Dashboard editor.

 
#Dashboard editor
 
##Navigation

The dashboard editor… This is where the fun begins! Let’s get started actually gaining insights to your data! 

There are three main parts to the dashboard editor: the items bar on the left, the canvas in the middle and the settings tab on the right. Let’s get some explanations about all the panes and extra buttons. 

##Items pane
 
Selecting ‘add item’ on left-hand pane will display the different items you can drag and drop into the canvas. There are general items, filters, classic charts, maps and more complex charts. We will discuss each object in more detail:

###General

+ A text object creates a formattable template text box. It can be used for adding sources or adding additional information about the items or data displayed. 
+ An image object adds a picture or icon to the dashboard. For security reasons, uploading pictures is not possible, but you can host your image on imgur, flickr or any other service and fill in the url in the image objects settings. 
+ Video object
+ Number object
+ Add tables to view your data in table format. A pivot table allows you to make a table based on datasets linked to one another. If the datasets are not already linked, you will get a prompt to do so when you add a column from a different dataset to the pivot table.
+ A spacer [ICON] allows you to create self-defined gaps between the items in your dashboard, allowing for a more attractive layout organization.

###Filters

Filter items let you view your data in various ways. Each one is briefly mentioned below. 

+ A date filter allows you to specify which time period is displayed for your items. Applying a filter item filters the dates for the entire dashboard. 
+ A date slider [ICON] performs the same operation as a date filter, but it creates a module allowing the user or viewer to adjust the time period of the date filter interactively.
+ A search box allows viewers to search for a specific dimension in the data, and filter results to just this dimension. For example, for items explaining the volume of sales for all products over time, a one could search for a specific product, in order to only display this product in the graphs. 
+ A select box lets the viewer select a dimension from a drop-down menu. 
+ A slicer allows users to select which dimensions to display by means of a check-box list of  items. 

###Bar & Column Charts
+ A bar chart is a graph that displays grouped data using rectangular bars. The lengths of the bars are proportional to the values that they represent. 
+ Group bar charts are a way of representing or comparing information on different sub-groups within the main categories. For example, volume of sales for a product can be divided into the age groups that purchases them. 
+ The stacked bar chart depicts items stacked side-by-side, differentiated by colored bars or strips. A stacked graph is useful for looking at changes in, for example, expenditures added up over time, or across several products and services. The graph integrates different data sets to create a richer picture of (the sum of) changes.
+ The column charts (column, grouped column, stacked column) are identical to the bar charts, except that data is plotted vertically instead of horizontally. For the stacked column chart, data items are then stacked on top of one another. 

###Line charts

+ A line chart is a graph displaying information as a series of data points that are connected by straight line segments. This classic chart is common for many purposes, but is most often used to represent changes in data over time. For example, a line connected between data points for sales volume per month helps to visually represent the increase or decrease in sales that occur from one month to the next. 
+ The grouped line chart is used to represent the evolution of multiple dependent variables (y-axis) as a function of one independent variable (x-axis). For example, you could visualize the evolution of various product sales, where each line represents the specific volume of sales for one individual product.
+ A line color chart can be used to visually point out various trends or categories of the data line displayed. For example, color coding can be used to indicate those months when sales are increasing or decreasing, or, as another example, months when sales are at a peak period. 

###Scatter & Bubble Plots

+ A scatter plot is one of the simplest ways to represent data by plotting two variables against each other. This type of chart is best used to represent continuous rather than categorical variables. The result is a series or “scatter” of individual points. Each data point then represents one XY value. 
+ A group scatter can then display further trends on a scatter plot by grouping the data points and color-coding them based on a third dimension. 
+ A bubble chart is a method of displaying three dimensions (x, y, z) or series of data in a chart format. Bubble charts can be considered a variation of a scatter plot, where the data points are replaced with bubbles. The location of each bubble represents its XY value, while the size of the bubble expresses the third dimension, Z. For example, a good use for a bubble chart is to display the number of customers buying a product (X), the total sales from that product (Y), and the percentage of total sales that product represents (Z). 
+ A colored bubble chart differentiates the chart as in the group scatter, further dividing the data into sub-groups.

###Area Charts
+ An area chart is simply a line chart with the area below the line filled in. This is best used to display the cumulative volume of a variable over time. 
+ A stacked area chart is then useful to display the contribution of different values to an overall total over time or as a function of another variable. As an example, Cumul.io can analyze its number of customers over time, differentiated by the sector they work in, such as marketing, private commerce, geographic analysis, socio-economic analysis, etc. 
+ A 100 stacked area chart is used to display the relative contributions of various components and how these vary as a function of another variable. The area of each component corresponding to any given point on the X axis then represents its percentage of the total at that point. As an example, say that during the year of 2015, the relative sectors of Cumul.io customers on average is represented by: marketing (35%), private commerce (30%), geographic analysis (20%), socio-economic analysis (10%), and other (5%). In 2016, these proportions could change to: 30%, 25%, 15%, 5%, and 25%, respectively, as the Cumul.io platform expands into other sectors. A stacked area chart would show this evolution over time. 
+ A streamgraph is a type of stacked area chart which is displaced around a central axis, resulting in a flowing, organic shape. This can ideally be used to represent the evolution of an overall total over time, as well as the relative contributions of various sub-parts. As an example, consider a company selling multiple smartphone applications to users. The company could use a streamgraph to show the evolution of total application use of users over time, and could differentiate the stream based on the relative use of each individual application.

###Pie & Donut
+ Pie chart is a graph where a circle is divided into sectors that each represent a proportion of the whole. The arc length of each slice is proportional to the value it represent. This type of chart is often used in business and media. 
>We cannot recommend pie and donut charts as best practice since they have been criticized by experts. It can be difficult to compare different sections of a pie chart and to make comparisons across different charts. (see: https://www.perceptualedge.com/articles/visual_business_intelligence/save_the_pies_for_dessert.pdf)
+ A donut chart is similar to a pie chart, but can be used to represent more than one data series. Different rings of the donut then represent different datasets. 

###Small Multiples

+ Multiples charts can be used to combine several charts into one figure. This is often done when multiple trends are interconnected by sharing an x- or y-axis. ...
+ Multiples-bar: Coming soon to Cumul.io!
+ Multiples-column: Coming soon to Cumul.io!
+ Multiples-line: Coming soon to Cumul.io!
+ Multiples-scatter: Coming soon to Cumul.io!

###Maps
+ A cloropleth map uses variations in shading or coloring over a predefined area in order to explain the average values of a variable in that area. For example, the average unemployment in each province in Belgium can be displayed, using a shading percentage that is proportional to the unemployment level. 
+ Symbol maps will scale the size of a simple symbol (for example, a circle or square) in a proportional way to the value found at that location. The symbol can be scaled to the exact value, or can be graduated based on the different categories the value may fall into. Proportional symbol maps may be preferred over dot density maps because it is easier for viewers to quickly gain insights from the map since estimating the size of a symbol is less tedious than counting many little dots. An advantage of proportional symbol maps over choropleth maps is that the size of the areal unit plays less of a role. For example, consider population density. If a country with a small geographic area, such as Belgium, has a large associated value, it will have a large symbol over it. On a choropleth map, however, smaller places are easily overlooked on a complex border map, such as, in this case, Europe. No matter what color is assigned to countries, the larger areas on the map, such as nearby France and Germany, still dominate when a user is visually inspecting the map. Therefore smaller countries with higher population densities can be overlooked. 
Source: http://indiemapper.com/app/learnmore.php?l=proportional_symbols 

+ A marker map simply uses a predefined symbol to display locations. This can be helpful, for example, if a company wants to show users where they are present in the world by showing the locations of offices in New York City, Brussels, and Hong Kong. 
+ Hexbin maps are an alternative way to visualizing density maps from large datasets. It aggregates the data points that fall within either a rectangle or hexagonal shape, creating a new value for that area matching the number of data points contained. 
+ A heatmap is a graphical or raster representation, where the values of different pixels are represented by different colors. It is different from a cloropleth map in that it does not conform to specific geographic boundaries. An example of a heatmap is a weather radar displaying expected rainfall. Different color schemes can be used for heatmaps, but their representation is often hierarchical. Darker colors can, for example, represent higher expected rainfall. 
+ Route map: Coming soon to Cumul.io!
+ Dot map: Coming soon to Cumul.io!

###Special Charts
+ A bubble chart is a simple version of the bubble scatter mentioned above, and can be used to represent quantitative information by means of the shapes of various circles, or ‘bubbles’, displayed next to one another on the chart, with sizes proportional to the quantity they represent. It can be used, for example, to explain the volume of different types of products sold by company. 
+ Strip plots are arranged with categories on the x-axis and display the distribution of points over each category, or the extent of a ‘column’. This gives users a better idea of the distribution their data has in various groups, and allows for a better visualization of other metrics like the mean, distribution quartiles, and outliers. For example, a marketing company can investigate the variation in the number of contracts signed, grouped by various business sectors for comparison.
+ A treemap is a visualization of hierarchical structures, using a set of nested rectangles organized within a predefined space. Each branch of a tree is represented in a rectangle, and within this rectangle, smaller rectangles represent sub-branches. Color coding can be used for separate dimensions of the data. This type of visualization helps users to compare nodes and sub-branches in a compact way, even when various branches are far removed from one another in the tree. This is good for spotting patterns and trends. 
+ A radar chart, also called a web, spider or star chart, is a plot consisting of a series of equi-angular lines, or spokes, originating and extending from the same point. The position of the data value along each spoke is proportional to the magnitude of the variable in question for that spoke. Lines connecting the data values for each spoke give it a star-like or web-like appearance. Several variables can be analyzed in one chart, making it a useful way to represent multivariate information. For example, a radar chart could represent the overall budget scheme of a company, where overall revenues from sales is allocated to meet the needs of the different departments of HR, marketing, technical development, etc. 
+ Heat matrix: Coming soon to Cumul.io!
+ Bar line chart: Coming soon to Cumul.io!
+ Pareto diagram: Coming soon to Cumul.io!
+ Boxplot: Coming soon to Cumul.io!
+ Boxplot with width: Coming soon to Cumul.io!
+ Bullet chart: Coming soon to Cumul.io!
+ Dot chart: Coming soon to Cumul.io!
+ Pyramid: Coming soon to Cumul.io!


###Financial Charts
+ Open-high-low-close chart: Coming soon to Cumul.io!
+ Candlestick chart: Coming soon to Cumul.io!
+ Kagi chart: Coming soon to Cumul.io!


## Settings Pane

The general dashboard settings can be found in the taskbar pane in the right-most tab (you guessed it, the settings tab). These settings are applicable to the entire dashboard. You can enable or disable a dashboard (sub)title here, specify the margin between objects, and do all kinds of other things as well. Explore the options for yourself! 

These settings are valid for the complete dashboard and all of its views (desktop, tablet, mobile) except if you have unsynced the different views. We’ll get to that. 
 
As with the settings tab, the filters tab makes changes that are applicable to the complete dashboard. This means that if you filter out certain records here, they will never be shown or taken into account for any item you place in your dashboard. 

Any field of any dataset can be filtered, as long as the dataset is being used in the dashboard. Possible filters include, but are not limited to, ‘is in’, ‘equals’, ‘is greater than’, ... The usual stuff!

The data tab allows you to navigate to your datasets and add them to the canvas. Simply select a dataset and drag and drop fields to the canvas! 

The item tab show you the selected item’s specific settings. These settings involve general things like title, background, and borders, but also displays item-specific settings that influence the visualization. 


 
 
##Canvas
 
The canvas serves as your ultimate workspace, where you can drop any of the objects you need and start analyzing. Within an object that you add to the canvas, there are different slots into which you can drag data. This generally corresponds to the  ‘X-axis’ (independent variable), the ‘Measure’ (y-axis, or dependent variable), and a ‘group-by’ function allowing further differentiation of the data. Some slots are limited to certain data types. For example, a bar chart, inherent in its definition, is only limited to categorical variables on the y-axis, while the y-axis of line charts can accommodate both continuous and categorical data. On the right hand side of each object, three icons appear that allow the user to (1) adjust data properties, (2) adjust settings for the object, and (3) delete the object entirely. 

 
###Screensize views

A the top of the canvas, you can switch views between mobile, tablet and desktop. By default, these three different views are in sync, which means that if you update an object in one of the views, it is automatically updated in the others as well. In the dashboard settings tab you can disable this option, allowing you to create different dashboards for each of the three individual views, without altering the appearance of the others. Alternatively, you can opt for a fixed-width dashboard, which keeps the display of your work at the same width, regardless of the device screen size. 
 
###Sharing dashboard
 
So you’ve gotten your insights ready and created a stunning dashboard? Great! Let’s share it! 

Sharing a dashboard is similar to sharing a dataset. You can share with other Cumul.io groups and users within your organisation, or you can share publicly.

To share a dashboard with groups or users in your organisation, select a specific user and assign them the role you allow them to have. There are several levels of access that users may have:
+ “Can view” means the user can view the dashboard but cannot edit or make a duplicate
+ “Can use” means the user can make a duplicate, but cannot edit the original dashboard
+ “Can Edit” means the user can view, use and edit the Dashboard
+ An “owner” can do all of the above and can also adjust the privileges and roles of other dashboard users.

Publicly sharing a dashboard can be done by ‘Link sharing’. Once this option is turned on, a unique short url is created which redirects the visitor to the published dashboard. Only viewers who receive the URL will be able to view the dashboard. This sharing method is similar to sharing documents with Dropbox, Google Drive or WeTransfer. 

This method requires the datasets to also be made publicly available (otherwise the dashboard would not be able to query the data). This option does NOT mean the dataset will show up in the Cumul.io public library. 

Finally, sharing with social media is also possible. With this option a link for the dashboard will be sent to the specified social media platform.




