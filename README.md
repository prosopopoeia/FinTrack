FinTrack v1.0 (FT1)

There are a number of budgeting/financial tracking software applications available on the internet of varying complexity (and usefulness!).
Financial Tracker is the first iteration of a project that is hoped will grow to be flexible enough for everyday needs or to as a simple tool 
for small business/contractor needs. V1 is focused on personal financial tracking with plans to expand functionality to add flexibility at a
later time.

As a prototype, this application may be something of a stubb. Ideally, one would set up the application to interact with an API of the user's
financial institution. The limitation here is the API endpoint's data and format are unknown to the author. As a proxy, and to allow for test
data, an input page will allow the user to upload bank-statement like documents (which are also provided for the convenience of prototype users).

Distintivity and Complexity Requirements


1. Complexity and distinctiveness. 

	It would be difficult to avoid all overlap with previous assignments when creating a application of this nature. However, a number of distinct 
	features are presented in this application. To enumerate a few:
		
		- Graphics 
			The program features graphical components to help users to visual the data. These components are adaptations of a graphing library 
			provided by Google Charts (https://developers.google.com/chart/). These components were fairly easy to incorporate and provide a way to
			quickly evaluate the data presented. Users may toggle between a pie chart and a bar graph. The graphs and chart each had to accomodate a variety of views. It was necessary to make the visuals flexible enough to handle the 
			size of the data set used to populate the graphic. For instance, a view in which the user can look at all bank transactions over the 
			lifetime of their transactions had to be capable of displaying categories such that they were distiguishable from neighboring elements.
			For this purpose, a bar graph that scales based on the number of transactions in the data set is provided (though the option to view 
			the data via a pie chart is still available).
			
		- Parsing
			Text parsing using Python's regular expression library was employed to split apart the bank-statement like documents to extract the 
			relevant financial data. In addition, a utility to upload documents is provides another distinction from previous projects.
			
		- Document Utility
			Functionality to upload document for parsing.
			
		- Data Crunching
			Django's built-in filters and functions were used more extensively. Tallying the data and presenting it to the user was done.

2. Files
 
		