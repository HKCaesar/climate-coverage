# climate-coverage

<h2> Motivation </h2>

To track media coverage on climate change since the 90s focusing on regional reporting during weather events, specifically droughts, hurricanes, tornadoes, and flooding. Specifically:    

Are these events increasingly discussed in the context of climate change, as the science linking it to the frequency or severity of these events has become more certain?    

How has reporting evolved, and are there regional differences?     

<h2> Brief Overview of Methodology </h2>

Tools: scrapy, selenium, pandas, MIT NER, scikit-learn, flask, D3

I scraped newspaper articles from 12 newspapers, regional (e.g. Des Moines Register, Austin American-Statesman) and national (e.g. NY Times, Fox News, USA Today), referencing droughts, hurricanes, tornadoes, or flooding. To answer the first question from above, I looked at how frequently the phrase 'climate change' or 'global warming' was mentioned over time. 

For the second question, I began by using LDA since that was most frequently referenced in the academic literature. However, I found that my topics were more coherent using tf-idf with NMF. I also found that removing locations using NER led to clearer topics for each event type. A blog post will follow soon with greater details on this process and the results!    

<h2> Final product </h2>

An interactive D3 dashboard. For a demo, check out this link: https://www.youtube.com/watch?v=h6mc1eEqTw4. Again, stay tuned for the complete dashboard!
