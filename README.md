# Data-Management-and-Analytics, CSCI-UA479
Homework and projects from DMA course Fall 2023 taught by Joseph Veroza  
<details>
  <summary>Course Description:</summary>
  CSCI-UA 479 Data Management and Analysis  
  
Students that successfully complete CSCI-UA 479 Data Management and Analysis are not eligible to take CSCI-UA 60 Database Design and Implementation. Extracting, transforming and analyzing data in myriad formats. Using traditional relational databases as well as non-relational databases to store, manipulate, and query data. Students will learn how to work with data by writing custom programs, creating queries, and using current data analysis tools and libraries… all on a wide array of data sets. Additional related topics will be covered, such as data modeling, cloud databases, and API programming
</details>


### [Assignment 1: BitList and Book(s)]( https://github.com/nyu-csci-ua-0479-001-fall-2023/homework01-ericemmendorfer )
<details>
  <summary>Overview:</summary>

    
  [Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/01.html)

    
  ### Part 1: BitList Class  
  In a file called bits.py, create a class, BitList, that represents a series of bits. The class and instances of the class will have methods representing operations that can be performed on those bits.  
    
  You can test your class implementation by running the unit tests in bits_test.py. These unit tests will check that your class and methods behave (mostly) as specified by the requirements below.  

  Methods Include:  
  
  __eq__(self, other): Returns a boolean if two BitList are equal  
   
  BitList.from_ints(b1, b2, ...bN):   
  
  str: Converts the BitList to a string  
  
  .arithmetic_shift_left() and .arithmetic_shift_right()  
  
  .bitwise_and(otherBitList)  
  
  .chunk(chunk_length)  
  
  .decode(encoding='utf-8')


 ### Part 2: Books  
  Using at least two books from project Gutenberg use file io and basic Python to manipulate the content of the books.

1. Gather Your Data
  a. "manually" download txt versions of at least two books (right-click save as on the link – you do not have to have to programmatically download these books)
  b. save the books into the data folder of your repository
2. Working with Files
a. start jupyter lab on the commandline in the root of your cloned project directory directory: jupyter-lab
b. open jupyter lab in your browser; use the file explorer to find, open, and edit the notebook book.ipynb in a markdown cell:
c. write out information about the books you downloaded
-  a description of the books (titles and authors, for example… or all works by author, etc.)
-  the url to the book or folder of books
-  any license information
-  encoding if provided
  
  d. write a question you'd like answered about the books that might require some programming… for example: 
-  who was the most frequently mentioned character in Pride and Prejudice… and in Sense and Sensibility?
-  are the pronouns in Mary Shelley's books predominantly male or female?
-  etc. …. (feel free to use either of the above questions, or come up with your own!)

  e. open the txt versions of the books that you downloaded by writing Python in your notebook
