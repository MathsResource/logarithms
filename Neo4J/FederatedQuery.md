Federated search is an information retrieval technology that allows the simultaneous search of multiple searchable resources. A user makes a single query request which is distributed to the search engines, databases or other query engines participating in the federation. The federated search then aggregates the results that are received from the search engines for presentation to the user. Federated search can be used to integrate disparate information resources within a single large organization ("enterprise") or for the entire web. 
Federated search, unlike distributed search, requires centralized coordination of the searchable resources. This involves both coordination of the queries transmitted to the individual search engines and fusion of the search results returned by each of them. 

Contents
1
Purpose
2
Process
3
Implementation
4
Challenges
5
See also
6
References
7
Further reading
Purpose[edit]
Federated search came about to meet the need of searching multiple disparate content sources with one query. This allows a user to search multiple databases at once in real time, arrange the results from the various databases into a useful form and then present the results to the user. 
As such, it is an information aggregation, or integration approach - it provides single point access to many information resources, and typically returns the data in a standard or partially homogenized form. Other approaches include constructing an Enterprise data warehouse, Data lake, or Data hub. Federated Search queries many times in many ways (each source is queried separately) where other approaches import and transform data many times, typically in overnight batch processes. Federated search provides a real-time view of all sources (to the extent they are all online and available). 
In industrial search engines, such as LinkedIn, federated search is used to personalize vertical preference for ambiguous queries.[1] For instance, when a user issues a query like "machine learning" on LinkedIn, he or she could mean to search for people with machine learning skill, jobs requiring machine learning skill or content about the topic. In such cases, federated search could exploit user intent (e.g., hiring, job seeking or content consuming) to personalize the vertical order for each individual user. 
Process[edit]
As described by Peter Jacso (2004[2]), federated searching consists of (1) transforming a query and broadcasting it to a group of disparate databases or other web resources, with the appropriate syntax, (2) merging the results collected from the databases, (3) presenting them in a succinct and unified format with minimal duplication, and (4) providing a means, performed either automatically or by the portal user, to sort the merged result set. 
Federated search portals, either commercial or open access, generally search public access bibliographic databases, public access Web-based library catalogues (OPACs), Web-based search engines like Google and/or open-access, government-operated or corporate data collections. These individual information sources send back to the portal's interface a list of results from the search query. The user can review this hit list. Some portals will merely screen scrape the actual database results and not directly allow a user to enter the information source's application. More sophisticated ones will de-dupe the results list by merging and removing duplicates. There are additional features available in many portals, but the basic idea is the same: to improve the accuracy and relevance of individual searches as well as reduce the amount of time required to search for resources. 
This process allows federated search some key advantages when compared with existing crawler-based search engines. Federated search need not place any requirements or burdens on owners of the individual information sources, other than handling increased traffic. Federated searches are inherently as current as the individual information sources, as they are searched in real time. 
Implementation[edit]
 

Federating across three search engines
One application of federated searching is the metasearch engine. However, the metasearch approach does not overcome the shortcomings of the component search engines, such as incomplete indexes. Documents that are not indexed by search engines create what is known as the deep Web, or invisible Web. Google Scholar is one example of many projects trying to address this, by indexing electronic documents that search engines ignore. And the metasearch approach, like the underlying search engine technology, only works with information sources stored in electronic form. 
One of the main challenges of metasearch, is ensuring that the search query is compatible with the component search engines that are being federated and combined. When the search vocabulary or data model of the search system is different from the data model of one or more of the foreign target systems, the query must be translated into each of the foreign target systems. This can be done using simple data-element translation or may require semantic translation. For example, if one search engine allows for quoting of exact strings or n-grams and the another does not, the query must be translated to be compatible with each search engine. To translate a quoted exact string query, it can be broken down into a set of overlapping [N-gram|N-grams] that are most likely to give the desired search results in each search engine. 
Another challenge faced in the implementation of federated search engines is scalability. It is difficult to maintain the performance, the response speed, of a federated search engine as it combines more and more information sources together. One implementation of federated search that has begun to address this issue is WorldWideScience, hosted by the U.S. Department of Energy's Office of Scientific and Technical Information. WorldWideScience [3] is composed of more than 40 information sources, several of which are federated search portals themselves. One such portal is Science.gov [4] which itself federates more than 30 information sources representing most of the R&D output of the U.S. Federal government. Science.gov returns its highest ranked results to WorldWideScience, which then merges and ranks these results with the search returned by the other information sources that comprise WorldWideScience.[4] This approach of cascaded federated search enables large number of information sources to be searched via a single query. 
Another application Sesam running in both Norway and Sweden has been built on top of an open sourced platform specialised for federated search solutions. Sesat,[5] an acronym for Sesam Search Application Toolkit, is a platform that provides much of the framework and functionality required for handling parallel and pipelined searches and displaying them elegantly in a user interface, allowing engineers to focus on the index/database configuration tuning. 
To personalize vertical orders in federated search, LinkedIn search engine [1] exploits the searcher's profile and recent activities to infer his or her intent, such as hiring, job seeking and content consuming, then uses the intent, along with many other signals, to rank vertical order that personally relevant to the individual searcher. 