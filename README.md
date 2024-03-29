# WEB CRAWLER
## A set of programs that emulate some functions of a search engine

### Implementation:

##### We have implemented a web crawler which asks the user for an initial webpage and then crawls through that webpage and its internal links.
##### It performs multiple searches and stores its data in a SQL database (spider.sqllite)
##### Ranked the search results using the Page Rank algorithm to rank the most relevant search result
##### It then creates a visualization using a JSON file (which has all the data dumped into it), The result is a Node Web.

#### Please check the poster file in the Repository for more information


### Visualization:

![Webpage_graph](https://user-images.githubusercontent.com/69566994/149311366-65ab9cc7-0fa9-4367-8195-59bca4f2423d.png)


### Alternative Algorithm

##### Over the summer I read about another way to find the rank of our search results. I have mentioned a method of converting the rank match algorithm as an optimization problem and solving it using Linear Algebra.
##### Now we know that the page rank algorithm uses spidering but it spiders through an imaginary web of webpages that are all connected. What if we imagine this web as a matrix with the value of each cell as the number of web pages that refer to that webpage? It makes sense to use this system. Now we have a matrix and we have to optimize the system. What should we use to find the order of the importance of this system or in other words how can we have a vector that contains index values for each row of this matrix? The answer to this is to use the eigenvalue pair. This finds us a set of vectors. Each of which contains the rank of the values.

### A good reference to this method is in this research page from the University of Pennsylvania by Herbert S. Wilf:  https://www2.math.upenn.edu/~wilf/website/KendallWei.pdf

#### Notes:
- If you want to restart the Page Rank calculations without re-spidering the web pages, you can use spreset.py
- No future mass commits to the main are allowed