-  use a relative path to data/name_of_your_file (this should work on both MacOS and Windows despite the path separator differences)
-  alternatively, you can use os.path.join to construct paths with the right path separator
-  use jupyter notebook code cells to analyze the text in your file…and come up with an answer a dictionary (or counter object if you're familiar with counters) must be part of your analysis

  Notes:
  -  checking for an existence of a key with in may be helpful
  -  "catching" a KeyError will also identify keys that are missing
  -  adding a key looks like: d['new key'] = 'new value'
  -  update a key looks like: d['key'] = d['key'] + 1
  -  (or again, a counter object can be used)
  -  document your steps in markdown cells
  -  your answer does not have to be correct (or even exact!)… as long as you have some description of your analysis
  -  again, make sure you include the txt files in your repository within the data directory
</details>
 

### [Assignment 2: List Comprehensions, Classes, CSV, Tabular Data]( https://github.com/nyu-csci-ua-0479-001-fall-2023/homework02-ericemmendorfer  )
<details>
  <summary>Overview:</summary>

  
  [Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/02.html)    

### Part 1: Highest and Lowest Potentially affected vehicles.  

This part uses a modified dataset from https://www.kaggle.com/datasets/michaelbryantds/automobile-recalls-dataset. 
 
 This data contains Manufacturer name, Recall Type, Component, etc.
  
The dataset contained in your repository has been modified:
-  columns have been removed
-  column names have been changed
-  some rows have been removed due to non numeric values in numeric columns
-  some rows have been removed to consider only subset of the data


    
In recall.ipynb:  


-  using list comprehensions, dictionary comprehensions and generators is okay (a for within these structures is ok) open the recalls-truncated.csv file
-  display the Manufacturer and Potentially Affected fields for the highest and lowest Potentially Affected in the dataset
-  only do this for rows that have vehicle value for the Recall Type column
-  your discretion on what to do if there are ties
-  print out your results in any format that you prefer (dict, tuple, str, etc.)
### Part 2: nelta.py
### Part 3: nelta.py and Recalls with Potentially affected vehicles > 500,000
  
</details>


### [Assignment 3: Sourcing Data, Summary Statistics, and Basic Data Visualization]( https://github.com/nyu-csci-ua-0479-001-fall-2023/homework03-ericemmendorfer  )
<details>
  <summary>Overview:</summary>
  
  [Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/03.html)  
  
  Goals:
<li>source and document a dataset</li>
<li>use plain Python and built in modules to extract and transform data</li>
<li>work with numpy to calculate summary statistics</li>
<li>use matplotlib for simple data visualizations </li>
  <br>
Requirements
<li>1 x notebooks:  src/homework03.ipynb</li>
<li>1 x original data set:  data/raw/* </li>
  <br>
Overview: <br>
In this assignment, you'll create a single notebook, (ipynb) that contains documentation and code. There are 6 parts to this assignment:
  
  1. write some questions that may be answered by using summary statistics and / or creating visualizations
  
  2. select and document a data set
- ⚠️ the data should be comma / pipe / tab delimited…
- ⚠️ the data set should have at least one numeric column and one column that contains categorical data
- include documentation regarding the source of the data
- include the data set in your repository so that your notebooks can be run by the graders without having to perform any setup (if data set is > 100MB, link to file instead)

3. use "regular" python with built-in modules to create a data pipeline to extract or transform data
4. work with numpy or regular Python to calculate summary statistics
5. create at least two visualizations with matplotlib
6. write a conclusion answering your initial questions based on the summary statistics you calculated or visualizations you created
- describe the results of your calculations and visualizations
- describe whether or not they were able to answer your initial questions
</details>


### [Assignment 4: Pandas Basics](https://github.com/nyu-csci-ua-0479-001-fall-2023/homework04-ericemmendorfer  )
<details>
  <summary>Overview:</summary>  

  [Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/04.html)  

  Goals:
<li>importing data with pandas</li>
<li>cleaning / preparing data with pandas</li>
<li>using pandas for basic data analysis</li>
<li>displaying summary statistics</li>
<li>value counts</li>
<li>consuming data from the web</li>
<li>merging / joining data </li>
  <br>
Overview:
  <br>
This homework consists of two parts:

1. Analyzing NYC Traffic Accidents data from Janurary-August 2020
2. A data cleaning / transformation project of your choice with pandas
</details>


### [Assignment 5: Data from the Web, Combining Data](https://github.com/nyu-csci-ua-0479-001-fall-2023/homework05-ericemmendorfer  )
<details>
  <summary>Overview:</summary>

  [Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/05.html)
  
</details>



### [Assignment 6: Single Table, Importing Data, SQL](https://github.com/nyu-csci-ua-0479-001-fall-2023/homework06-ericemmendorfer  )
<details>
  <summary>Overview:</summary>

[Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/06.html)

</details>


### [Assignment 7: ER diagrams, SQL queries, Postgresql, Normalization, DDL Commands](https://github.com/nyu-csci-ua-0479-001-fall-2023/homework07-ericemmendorfer  )
<details>
  <summary>Overview:</summary>
  
[Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/07.html)

</details>


### [Assignment 8: Window Functions, Analyze Query Performance, SQLAlchemy](https://github.com/nyu-csci-ua-0479-001-fall-2023/homework08-ericemmendorfer  )
<details>
  <summary>Overview:</summary>

[Full Requirements](https://cs.nyu.edu/courses/fall23/CSCI-UA.0479-001/_site/assignments/08.html)

</details>



### In Class Assignment 1: Manual File Parsing and Data Visualizstion
### In Class Assignment 2: Normalization
### In Class Assignment 3: MongoDB
