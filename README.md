# WEB CRAWLER
## A set of programs that emulate some functions of a search engine

### Implementation:

##### We have implemented a web crawler which asks the user for an intial webpage and then crawls through that webpage and its internal links.
##### It performs multiple searches and stores its data into a sql database(spider.sqllite)
##### Ranked the search results using the Page Rank algorithm to rank the most relevant search result
##### It then creates a visualization using a json file (which has all the data dumped into it), The result is a Node Web.

#### Please check the poster file in the Repository for more information


### Visualization:

![Webpage_graph](https://user-images.githubusercontent.com/69566994/149311366-65ab9cc7-0fa9-4367-8195-59bca4f2423d.png)


### Alternative Algorithm

##### Over the summer I read about another way to find the rank of our search results. I have mentioned a method of converting the rank match algorithm as a optimization problem and solve it using Linear Algebra.
##### Now we know that the page rank algorithm uses spidering but it spiders throught an imaginary web of webpages that are all connected to one-another. What if we imagine this web as a matrix with the value of each cell as the amount of webpages that refer to that webpage. It makes sense to use this system. Now we have a matrix and we have to optimize the system. What should we use to find the order to importance of this system or in other words how can we a vector that contains index values for each row of these matrix. The answer to this is to use the eigenvalue pair. This finds us a set of vectors. Each of which contains the rank of the values.

#### Notes:
- If you want to restart the Page Rank calculations without re-spidering the web pages, you can use spreset.py
- No future mass commits to main are allowed
