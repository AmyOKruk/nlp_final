# Do British tabloids treat Meghan Markle more negatively than Kate Middleton?

For my final project, I applied natural language processing techniques to investigate whether Meghan Markle has been treated more negatively by British tabloids than Kate Middleton.

To do this, I examined articles mentioning Markle and Middleton in key tabloids over the last two years. I looked at both the different words and topics associated with each woman. While sentiment analysis seemed like an obvious choice, I did not use this technique because it is unreliable, especially when applied to complex sentences with multiple subjects.

The results indicated that since 2017, the Daily Mail, The Sun and The Mirror have published many more stories about Markle than Middleton, approximately 3.5x more. This is likely due to the media frenzy over her wedding to Prince Harry in May 2018. 

While it is hard to quantify if the tabloids treatment of Markle was more negative, some interesting trends did emerge. Surprisingly,  words highly associated with Kate Middleton were “cry,” “tears,” and “suffering.” These words likely point to the narrative in the British tabloids that there is tension between the duchesses, with Meghan having ‘left Kate Middleton in tears’ over various feuds, as reported by The Sun and others.  

The results of topic modeling also suggest the tabloid’s reporting on Markle has been more politically charged than Middleton. While topics associated with Middleton largely covered family and fashion, one of Markle’s topics contained words such as 'police', 'white', 'time', 'man', 'woman', 'troops', 'afghanistan', 'trump' and  'black'. 

Overall, more analysis and exploration is needed to conclusively determine if the tabloids’ treatment of Markle is more cynical or unkind than Middleton’s.

# Methodology

# Timeframe 
I chose to collect articles published over the last two years from Nov. 27, 2017 to Nov. 27, 2019. While I originally wanted to compare the two-year period centered around each royal marriage, The Sun and The Mirror do not allow users to search for articles published earlier than around 2016. Unfortunately, Middleton's marriage was over seven years ago on April 29, 2011. Regardless, the two-year period ensured an adequate sample size of articles.

# Choosing news outlets
There are no news APIs or ready-made datasets of British tabloid articles, so I made my own. I used web scraping to collect articles about Middleton and Markle over a two-year period from Britain's top three tabloids by circulation:

# The Sun
A tabloid newspaper founded in 1964 and published in the United Kingdom and Ireland.
thesun.co.uk
circulation: 1,240,959

# Daily Mail
A daily middle-market tabloid newspaper published in London.
dailymail.co.uk
circulation: 1,166,500

# The Mirror
A national daily tabloid newspaper founded in 1903.
mirror.co.uk
circulation: 463,256 

# Collecting articles

To collect the articles, I used each tabloid website's search feature to search "Kate Middleton" and "Meghan Markle." I scraped the search results and then filtered them to include only articles that contain "Kate" and/or "Middleton" and "Meghan" and/or "Markle" in their headlines. I also filtered the articles based on my two-year timeframe of interest.

This resulted in the following number of articles:

# The Daily Mail
Kate Middleton: 724
Meghan Markle: 2,799

# The Sun
Kate Middleton: 852
Meghan Markle: 3,118

# The Mirror
Kate Middleton: 772
Meghan Markle: 2,613

# Limitations

One limitation to this analysis is that the corpus of articles about Markle is much bigger than Middleton. This is likely because Markle married Prince Harry in May 2018, generating a lot of media interest. However, since my analysis looks at topics and words associated with each woman based on their own collection of articles, Markle’s over representation is not overly problematic, although the analysis of her tabloid treatment may be more accurate than Kate’s due to the large sample size. 

Further, this analysis only considers online tabloid articles, not those found in print or published elsewhere.


 
