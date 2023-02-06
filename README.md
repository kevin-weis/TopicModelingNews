# TopicModelingNews
Project for experimenting with using BERTopic to model news articles from AP, Reuters, and CNN 


News Articles were scraped using the Scrapy package. In total, almost 30k articles were scraped, with 9-10k articles per source. 

Articles were then pre-processed using several steps and an interative process. First, texts from before 2016 were dropped. Next, articles with fewer than 100 words were dropped. I then used trigrams to help identify different common phrases in the text that were uninformative and should be dropped, e.g., blurbs of news sources describing themselves or advertising their media products. Finally, articles that were tagged by their original sources as being 'Pictures' or '24 hours in photos' were dropped. The final collection of texts ended up being around 21k articles. 

For Topic Modeling, I used BERTopic and experimented with parameters to get a distribution of topics that were useful without resulting in an overwhelming number of topics. I then visualized the topics over time. 
