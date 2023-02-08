To begin, the project is implemented using Python 3.10.
For dependencies, they are inside the file requirements.txt which can be installed (preferably in a virtual environment) by
`pip install -r requirements.txt`
Once that is done, go to concordia folder by
`cd concordia`
This will start crawling ginacody website with a limit of 80 pages (scrapy actually does a little more depending on how many requests it has on the queue when it gets to 80, so it does 80 + what is in queue).  It will take around 2 min. 
`scrapy crawl concordia`
Then, this will create a folder called test_html which contains all the HTML files
What is left is just going back  
`cd ..`
Then run 
`python main.py`
Which calls all the different classes and methods to generate the txt files “Cluster_k-3.txt” and “Cluster_k-6.txt”. Inside there are the top 20 words for each cluster and the afinn score of each one.
