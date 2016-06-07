# Cumul.io User Guide

Welcome to Cumul.io! You’ve definitely made the right choice in signing up! You’re now on your way to having control over your data and being able to gain meaningful insights in a safe, simple and manageable way. That’s a nice feeling, right?
>These are the user docs! Switch to the [API docs](https://www.google.com)?

The following guidelines will enable you to get started with exploring data yourself, without ever requiring any technical expertise!

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

 
###Data types

The cumul.io platform supports several types of data: 

+ **Numeric data** is information of a measurable form. It is always collected in number form, although there are other types of data that can appear in number form. An example of numerical data would be the number of software licenses sold by a company in one month. You can perform almost any mathematical operation on numeric data, you can arrange it in ascending or descending order, and the answers must be able to be represented in fraction or decimal form. 

+ **Hierarchical data** is a set of items that are related to each other by relationships containing hierarchy. Its structure uses a one-to-many relationship for data elements, consisting of a tree structure that links a number of separate elements to one "parent" primary record. As an example, consider a company consisting of individual employees that each report to a given department. The department is then considered the parent record and the individual employees are then secondary records, each one linking back to its respective department, or parent record.

+ **Datetime data** can combine both a date and a time. It stores chronological information such as month, day, year, hours, minutes, and seconds. This consists of numerical data stored in a specific format; for example, 'YYYY-MM-DD HH:MM:SS' to represent the year, month, date, hour, minutes, and seconds, in that order. 

+ **Topography data** includes many types of geographical information that can be found on a map at a specific elevation on Earth’s surface. Cumul.io supports vector data, which can consist points, lines, or polygons. This can include, for example, municipal boundaries, contour lines, rivers, lakes, roads, railroads, towns, land cover boundaries, GPS points, or GPS tracks. 
 
###Derived columns

The Derived Column option basically does what it says: it allows new data fields to be derived from your existing data. This is done by way of a “transformation” that creates new column values by applying expressions to the transformation input columns. This process is similar to most spreadsheet operations. 

To get you started, consider some of the following features of our platform. An expression can contain any combination of variables, functions, operators, and columns from the transformation input. The result may either be added as a new column or may be inserted into an existing column as a replacement value. The Derived Column transformation can define multiple derived columns at once, and any variable or input columns can appear in multiple expressions.

This transformation can be used to perform many tasks, some of which are explained in the following examples. 

It is possible to concatenate data from different columns into a derived column. For example, say you have a column for “first name” and a column for “last name” and you would like to combine them into one field representing a full name. The values from FirstName and LastName columns can be combined into the single derived column of FullName, by using the expression FirstName + " " + LastName.

Mathematical functions can be applied to numeric data and the result can be stored in a derived column. For example, you could change the length and precision of a numeric column, SalesTax, to a number with two decimal places by using the expression ROUND (SalesTax, 2).

Say you would like to convert date strings into a specific format. For example, ‘MM-DD-YY’ should become ‘DD-MM-YY’. This can be done using the specific expression:           Not sure if this is possible in the platform



###Dataset info page
 
Under the Datasets tab you find your list of datasets, and using the icons on the right-hand side of each dataset listed, you can perform simple actions, or you may navigate to the dataset info page. This is where you can find general information on your specific dataset and perform a variety actions. You may see the details of the information stored in the dataset, share it with your team, delete the dataset or upload a newer version. This page also allows you to add tags as well as a description, which is helpful for finding the dataset using the search function. This is especially useful if you decide to publicly publish your dataset, because it enables other users to easily arrive ?? at your data. 

 
###Joins & Links

In order to blend datasets together, you must first specify how different datasets are linked. Therefore, find the links modal option within your dataset view. As with most operations in Cumul.io, you can create a link by dragging the foreign key (of your lookup table) to the primary key (of your master table). Yes, the overall principle is as simple as that! However, let’s talk about some of the details of how the platform performs the links.

Joins and links are done using the LOOKUP principle, which is as straightforward as it sounds: Cumul.io “looks up” a specified value in another dataset. A join therefore occurs when the specified value of a field in dataset A is found in another field from Dataset B. 
There are three different kind of joins in Cumul.io 

+ Exact match: This is possible when a value in dataset A is exactly the same as in dataset B. For example, this could be a customer ID or reference code that is the same in each of your datasets.

+ Fuzzy match: This option is used when a value in dataset A is very similar to the corresponding value in dataset B. For example, if customer names are filled in manually and some typing errors were made, a match can still be found.

+ Time match: This joins datetime values of dataset A to dataset B, with the option of defining the match in different ways. After creating your link in the modal, the following options can be chosen by selecting the icon on your link. 

 + Value A is closest to a datetime Value B
 + Value A is closest to, but occurring after a datetime Value B
 + Value A is closest to, but occurring before a datetime Value B 
 
###Sharing datasets
 
Sharing datasets can be done with users or groups that exist within your organization or business. There are several levels of access that users may have. “Viewers” are simply able to view the dataset but cannot use it in a dashboard. “Can use” means the user is able to use the dataset in a dashboard. “Edit” means the user can view, use and edit the dataset. An “owner” can do all of the above and can also adjust the privileges and roles of each dataset user, specifying whether they can view, use, edit or become the owner of a dataset. 




