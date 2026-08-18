---
title: "Lee, D., Hosanagar, K., & Nair, H. S. (2018). Advertising content and consumer engagement on social media-Evidence from Facebook. Management Science"
source_file: "Lee, D., Hosanagar, K., & Nair, H. S. (2018). Advertising content and consumer engagement on social media-Evidence from Facebook. Management Science.pdf"
---

```
This article was downloaded by: [128.227.24.141] On: 19 January 2018, At: 04:10
Publisher: Institute for Operations Research and the Management Sciences (INFORMS)
INFORMS is located in Maryland, USA
```

# **`Management Science`** 

```
Publication details, including instructions for authors and subscription information:
http://pubsonline.informs.org
```

```
Advertising Content and Consumer Engagement on Social
Media: Evidence from Facebook
```

```
Dokyun Lee, Kartik Hosanagar, Harikesh S. Nair
```

## **`To cite this article:`** 

```
Dokyun Lee, Kartik Hosanagar, Harikesh S. Nair (2018) Advertising Content and Consumer Engagement on Social Media:
Evidence from Facebook. Management Science
```

```
Published online in Articles in Advance 18 Jan 2018
```

```
.  https://doi.org/10.1287/mnsc.2017.2902
```

## **`Full terms and conditions of use:`** **<u>`http://pubsonline.informs.org/page/terms-and-conditions`</u>** 

```
This article may be used only for the purposes of research, teaching, and/or private study. Commercial use
or systematic downloading (by robots or other automatic processes) is prohibited without explicit Publisher
approval, unless otherwise noted. For more information, contact permissions@informs.org.
```

```
The Publisher does not warrant or guarantee the article’s accuracy, completeness, merchantability, fitness
for a particular purpose, or non-infringement. Descriptions of, or references to, products or publications, or
inclusion of an advertisement in this article, neither constitutes nor implies a guarantee, endorsement, or
support of claims made of that product, publication, or service.
```

```
Copyright © 2018, INFORMS
```

## **`Please scroll down for article—it is on subsequent pages`** 

```
INFORMS is the largest professional society in the world for professionals in the fields of operations research, management
science, and analytics.
```

```
For more information on INFORMS, its publications, membership, or meetings visithttp://www.informs.org
```

**MANAGEMENT SCIENCE** **_Articles in Advance_** , **pp. 1–27 ISSN 0025-1909 (print), ISSN 1526-5501 (online)** 

**http://pubsonline.informs.org/journal/mnsc/** 

# **Advertising Content and Consumer Engagement on Social Media: Evidence from Facebook** 

### **Dokyun Lee,**<sup>**a**</sup> **Kartik Hosanagar,**<sup>**b**</sup> **Harikesh S. Nair**<sup>**c, d**</sup> 

**a** Tepper School of Business, Carnegie Mellon University, Pittsburgh, Pennsylvania 15213; **b** The Wharton School, University of Pennsylvania, Philadelphia, Pennsylvania 19104;<sup>**c**</sup> Stanford Graduate School of Business, Stanford University, Stanford, California 94305;<sup>**d**</sup> JD.com American Technologies Corporation USA, Santa Clara, California 95054 **Contact:** dokyun@cmu.edu, http://orcid.org/0000-0002-3186-3349 (DL); kartikh@wharton.upenn.edu (KH); harikesh.nair@stanford.edu (HSN) 

|**Received:** June 2, 2014<br>**Revised:** September 15, 2015; July 22, 2016;<br>February 13, 2017; June 6, 2017<br>**Accepted:** July 14, 2017<br>**Published Online in Articles in Advance:**<br>January 18, 2018|**Abstract.** We describe the efect of social media advertising content on customer engage-<br>ment using data from Facebook. We content-code 106,316 Facebook messages across<br>782 companies, using a combination of Amazon Mechanical Turk and natural language<br>processing algorithms. We use this data set to study the association of various kinds<br>of social media marketing content with user engagement—defned as _Likes_, comments,<br>shares, and click-throughs—with the messages. We fnd that inclusion of widely used|
|---|---|
|**https://doi.org/10.1287/mnsc.2017.2902**<br>**Copyright:** © 2018 INFORMS|content related to brand personality—like humor and emotion—is associated with higher<br>levels of consumer engagement (_Likes_, comments, shares) with a message. We fnd that<br>directly informative content—like mentions of price and deals—is associated with lower<br>levels of engagement when included in messages in isolation, but higher engagement<br>levels when provided in combination with brand personality–related attributes. Also, cer-<br>tain directly informative content, such as deals and promotions, drive consumers’ path<br>to conversion (click-throughs). These results persist after incorporating corrections for<br>the nonrandom targeting of Facebook’s EdgeRank (News Feed) algorithm and so refect<br>more closely user reaction to content than Facebook’s behavioral targeting. Our results<br>suggest that there are benefts to content engineering that combines informative charac-<br>teristics that help in obtaining immediate leads (via improved click-throughs) with brand<br>personality–related content that helps in maintaining future reach and branding on the<br>social media site (via improved engagement). These results inform content design strate-<br>gies. Separately, the methodology we apply to content-code text is useful for future studies<br>utilizing unstructured data such as advertising content or product reviews.|
||**History:** Accepted by Chris Forman, information systems.<br>**Funding:** The authors gratefully acknowledge fnancial support from the Jay H. Baker Retailing Cen-<br>ter and Mack Institute of the Wharton School, and the Wharton Risk Center (Russell Ackof<br>Fellowship).<br>**Supplemental Material:** The online appendix is available athttps://doi.org/10.1287/mnsc.2017.2902.|

**Keywords: consumer engagement • social media • advertising content • content engineering • marketing communication • machine learning • natural language processing • selection • Facebook • EdgeRank • News Feed algorithm** 

## **1. Introduction** 

Social networks are increasingly taking up a greater share of consumers’ time spent online. As a result, social media—which includes advertising on social networks and/or marketing communication with social characteristics—are becoming a larger component of firms’ marketing budgets. As firms increase their social media activity, the role of _content marketing_ (or _content engineering_ ) has become important. Content marketing seeks to develop content that better engages targeted users and drives the desired goals of the marketer. 

This raises the question: What content works best? Surprisingly, this problem is understudied. The most important body of academic work on this topic is the applied psychology and consumer behavior literature that discuss ways in which the content of marketing communication engages consumers and captures 

attention. However, most of this work is implemented primarily in laboratory settings. Relatively little has been explored systematically about the empirical consequences of advertising and promotional content in _real-world, field settings_ outside the laboratory. Despite its obvious relevance to practice, advertising content is also relatively underemphasized in economic theory. Economic models of directly informative advertising (see Butters 1977, Grossman and Shapiro 1984) typically allow for advertising to inform agents only about price and product existence—yet, casual observation and studies in lab settings (see Armstrong 2010, Berger 2014) suggest that advertisements contain information and content beyond prices. Canonical models of advertising in which advertising acts as a signal of quality (see Nelson 1974, Kihlstrom and Riordan 1984, Milgrom and Roberts 1986) do not emphasize 

1 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

2 

content because advertising intensity conveys the relevant information about product quality in equilibrium to market participants. In this paper, we explore the role of content in driving consumer engagement in social media in a large-scale field setting. We document that a variety of emotional, humorous, and directly informative advertising content attributes are associated with consumer engagement, and investigate how the role of content varies across engagement types. The richness of the engagement data and the ability to content-code messages in a cost-efficient manner enable us to explain these associations at a larger scale than much of previous literature on the topic. 

Our analysis is of relevance to industry in improving firms’ social media marketing strategies. Many industry surveys (e.g., Ascend2 2013, _eMarketer_ 2013) report that achieving engagement on large audience platforms like Facebook is key to these strategies. Marketing agencies’ financial contracts are also often negotiated on the basis of the engagement the agencies attain for their clients. In the early days of the industry, it was thought that engagement was primarily driven by the volume of users socially connected to the brand. Accordingly, firms aggressively acquired followers on platforms like Facebook by investing in paid ads that increased the _reach_ of their messages on the platform. However, this strategy shifted as audits of data (e.g., Creamer 2012) showed that only a small percentage of an average firm’s Facebook fans demonstrated any engagement with the brand by _Liking,_ sharing, or commenting on such messages. As a result, industry attention expanded from the mere acquisition of social media followers, per se, to the design of content that achieves both better reach and engagement among social media followers. The development of filtering algorithms by Facebook, which implied that the engagement obtained by a firms’ messages determine their future reach on the platform accelerated this trend.<sup>1</sup> While attention in the industry has shifted toward content in this manner, we still do not understand precisely what kinds of content work better for which firms and in what ways. For example, are messages seeking to inform consumers about product or price attributes more effective than persuasive messages with humor or emotion? Do messages explicitly soliciting user response (e.g., “ _Like_ this post if . . . ”) draw more engagement or in fact turn users away? Does the same strategy work for different engagement types? Our paper explores these kinds of questions systematically and contributes to the formulation of better content marketing policies in practice.<sup>2</sup> 

Our empirical investigation in this paper pertains to social media marketing on Facebook. Most top brands maintain a Facebook page on which they serve posts and messages to connected users. This form of free social media marketing has increasingly become 

an important channel for firms. The data comprise information on about 100,000 such messages posted by a panel of about 800 firms over an 11-month period between Sept 2011 and July 2012. For each message, the data also contains time-series information on two kinds of engagement measures— _Likes_ and comments—observed on Facebook. In addition, we have cross-sectional data on shares and click-throughs. We supplement these engagement data with message attribute information that we obtain using a survey we implement on Amazon Mechanical Turk (henceforth “AMT”), combined with a natural language processing algorithm (henceforth “NLP”) we built to tag messages. Three aspects make this a helpful setting to study the role of content in social media marketing. First, Facebook messages have a variety of content attributes but are short and to the point, so it is feasible to encode most of the attributes for research purposes without incurring overwhelming time or cost that may otherwise preclude a large-scale investigation. Second, Facebook requires real names and, therefore, data on user activity on Facebook is often more reliable compared to other social media sites. Third, user engagement is measured on a daily basis (panel data) at the message level. The measurement is accurate because it represents precise tracking within a closed system. 

The strategy for classifying content we adopt is motivated by the psychology, marketing, and economic literature on advertising (see Cialdini 2001, Bagwell 2007, Berger 2014, Chandy et al. 2001, and Vakratsas and Ambler 1999 for some overviews). In the economics literature, it is common to classify advertising as informative (shifting beliefs about product existence or prices) or persuasive (shifting preferences directly). This classification is difficult to operationalize for two reasons. Firstly, the basis of informative content is typically limited to prices and/or existence, and exactly what content is “persuasive” is usually not well defined and is treated as a catch-all without finer classification. Secondly, some content can be both “persuasive” and indirectly “informative” (e.g., Sahni et al. 2016). For instance, the fact that many people in a consumer’s social group are using the product may persuade the consumer to use the product (i.e., it is “persuasive”) or provide a signal that it is a good match with consumers like him (i.e., it is “ _indirectly_ informative”). 

To avoid these difficulties, we use a grouping of the content attributes that reflect the type of content we see on Facebook and parallels finer classification schema that has appeared in the advertising literature. Here, we follow the work of Resnik and Stern (1977), who operationalize directly informative advertising based on the number of informational cues present in a message (see Abernethy and Franke 1996 for several studies in this stream). Some criteria Resnik and Stern (1977) suggest for classifying content as directly informative 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

3 

are whether it includes details about products, promotions, availability, price, and product-related aspects that could be used in optimizing the purchase decision. Following this stream, any product-oriented facts, and brand and product mentions, are categorized as directly informative content. 

The other types of content we see in Facebook posts involve aspects of brand personality. For instance, we observe thousands of posts from firms that contain humor, emotional appeal, casual banter, or discussion of the brand’s philanthropic outreach. We interpret these as attempts by the firm to establish a brand personality—i.e., “a set of human characteristics associated with the brand” (Aaker 1997, Weiss and Huber 2000). One reason firms may be using such content is that consumers tend to choose brands that are in congruence with their own personalities (Govers and Schoormans 2005). Further, the branding literature suggests that functional benefits of a brand also become more persuasive when expressed by the brand’s personality (Keller 1993, Aaker 1996). Overall, we see the role of this type of content as attempts by firms to promote relationship building and to persuade consumers to adopt their brand via such relationships. 

Finally, we also present results for each content attribute separately so that the reader can judge disaggregate effects without the need for any ex post grouping. 

Estimation of the effect of content on subsequent engagement is complicated by the nonrandom allocation of messages to users. A typical concern for empirical work in such settings is of reverse causality—that firms target specific content to selected subaudiences— so the subsequent covariation in outcomes reflect both the effect of the content and the targeting policies of the firms (e.g., Nair et al. 2017). This concern is not first order in our context because unlike Facebook’s banner advertisements or sponsored posts, the Facebook organic page environment does not allow companies to target specific audiences. That is, a firm’s posts are meant for all of its fans. Instead, all targeting is implemented ex post by Facebook via its proprietary EdgeRank (or News Feed) algorithm, the goal of which is to present the user with a positive experience on Facebook that is not polluted with content that he does not value. EdgeRank tends to serve messages to users that are newer and expected to appeal better to his/her tastes. Hence, the main concern for inference created by targeting arises from the selection induced by EdgeRank. For instance, suppose Facebook’s targeting rule results in a particular type of post being assigned to more active users; then, we might incorrectly infer that posts of that type receive greater engagement from users. We account for this problem by developing an econometric correction for the filtering induced by EdgeRank and discussing how it can be 

incorporated into the estimation procedure. The correction serves as a semiparametric “control function” for the nonrandom selection induced by the filtering algorithm. We discuss other endogeneity concerns and robustness to additional threats to validity later in the paper. 

Our main finding is that brand personality content is associated with higher levels of consumer engagement with a message, while directly informative content is associated with lower levels of engagement when included in messages in isolation but higher engagement levels when provided in combination with brand personality–related attributes. Also, certain directly informative content, such as deals and promotions, is associated with immediate leads to conversion (higher click-throughs). Combining both types of content enables the brand to obtain both the engagement and branding produced by the brand personality– related content, as well as the immediate leads produced by directly informative content, along with any additional engagement they generate in combination. This finding is of substantive interest because many firms in our data post messages with one content type or the other, rather than in combination. Our results suggest, therefore, that there may be gains to content engineering by combining characteristics. Using only brand personality–related content drives engagement but also involves foregoing some of the benefits of obtaining leads and direct response. Similarly, using only directly informative content in posts is counterproductive because it reduces engagement and thus reduces future reach because of the intermediating role of EdgeRank’s filtering. This seems to be the main trade-off between these two content types on the Facebook platform. Combining characteristics achieves a balanced trade-off between reach and website visits. Our empirical results also unpack these effects into component attribute effects. 

We end this introduction with three caveats. First, we do not address the separate but important question of how engagement affects product demand and firms’ sales so as to complete the link between ad attributes and those outcome measures. The reader should note that the data required for the analysis of this question at a scale comparable to this study are still not widely available to researchers. Further, as mentioned, firms and advertisers care about engagement per se and are willing to invest in social media marketing for generating engagement, rather than caring only about sales. One interpretation is that advertising is a dynamic problem, and one of its roles is to build long-term brand capital for the firm. To the extent that the brand capital is generated by intermediary activities like increased consumer engagement, increased awareness, and inclusion in the consumer consideration set, studying the formation and evolution of these 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

4 

intermediary activities—like engagement—is useful to understanding the mechanisms by which advertising affects sales in market settings. Finally, other papers (such as Goh et al. 2013, Rishika et al. 2013, Sunghun et al. 2015), as well as industry reports (comScore 2013, Chadwick-Martin-Bailey 2010, HubSpot 2013), have linked the social media engagement measures we consider to customer acquisition, sales, and profitability metrics. 

Secondly, a caveat to our selection correction is that it is built on prior (but imperfect) knowledge of how EdgeRank is implemented. In the absence of additional experimental/exogenous variation, we are unable to address all possible issues with possible nonrandom assignment perfectly. We view our work as an exploratory study of content variables in social media that could be the basis of further rigorous testing and causal assessment, albeit at a more limited scale. A fully randomized large-scale experiment that provides a cross-firm and cross-page-type assessment as provided here may be impossible or cost prohibitive to implement; hence, we think a cross-page-type study based on observational field data of this sort has value.<sup>3</sup> 

Thirdly, though we consider a larger range of content attributes than the existing literature, it is practically impossible to detail the full range of possible content profiles produced on a domain as large as Facebook (or in data as large as ours). We choose content profiles that reflect issues flagged in the existing academic literature and those that are widely used by companies on Facebook. We discuss this in more detail in Section 2. 

**_Relationship to the Literature._** This paper is most closely related to the literature on advertising content. On the theory side, a number of new papers allow ad content to matter in equilibrium by augmenting the canonical signaling model in a variety of ways—e.g., Anand and Shachar (2009) by allowing ads to be noisy and targeted, Anderson and Renault (2006) by allowing ad content to resolve consumers’ uncertainty about their match value with a product, and Mayzlin and Shin (2011) and Gardete (2013) by allowing ad content to induce consumers to search for more information about a product. On the empirical side, representative papers that have investigated the effect of ad content in field settings include Bertrand et al. (2010) (effect of direct-mail ad content on loan demand), Liaukonyte et al. (2015) (effect of TV ad content on viewership and online sales), Tucker (2014) (effect of ad persuasion on YouTube video sharing), Tucker (2016) (effect of “social” Facebook ads on philanthropic participation), and Sudhir et al. (2016) (ad content in mailers soliciting charitable donations). Recent studies that have explored the effect of content more generally (and not specifically ad content) include Berger and Milkman (2012) (effect of emotional content in _New York Times_ articles on article sharing) and Gentzkow and 

Shapiro (2010) (effect of newspaper’s political content on readership). Relative to these literatures, our study makes two main contributions. First, from a managerial standpoint, we discuss the value of combining brand personality–related and directly informative content to balance reach/engagement with website clicks in social media, and demonstrate the differential effects of these types of content on consumer-oriented outcomes. This can help drive content engineering policies in firms. Second, to our knowledge, none of the prior studies on ad content have been conducted at the scale of this study, which spans several industries. We believe that the content-tagging methodology we develop, which combines surveys implemented on AMT with machine learning algorithms, provides a useful framework on which to build future studies that analyze the content of marketing communication. 

# **2. Data** 

Our data set is derived from the “Pages” feature introduced by Facebook in November 2007. Facebook pages enable companies to create profile pages and to post status updates, advertise new promotions, ask questions, and push content directly to consumers. The left panel of Figure 1 shows an example of Walmart’s Facebook page, which is typical of the type of pages large companies host. In what follows, we use the terms “pages,” “brands,” and “firms” interchangeably. Our data comprise posts served from firms’ pages onto the Facebook profiles of the users that are linked to the firm on the platform. To fix ideas, consider a typical message (see the right panel of Figure 1): “Pretty cool seeing Andy giving Monfils some love. . . Check out what the pros are wearing here: http://bit.ly/ nyiPeW.”<sup>4</sup> In this status update, a tennis equipment retailer starts with small talk, shares details about celebrities (Andy Murray and Gaël Monfils), and ends with a link to a product page. Each such message is a unit of analysis in our data. 

## **2.1. Data Description** 

**2.1.1. Raw Data and Selection Criteria.** To collect the data, we partnered with an anonymous firm, henceforth referred to as Company X, that provides analytics services to Facebook page owners by leveraging data from Facebook’s Insights. Insights is a tool provided by Facebook that allows page owners to monitor the performance of their Facebook messages. Company X augments data from Facebook Insights across a large number of client firms with additional records of daily message characteristics, to produce a raw data set comprising a message-day-level panel of messages posted by companies via their Facebook pages. The data includes two consumer engagement metrics: the number of _Likes_ for and comments on each message each day. These metrics are commonly used in industry as measures of engagement. They are also more granular 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

5 

**Figure 1.** (Color online) (Left) Example of a Firm’s Facebook Page (Walmart); (Right) Example of a Firm’s Message and Subsequent User Engagement with That Message (Tennis Warehouse) 

_Sources._ https://www.facebook.com/walmart/ and https://www.facebook.com/tenniswarehouse/. _Note._ Example is not necessarily from our data. 

than other metrics used in extant research, such as the number of fans who have _Liked_ the page. Also available in the data are the number of impressions of each message per day (i.e., the total number of users to which the message is exposed). In addition, page-day-level information such as the aggregate demographics of users (fans) who _Liked_ the page on Facebook or have ever seen messages by the page are collected by CompanyXonadailylevel.Thiscomprisesthepopulationof users to which a message from a firm can potentially be served. We leverage this information in the procedure we present later for accounting for nonrandom assignment of messages to users by Facebook. Once a firm serves a message, the message’s impressions, _Likes,_ and comments are recorded daily for an average of about 30 days (maximum: 126 days).<sup>5</sup> The raw data contain about a million unique messages by about 2,600 unique companies. 

To the best of our knowledge, these data are the most complete observational data available outside of Facebook at the time of writing. The data include details such as demographics of page fans and engaged fans, which cannot be scraped by outsiders (but are important for correcting for EdgeRank) but are available only to the page owners via Facebook’s application programming interface (API). The data also include daily snapshots of message-level engagement that Facebook provides to page owners. These daily snapshots generate the within-message variation that enables the panel analysis in our paper and is additionally collected by Company X on top of Facebook’s Insights tool. Finally, 

page owners do not have access to data on performance of any messages by other pages, unlike this data set, which spans a number of companies across sectors. 

We clean the data to reflect the following criteria: (i) only pages located in the United States, (ii) only messages written in English, and (iii) only messages with complete demographic data. After cleaning, the data span 106,316 unique messages posted by 782 companies between September 2011 and July 2012. This results in about 1.3 million rows of message-level daily snapshots recording about 450 million page fans’ responses. Removing periods after which no significant activity is observed for a message reduces this to 665,916 rows of message-level snapshots (where activity is defined as either impressions, _Likes_ , or comments). The companies in our data set are categorized into six broader page categories as per the classification used by Facebook and self-selected by page owners: Celebrities and Public Figures (e.g., Roger Federer), Entertainment (e.g., Star Trek), Consumer Products and Brands (e.g., Tesla Motors), Organizations and Company (e.g., WHO), Websites (e.g., TED), and Local Places and Businesses (e.g., Walmart). 

**2.1.2. Content-Coded Data.** We use a two-step method to label content. First, we contract with workers through AMT and tag 5,000 messages for a variety of content profiles. Subsequently, we build an NLP algorithm by combining several statistical classifiers and rule-based algorithms to extend the content-coding to the full set of 100,000 messages. This algorithm uses the 5,000 AMT-tagged messages as the training data 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

6 

set. We describe these methods in more detail later in the paper. 

Table 2 outlines the finer classification of the attributes we code up, including precise definitions, summary statistics, and the source for coding the attribute. As noted before, we broadly group the messages as directly informative, brand personality– related, or both. Some messages inform consumers about deals and discounts about products, while other messages seek to connect with consumers on a personal level to promote brand personality and form relationships, and are social in nature. We call the first type directly informative content and the second brand personality–related content. Some messages do both at the same time by including casual banter and product information simultaneously (e.g., “Are you a tea person or a coffee person? Get your favorite beverage from our website: http://www.specific-link-here.com”). 

As mentioned in the introduction, directly informative content variables are identified using the work of Resnik and Stern (1977), which provides 14 evaluative content criteria such as product price, deals, and availability to identify these in a message. In Table 2, the eight variables— _BRANDMENTION_ , _DEAL_ , _PRICECOMPARE_ , _PRICE_ , _TARGET_ , _PRODAVAIL_ , _PRODLOCATION_ , and _PRODMENTION_ —are directly informative. These variables enable us to assess the association of search attributes, brand, price, and product availability information with engagement. Brand personality– related content is chosen to reflect attributes that occur commonly in Facebook’s posts and those pointed out as important in driving consumer response in existing consumer behavior research. For example, emotional and humorous content has been identified as a driver of virality (Porter and Golan 2006, Berger 2014, Berger and Milkman 2012). Philanthropic content has been studied in the context of advertising effectiveness (Tucker 2016), and Berger and Schwartz (2011) documented that the interestingness of content, such as mentions of remarkable facts, is effective in generating word-of-mouth. The eight variables _REMFACT_ , _EMOTION_ , _EMOTICON_ , _HOLIDAYMENTION_ , _HUMOR_ , _PHILANTHROPIC_ , _FRIENDLIKELY_ , and _SMALLTALK_ 

are classified as brand personality–related. These definitions include emotional content, humor, banter, and philanthropic content. While not fully exhaustive, we attempted to cover most variables that are (1) highlighted by prior academic research to be relevant and (2) commonly discussed and used in the industry. 

Besides these main variables of interest, controls noted as important in industry reports are also profiled. This includes content that explicitly solicits readers to comment or includes blanks for users to fill out (thus providing an explicit option to facilitate engagement). Additionally, characteristics like whether the message contained photos or website links, and the type of the page owner (e.g., business organization versus celebrity) are also coded. Other message-specific characteristics and controls include metrics such as message length in characters and SMOG (“Simple Measure of Gobbledygook”), an automatically computed reading complexity index that is widely used. A higher SMOG value implies that a message is harder to read. Table 1 shows sample messages taken from Walmart’s page in December 2012 and shows how we would have tagged them. In Online Appendix 1, we include examples from different page types that are mostly informative, mostly brand personality, and mix of both. 

The reader should note that some elements of content tagging and classification are necessarily subjective and based on human judgement. We discuss our methods (which involve obtaining agreement across nine tagging individuals) in Section 2.2. All things considered, we believe that this is one of the most comprehensive attempts at tagging marketing communication–related content in the literature. 

**2.1.3. Data and Descriptive Graphics.** While there is active interest in social media, little is documented systematically about the kinds of content commonly used by firms. We start the descriptives by reporting on the type of content used by firms in our data. Table 2 reports summary statistics for the engagement variables and message characteristics of interest. Focusing first on message characteristics, one can see that messages with videos, price information, holiday mentions, 

**Table 1.** Examples of Messages and Their Content Tags 

|Sample messages|Content tags|
|---|---|
|_`Maria’s mission is helping veterans and their families`_|_PHILANTHROPIC_,_SMALLTALK_,_ASKLIKE_,_HTTP_|
|_`find employment. Like this and watch Maria’s story.`_||
|_`http://walmarturl.com/VzWFlh`_||
|_`Cheers! Let Welch’s help ring in the New Year.`_|_BRANDMENTION_,_SMALLTALK_,_HOLIDAYMENTION_,_EMOTION_|
|_`On a scale from 1–10 how great was your Christmas?`_|_SMALLTALK_,_QUESTION_,_HOLIDAYMENTION_|
|_`Score an iPad 3 for an iPad 2 price! Now at your local`_|_PRODMENTION_,_DEAL_,_PRODLOCATION_,_PRODAVAIL_,_PRICE_|
|_`store, $50 off the iPad 3. Plus, get a $30 iTunes Gift`_||
|_`Card. Offer good through 12/31 or while supplies last.`_||

_Source._ The messages are taken from 2012 December messages on Walmart’s Facebook page. 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

7 

**Table 2.** Variable Descriptions and Summary for Content-Coded Data 

|Variable|Description|Source|Mean|SD|Min|Max|
|---|---|---|---|---|---|---|
|_TAU_(τ)|Time since the post release (day)|Facebook|6.253|3.657|1|16|
|_LIKES_|Number of “_Likes_” post has obtained|Facebook|48.373|1,017|0|324,543|
|_COMMENTS_|Number of “comments” post has<br>obtained|Facebook|4.465|78.19|0|22,522|
|_IMPRESSIONS_|Number of times message was shown to<br>users (unique)|Facebook|9,969.2|129,874|1|4.5×10<sup>7</sup>|
|_SMOG_|<br>SMOG readability index (higher means<br>harder to read)|Computed|7.362|2.991|3|25.5|
|_MSGLEN_|Message length in characters|Computed|157.41|134.54|1|6,510|
|_HTTP_|Message contains a link|Computed|0.353|0.478|0|1|
|_QUESTION_|Message contains questions|Computed|0.358|0.479|0|1|
|_BLANK_|Message contains blanks (e.g., “My<br>favorite artist is __”)|Computed|0.010|0.099|0|1|
|_ASKLIKE_|Explicit solicitation for “_Likes_” (e.g.,<br>“Like if . . . ”)|Computed|0.006|0.080|0|1|
|_ASKCOMMENT_|Explicit solicitation for “comments”|Computed|0.001|0.029|0|1|
|_MSGTYPE_|Categorical message type assigned by<br>the Facebook|Facebook|||||
|—App|Application related messages|Facebook|0.099|0.299|0|1|
|—Link|Link|Facebook|0.389|0.487|0|1|
|—Photo|Photo|Facebook|0.366|0.481|0|1|
|—Status update|Regular status update|Facebook|0.140|0.347|0|1|
|—Video|Video|Facebook|0.005|0.070|0|1|
|_PAGECATEGORY_|Page category closely following<br>Facebook’s categorization|Facebook|||||
|—Celebrity|Singers, Actors, Athletes, etc.|Facebook|0.056|0.230|0|1|
|—ConsumerProduct|Consumer electronics, packaged goods,<br>etc.|Facebook|0.296|0.456|0|1|
|—Entertainment|TV shows, movies, etc.|Facebook|0.278|0.447|0|1|
|—Organization|<br>Nonproft organization, government,<br>school organization|Facebook|0.211|0.407|0|1|
|—PlaceBusiness|Local places and businesses|Facebook|0.071|0.257|0|1|
|—Website|Page about a website|Facebook|0.088|0.283|0|1|

or emoticons are relatively uncommon, while those with small talk and information about where to obtain the product ( _PRODAVAIL_ / _PRODLOCATION_ ) are very common. Figure 2 reports on the cooccurrence of the various content attributes. The patterns are intuitive. For instance,emotionalandphilanthropiccontentcooccur often; so does emotional and friend-like content as well as content that describes product deals and availability. To better describe the correlation matrix graphically, we ran cluster analysis (using hierarchical clusteringpickingthenumberofclustersusingtheaverage silhouette width). This suggested two clusters in the data. Figure 2 shows via a solid line how content types are clustered across messages. We see that brand personality–related content types and directly informative content types are roughly split into two separate clusters, suggesting that firms tend to use one or the other in their messages. Later in the paper, we show evidence suggesting that this strategy may not be optimal. 

Figure 3 shows the percentage of messages featuring a content attribute split by page type. At the time of data collection, Facebook listed six main page types and page owners self-selected into one of these six types. 

In each cell of the figure, we represent the relative percentages by the size of the bubbles. The largest bubble is _SMALLTALK_ for the celebrities category (60.4%), while the smallest is _PRICECOMPARE_ for the celebrities category (0%). This means that six in 10 messages by celebrity pages in the data have some sort of small talk (banter) and/or content that does not relate to products or brands, and that there are no messages by celebrity-owned pages that feature price comparisons. “Remarkable facts” (our definition) are posted more by firms in the entertainment category and less by local places and businesses. Consistent with intuition, consumer product pages and local places/businesses post the most about products ( _PRODMENTION_ ), product availability ( _PRODAVAIL_ ), product location ( _PRODLOCATION_ ), and deals ( _DEAL_ ). Emotional ( _EMOTION_ ) and philanthropic ( _PHILAN_ ) content have high representation in pages classified as celebrity, organization, and websites. 

We now discuss the engagement data. Figure 4 shows box plots of the log of impressions, _Likes_ , and comments versus the time (in days) since a message is released (τ). Both comments and _Likes_ taper off to zero 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

8 

**Table 2.** (continued) 

|Variable|Description|Source|Mean|SD|Min|Max|
|---|---|---|---|---|---|---|
||Brand perso|nality–related|||||
|_REMFACT_|Remarkable fact mentioned|AMT|0.527|0.499|0|1|
|_EMOTION_|Any type of emotion present|AMT|0.524|0.499|0|1|
|_EMOTICON_|Contains emoticon or net slang<br>(approximately 1,000 scraped from<br>web emoticon dictionary e.g.,<br>:D, LOL)|Computed|0.012|0.108|0|1|
|_HOLIDAYMENTION_|Mentions U.S. holidays|Computed|0.006|0.076|0|1|
|_HUMOR_|<br>Humor used|AMT|0.375|0.484|0|1|
|_PHILANTHROPIC_|Philanthropic or activist message|AMT|0.498|0.500|0|1|
|_FRIENDLIKELY_|<br>Answer to question: “Are your<br>friends on social media likely to<br>post message such as the shown”?|AMT|0.533|0.499|0|1|
|_SMALLTALK_|Contains small talk or banter<br>(defned to be content other than<br>about a product or company<br>business)|AMT|0.852|0.355|0|1|
||Directly|informative|||||
|_BRANDMENTION_|Mentions a specifc brand or<br>organization name|AMT+Comp|0.264|0.441|0|1|
|_DEAL_|Contains deals: any type of discounts<br>and freebies|AMT|0.620|0.485|0|1|
|_PRICECOMPARE_|Compares price or makes price<br>match guarantee|AMT|0.442|0.497|0|1|
|_PRICE_|Contains product price|AMT+Comp|0.051|0.220|0|1|
|_TARGET_|Message is targeted towards an<br>audience segment (e.g.,<br>demographics, certain|AMT|0.530|0.499|0|1|
||qualifcations such as “Moms”)||||||
|_PRODAVAIL_|<br>Contains information on product<br>availability (e.g., stock and release<br>dates)|AMT|0.557|0.497|0|1|
|_PRODLOCATION_|Contains information on where to<br>obtain product (e.g., link or<br>physical location)|AMT|0.690|0.463|0|1|
|_PRODMENTION_|<br>Specifc product has been mentioned|AMT+Comp|0.146|0.353|0|1|

_Notes._ To interpret the “Source” column, note that “Facebook” means the values are obtained from Facebook, “AMT” means the values are obtained from Amazon Mechanical Turk, and “Computed” means it has been either calculated or identified using online databases and rule-based methods in which specific phrases or content (e.g., brands) are matched. Finally, “AMT + Computed” means primary data have been obtained from Amazon Mechanical Turk and further augmented with online resources and rule-based methods. 

after two and six days, respectively. The rate of decay of impressions is slower. Virtually all engagements and impressions (more than 99.9%) are accounted for within 15 days of release of a message. 

Figure 5 shows the average number of _Likes_ and comments by message type (photo, link, etc.) over the lifetime of a message. Messages with photos have the highest average _Likes_ (94.7) and comments (7.0) over their lifetime. Status updates obtain more comments (5.5) on average than videos (4.6) but obtain fewer _Likes_ than videos. Links obtain the lowest _Likes_ on average (19.8) as well as the lowest comments (2.2). 

Figure 6 presents the average number of _Likes_ and comments by content attribute. Emotional messages 

obtain the most number of _Likes_ followed by messages identified as “likely to be posted by friends” (variable: _FRIENDLIKELY_ ). Emotional content also obtain the highest number of comments on average followed by _SMALLTALK_ and _FRIENDLIKELY_ . The reader should note these graphs do not account for the market size (i.e., the number of impressions a message reaches). Later, we present an econometric model that incorporates market size as well as selection by Facebook’s filtering algorithm to assess user engagement. 

# **2.2. Amazon Mechanical Turk (AMT)** 

We now describe our methodology for content-coding messages using AMT. AMT is a crowd-sourcing 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

9 

**Figure 2.** Cooccurrence of Attribute Characteristics Across Messages 

<!-- Start of picture text -->
2<br>5 26<br>1 27 35<br>1 34 38 49<br>2 35 38 48 55<br>1 32 41 51 53 58<br>1 32 41 57 61 61 71<br>1 –14 –7 –6 –10 –11 –5 –8<br>–1 –13 –7 –6 –10 –11 –7 –9 48<br>0 0 0 0 0 0 –1 –1 0 –1<br>–1 –11 –6 –3 –7 –6 –5 –5 5 6 1<br>0 20 29 33 29 33 35 38 –6 –5 0 7<br>0 1 25 41 30 31 40 45 1 2 0 7 29<br>0 6 29 47 36 40 46 51 –2 –1 0 11 34 59<br>0 14 35 52 43 48 56 59 –2 –2 0 6 37 59 69<br><!-- End of picture text -->

_Notes._ Shades in upper triangle represent correlations. Numbers in lower triangle represent the same correlations in numerical form in 100-s of units (range −100, +100). For example, the correlation in occurrence of humor and small talk across messages is 0.26 (cell [3, 2]). The dark line shows the separation into two clusters. Brand personality–related content and directly informative content attributes tend to form two separate clusters. 

marketplace for simple tasks such as data collection, surveys, and text analysis. It has now been successfully leveraged in several academic papers for 

online data collection and classification. To contentcode our messages, we create a survey instrument comprising a set of binary yes/no questions we pose to 

**Figure 3.** Bubble Chart of Broader Page-Type Category vs. Message Content 

<!-- Start of picture text -->
Websites 7 14 0 1 3 11 13 50 24 22 0 2 7 10 39 17<br>PlacesBusiness 7 5 0 1 1 2 10 40 53 39 1 7 7 18 36 31<br>Organization 21 12 0 0 2 16 14 50 44 9 0 3 8 6 28 17<br>Entertainment 17 7 1 0 3 7 12 48 46 9 0 3 5 7 24 18<br>ConsumerProduct 10 2 0 0 1 2 8 39 53 19 0 6 7 11 36 37<br>Celebrity 8 12 2 0 1 13 19 60 33 5 0 2 2 9 27 11<br>Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention<br><!-- End of picture text -->

_Notes._ Each bubble represents the percentage of messages within a row-page-type that has the column attribute computed for the 5,000 tagged messages. Larger and lighter bubbles imply a higher percentage of messages in that cell. Percentages do not add up to 100 along rows or columns as any given message can have multiple attributes included in it. The largest bubble (60.4%) corresponds to _SMALLTALK_ for the celebrity page category, and the smallest bubble (0%) corresponds to PRICECOMPARE for the celebrity category. 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

10 

**Figure 4.** Box Plots of Log(Engagement + 1) vs. Time Since Message Release 

<!-- Start of picture text -->
Log(Imp +1) vs.  �  (time since<br>post release) box plot<br>15<br>10<br>5<br>0<br>1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16<br>�<br>Log(Comment +1) vs.  �  (time since<br>post release) box plot<br>10<br>8<br>6<br>4<br>2<br>0<br>1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16<br>�<br>Log(Like +1) vs.  �  (time since<br>post release) box plot<br>12<br>10<br>8<br>6<br>4<br>2<br>0<br>1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16<br>�<br>Log(Imp +1)<br>Log(Comment +1)<br>Log(Like +1)<br><!-- End of picture text -->

_Notes._ Shown are box plots of (log) impressions, comments, and _Likes_ , respectively, versus τ. Both comments and _Likes_ taper to zero after two and six days, respectively. Impressions take longer. After 15 days, virtually all engagement and impressions (more than 99.9%) are accounted for. There are many outliers. 

workers (or “Turkers”) on AMT. To ensure high-quality responses from the Turkers, we follow several best practices identified in the literature—e.g., we obtain tags from at least nine different Turkers choosing only those who are from the United States, have more than 100 completed tasks, and an approval rate more than 97% (we also include an attention-verification question). See Online Appendices 2 and 3 for the final survey instrument and the complete list of strategies implemented to ensure output quality. 

**Figure 5.** Average _Likes_ and Comments by Message Type 

<!-- Start of picture text -->
Comment<br>80<br>Like<br>60<br>40<br>20<br>0<br>Link App Status update Video Photo<br>Note. Shown is the average number of  Likes  and comments obtained<br>by messages over their lifetime on Facebook, split by message<br>type.<br>Average count<br><!-- End of picture text -->

We computed the Cronbach’s Alphas, a commonly used interrater reliability measure, for the full set of 5,000 messages. The average Cronbach’s Alpha for our 5,000 tagged messages is 0.82 (median 0.84), above typically acceptable thresholds of 0.7. About 87.5% of the messages obtained an alpha higher than 0.7, and 95.4% higher than 0.6. For robustness, we replicated the study with only those messages with alphas above 0.7 (4,378 messages) and found that our results are qualitatively similar. At the end of the AMT step, approximately 2,500 distinct Turkers contributed to content-coding 5,000 messages. This constitutes the training data set for the NLP algorithm used in the next step. 

# **2.3. Natural Language Processing (NLP) for Attribute Tagging** 

We use NLP techniques to label message content from Facebook messages using the AMT-labeled messages as the training data. Typical steps for such labeling tasks include: (1) breaking the sentence into understandable building blocks (e.g., words or lemmas) and identifying sentence attributes similar to what humans do when reading; (2) obtaining a set of training sentences with labels tagged from a trusted source 

**Figure 6.** Average _Likes_ and Comments by Message Content 

<!-- Start of picture text -->
150 Comment<br>Like<br>100<br>50<br>0<br>Average count<br>Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention<br><!-- End of picture text -->

_Note._ Shown is the average number of _Likes_ and comments obtained by messages over their lifetime split by message content. 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

11 

identifying whether the sentences do or do not have a given content profile (in our case, this source comprise the 5,000 AMT-tagged messages); and (3) using statistical tools to infer which sentence attributes are correlated with content outcomes, thereby learning to identify content in sentences. When presented with a new set of sentences, the algorithm breaks the sentence down to building blocks, identifies sentencelevel attributes, and assigns labels using the statistical models that were fine-tuned in the training process. We summarize our method here briefly. A detailed description of the algorithms employed is presented in Online Appendix 4.<sup>6</sup> 

The use of NLP methods has gained traction recently in business research because of the readily available text data online (e.g., Netzer et al. 2012, Ghose et al. 2012). Our NLP methods closely mirror multistep methods used in the financial services industry to automatically extract financial information from textual sources (e.g., Malik et al. 2011) and are similar in flavor to winning algorithms from the recent Netflix Prize competition.<sup>7</sup> Briefly, our method combines five statistical classifiers with rule-based methods via heterogeneous “ensemble learning” to build up a final, master classifier. The _statistical classifiers_ we use are essentially binary classification machine learning models that take attributes as input and output predicted classification probabilities. We fit a variety of classifiers to our training data set. These include logistic regression with L1 regularization (which penalizes the number of attributes and is commonly used for attribute selection for problems with many attributes; see Hastie et al. 2009), Naive Bayes (a probabilistic classifier that applies Bayes theorem based on presence or absence of features), and support vector machines (a classification algorithm that works well for high dimensional problems) with L1 and L2 regularization and various kernels including linear, radial basis function, and polynomial kernels. We also utilize class-weighted classifiers and resampling methods to account for imbalance in positive and negative labels. The _rulebased methods_ we use are essentially algorithms that use large data sources (a.k.a. dictionaries) or specific _ifthen_ rules inputted by human experts to scan through particular words or occurrences of linguistic entities in the messages to generate a classification. We use a variety of rule-based methods. For example, in identifying brand and product mentions, we augment our AMT-tagged answers with several large lists of brands and products from online sources and a company list database from Thomson Reuters. Further, to increase the range of our brand name and product database, we also ran a separate AMT study with 20,000 messages in which we asked AMT Turkers to identify any brand or product name included in the message. We added all of the brand and product names we harvested this 

way to our look-up database. We then utilize a set of rules to identify brand and product mentions by looking up these lists. Similarly, in identifying emoticons in the messages, we use large dictionaries of text-based emoticons freely available on the Internet. 

Finally, we combine the classifications from the many classifiers and rule-based algorithms we use together via ensemble learning methods. Combining classifiers this way has several advantages since a single statistical classifier cannot successfully overcome the classical precision-recall trade-off inherent in the classification problem.<sup>8</sup> The final combined classifier has higher precision and recall than any of the constituent classifiers. 

**_Assessment._** We assess the performance of the overall NLP algorithm on three measures—viz., accuracy, precision, and recall (as defined in Endnote 8) using tenfold cross-validation. Table 3 shows these metrics for different content profiles. The performance is very good and comparable to performance achieved by the leading financial-information text-mining systems (Malik et al. 2011). We also report the improvement of the final ensemble learning method relative to using only a support vector machine classifier. As shown, the gains from combining classifiers are substantial. We obtain similar results for negative class labels. 

As a final point of assessment, note that several papers in the management sciences using NLP methods implement _unsupervised_ learning that does not require human-tagged data. These techniques use existing databases such as WordNet (lexical database for English) or tagged text corpus (e.g., tagged Brown Corpus) to learn content by patterns and correlations. _Supervised_ NLP instead utilizes human taggers to obtain a set of data that can be used to train the algorithm by examples. Unsupervised NLP is inexpensive, but its performance is relatively poorer compared to that of supervised NLP algorithms. One of the goals of this paper is to demonstrate how to utilize AMT in combination with ensemble learning techniques to produce robust supervised learning algorithms that perform well at the scale required for empirical work. We believe that the method will be useful in studies on unstructured language data such as ad content or product reviews. 

# **3. Empirical Strategy** 

Our empirical goal is to investigate the effect of message ad content on subsequent customer engagement. Engagement—the _y_ variable—is observed in the data; and content—the _x_ variable—has been tagged as above and is also observed. If messages are randomly allocated to users, the issue of assessing the effect of message content on engagement is straightforward; one simply projects _y_ on _x_ . Unfortunately, a complication 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

12 

**Table 3.** Performance of Text Mining Algorithm on 5,000 Messages Using Tenfold Cross-Validation 

||<br>le<br>perfo|With ensemble<br>arning (the best<br>rming algorithm)||Withou<br>(supp<br>versi|t ensemble lear<br>ort vector mach<br>on 1+rule-base|ning<br>ine<br>d)|
|---|---|---|---|---|---|---|
||Accuracy|Precision|Recall|Accuracy|Precision|Recall|
|_REMFACT_|0.94|0.99|0.68|0.88|0.99|0.33|
|_EMOTION_|0.97|0.99|0.87|0.94|0.98|0.65|
|_HUMOR_|0.98|1|0.90|0.97|1|0.14|
|_PHILANTHROPIC_|0.97|0.99|0.85|0.93|0.99|0.62|
|_FRIENDLIKELY_|0.94|0.99|0.68|0.90|0.99|0.41|
|_SMALLTALK_|0.85|0.88|0.80|0.78|0.34|0.28|
|_DEAL_|0.94|0.99|0.65|0.90|1|0.43|
|_PRICECOMPARE_|0.99|0.99|1|0.99|1|0.85|
|_TARGETING_|0.98|0.99|0.89|0.95|0.99|0.71|
|_PRODAVAIL_|0.96|0.99|0.76|0.91|1|0.10|
|_PRODLOCATION_|0.97|0.99|0.90|0.87|1|0.11|

_Notes._ This table presents metrics for performance of the classification algorithms used. The left three columns show the metrics for the final algorithm which combines classifiers via ensemble learning methods, while the right three columns show the metrics for a support vector machine algorithm. Notice that the support vector machine classifier tends to have low recall and high precision. Naive Bayes tends to have high recall but low precision. Classifiers on their own cannot successfully overcome the standard precision-recall trade-off (if one is higher, the other is lower). But combining many different classifiers with ensemble learning can increase both precision and recall. We obtain similar results for negative class labels. 

arises because Facebook’s policy of delivery of messages to users is nonrandom: users more likely to find a message appealing are more likely to see the message in their newsfeed, a filtering implemented via Facebook’s “EdgeRank” algorithm. The filtering implies a selection problem in estimation of the effect of message characteristics on engagement—if we see that messages with photos are more likely to be commented on by users, we do not know whether this is due to consumer propensity to comment on messages with photos or whether Facebook is very effective in showing messages with photos to users who are more likely to comment on them. If we do not correct for this selection issue, our analysis will reflect how content choices affect engagement on Facebook (which, by itself, is also managerially insightful) but will fail to decouple consumer response to content from the effect of platform-specific algorithms. Algorithms can change at any time (as has happened on Facebook since our study) and are different across platforms. Therefore, correcting for EdgeRank enhances the generalizability of our findings.<sup>9</sup> 

We address the selection issue via a two-step procedure: first by building a semiparametric model of EdgeRank that delivers an estimate of the expected number of impressions a message is likely to receive; then by incorporating this model to run a selectivitycorrected projection of _Likes_ and comments on message characteristics in the second stage. For the first stage, we exploit the fact that we observe the aggregated decisions of Facebook to serve impressions to users, and that EdgeRank is based on three variables as revealed by Facebook: Type, Tie, and Time.<sup>10</sup> 

• _Type_ ( _z_ ) refers to the type of message. Facebook categorizes message type into five classes: status update, photo, video, app, or link. 

• _Tie_ ( _hijt_ ) refers to the affinity score between page _j_ (company) and the Facebook user _i_ (viewer of the message) at time _t_ , which is based on the strength and frequency of the interaction history between the user and the page. 

• _Time_ (τ) refers to the time since the message. 

Our data set contains direct observations on the variables Type and Time. Recall that the data is at the message-day level. We do not have individuallevel data on a user’s history with pages to model tie strengths. However, we exploit the fact that we have access to demographics data on the set of users who _could potentially have been shown_ a message, versus _who were actually shown_ the message. The difference reflects the selection by EdgeRank, which we utilize as a proxy measure of tie strength–based targeting. Since we do not know the exact functional form of EdgeRank’s targeting rule, we work with a semiparametric specification, utilizing flexible splines to capture the effect of EdgeRank. At the end of this step, we thus obtain a flexible approximation to EdgeRank’s targeting. In the second step, we can then measure the effect of ad content on _Likes_ and comments, by controlling for the nonrandom targeting using this first-stage model. Figure 7 shows the empirical strategy visually. The advantages of directly modeling EdgeRank this way are that (1) by separating Facebook’s impression mechanism from the effect of content on consumer engagement, our results reflect more directly consumer behavior 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

13 

**Figure 7.** Impression–Engagement Funnel 

<!-- Start of picture text -->
Page fans FB’s EdgeRank Modeled using<br>determines which generalized<br>fans to show a additive model<br>particular post to<br>using 3Ts (Time<br>Impression Type, Tie)<br>Fitted impressions<br>Fans who have<br>seen the post<br>respond based<br>Engagement on post content Aggregate<br>and type logistic<br>regression<br>2-step estimation<br><!-- End of picture text -->

_Notes._ Facebook’s EdgeRank chooses subset of page fans to show messages released by the page and fans who have seen the message engage with the message based on content and type. EdgeRank is modeled with a semiparametric model (generalized additive model), and the final engagement is estimated through aggregate logistic regression. Details of estimation are in Sections 3.1 and 3.2. 

and not Facebook’s filtering strategy; and (2) we are also able to predict which message would eventually reach more users, which, in addition to handling selection, has auxiliary managerial value for advertisers seeking greater reach. Finally, we note that our method is implemented on data obtained from firms who host content on Facebook and, therefore, our firststage analysis is feasible for individual firms. 

# **3.1. First Stage: Approximating EdgeRank’s Assignment** 

We represent message _k_ ’s type in a vector _zk_ , the time since message _k_ was released in τ _k_ , and the history of user _i_ ’s past engagement with company _j_ on Facebook in a vector _h_ . Table 4 summarizes the notation. _ijt_ 

**Table 4.** User-Level Setup Notation 

|Notation|Description|
|---|---|
|_i_|User|
|_j_|Firm|
|_k_|Message|
|_t_|Time (day)|
|_zk_|message_k_’s media type (e.g., photo, video, status<br>update, app, link)|
|τ_k_|Time since message_k_ was released|
|_hijt_|History of user_i_’s past engagement with frm _j_|
|_g_(·)<br>|EdgeRank score approximating function|
|_n_<br>(_d_)<br>_k jt_<br>|Impressions of message_k_ by page _j_at time_t_ by<br>users in demographics bin_d_|
|�<br>(_d_)<br>_jt_<br>|Number of users of demographics bin_d_who_Liked_<br>page _j_ as of time_t_|
|θ<br>(_d_)<br>0|Intercept term for each demographics_d_|
|θ<sup>(</sup><sup>_d_)</sup><br>.|Parameters in EdgeRank approximation for<br>demographics bin_d_|

To understand our procedure, let _nk jt_<sup>(</sup><sup>_d_)denotethe</sup> number of users of demographic type _d_ � 1, . . . , _D_ who were shown message _k_ by firm _j_ at time _t_ . We refer to _nk jt_<sup>(</sup><sup>_d_)asimpressions.Weobserve</sup><sup>_nk jt_directly,and</sup><sup>_n_</sup> _k jt_<sup>(</sup><sup>_d_)</sup> is indirectly reported in the data and can be reverseengineered from Company X’s reports. A description of this procedure is provided in Online Appendix 5. Let �<sup>(</sup> _jt_<sup>_d_)denotethetotalnumberofusersofdemographic</sup> type _d_ for firm _j_ on day _t_ to whom the message can potentially be delivered. �<sup>(</sup> _jt_<sup>_d_)is directly observed in the</sup> data and comprises all users of demographics _d_ who have _Liked_ the firm on Facebook. To be clear, note that _Liking_ a message is different from _Liking_ a page— _Liking_ a page provides the firm that maintains that page an opportunity to serve its messages to that user via Facebook’s Newsfeed. �<sup>(</sup> _jt_<sup>_d_)is a count of all such users.</sup> 

If posts were randomly served to users by Facebook, the demographic distribution of _nk jt_<sup>(</sup><sup>_d_)wouldbe</sup> identical to the distribution of �<sup>(</sup><sup>_d_)Thedifference</sup> _jt_<sup>.</sup> is due to EdgeRank. Now, note that by EdgeRank’s assignment rule, the aggregated impressions for demographic type _d_ , _nk jt_<sup>(</sup><sup>_d_), is an (unknown) function of liked-</sup> fans �<sup>(</sup> _jt_<sup>_d_), the tie strength between users within demo-</sup> graphic bucket _d_ and the posting firm, _hijt_<sup>(</sup><sup>_d_), the type of</sup> message _zk_ , and time since message release τ _k_ , 

We do not observe individual-level data on each user _i_ ’s interaction with every message that could be the basis of estimating Equation (1). Instead, we can construct the aggregated number of impressions and liked-fans within a set of demographic buckets in the 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

14 

data. To use this variation as a source of approximating EdgeRank, we approximate the RHS of Equation (1) as 

where we use a firm–demographic bin-specific fixed effect, θ1<sup>(</sup><sup>_d_</sup> _j_<sup>),tocapturetheeffectofuserhistory.This</sup> approximation would literally be true if all individuals within demographic bucket _d_ had the same history with firm _j_ . In practice, this is not the case, and this may induce approximation errors into the procedure, because additional history heterogeneity within demographic buckets is not modeled (or is assumed into the error term). This is a caveat to our analysis. Access to individual-level data could be the basis of improving this procedure and relaxing this assumption. We view Equation (2) as a flexible approximation that allows us to leverage the observed variation in firm-level impressions across demographics while enabling us to include firm- and demographic-level fixed effects into a procedure that best approximates EdgeRank based on what we as researchers (and firms) know about Facebook’s filtering algorithm. We will also estimate the right-hand function _gd_ (·) separately for each demographic bucket, in effect allowing for slope heterogeneity in demographics in addition to intercept heterogeneity across demographics. 

The next step relates to approximating the function _gd_ (·). Since we do not know the exact functional form of the above selection equation, we approximate the function semiparametrically via a generalized additive model (GAM) (see Hastie and Tibshirani 1990). We choose GAM as it yields a flexible yet interpretable model for our first-stage that performs well and integrates smoothly into our second-stage estimation. The GAM is a generalized linear model with additive predictors consisting of smoothed (e.g., interpolation and curve fitting) covariates. It provides increased flexibility in approximating the unknown function, _gd_ (·). The GAM fits the following flexible relationship between a set of covariates _X_ and dependent variable _Y_ , 

where µ is a link function (e.g., Gaussian, Poisson, Gamma), and _s_ 1, _s_ 2, . . . , _sp_ are nonparametric smoothing functions such as cubic splines or kernel smoothers. We model the EdgeRank selection equation for each demographic _d_ as the following: 

where _hd_ ≡ _gd_<sup>−1(·)isthe identity (Gaussian)link func-</sup> tion, θ0<sup>(</sup><sup>_d_)</sup> is an intercept term unique to each demographic, _d_ , and θ1<sup>(</sup><sup>_d_</sup> _j_<sup>)is a firm–demographic fixed effect</sup> that captures the tie strength between the firm _j_ and demographics _d_ . �<sup>(</sup> _jt_<sup>_d_)isthenumberoffansofdemo-</sup> graphic _d_ for firm _j_ at time _t_ and denotes the potential audience for a message. _s_ 1 is a cubic spline smoothing function, essentially a piecewise-defined function consisting of many cubic polynomials joined together at regular intervals of the domain such that the fitted curve and the first and second derivatives are continuous.<sup>11</sup> We fit all models via the _R_ package `mgcv` described in Wood (2006). Lastly, we can interpret the coefficients as we normally do in a generalized linear model. 

Finally, we include dummy variables for message type ( _zk_ ) and for each day since release of the message (τ _k_ ; up to 16 days), to capture the effect of message type and time since release semiparametrically. These are allowed to be _d_ -specific. We collect the set of parameters to be estimated for each demographic bucket in of the estimation procedure.a vector,θˆ.<sup>(</sup><sup>_d_),</sup><sup>_d_�1</sup> θ<sup>, . . . ,</sup> .<sup>(</sup><sup>_d_). The estimated parameter vector, denoted</sup><sup>_D_, serves as an input to the second stage</sup> 

# **3.2. Second Stage: Modeling Engagement Given Message Assignment** 

We operationalize engagement via two actions, _Likes_ and comments, on the message. The selection problem is that users can choose to _Like_ or comment on a message only if they are served impressions, which generates nonrandom censoring because impression assignment is endogenous to the action. We address the censoring by including a correction for the fact that a user is shown a message nonrandomly, estimated semiparametrically as above. Suppose Ψ<sup>ˆ(</sup> _k jt_<sup>_d_)denotes the</sup> fitted estimate from the first stage of the expected number of impressions of message _k_ for firm _j_ among users of type _d_ at time _t_ , 

We model the probability that users of type _d_ will _Like_ a message given the full set of message characteristics, _Mkt_ , as logistic with parameters Ω � (δ _d_ , δ _j_ , ψ) _d_ �1... _D_ , _j_ �1... _J_ , where δ _d_ is a fixed effect for demographic bin _d_ and δ _j_ a fixed effect for firm _j_ , 

The parameter vector, Ω, is the object of inference in the second stage.<sup>12</sup> 

We will estimate Ω by fitting the model to explain _Qk jt_ , the observed number of _Likes_ of the message in each period in the data. To see the intuition for how our correction works in the estimation, note that we 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

15 

can aggregate Equation (5) across users, so that the expected number of _Likes_ is 

with Ψ<sup>ˆ(</sup> _k jt_<sup>_d_)aretreatedasknownfromthefirststage</sup> (Equation (4)). The right-hand side is a weighted sum of logit probabilities of _Liking_ a message. Intuitively, the decision to _Like_ a message is observed by the researcher only for a subset of users who were endogenously assigned an impression by Facebook. The selection functions Ψ<sup>ˆ(</sup> _k jt_<sup>_d_)serve as weights that reweigh the prob-</sup> ability of _Liking_ to account for the fact that those users were endogenously sampled, thereby correcting for the nonrandom nature of message assignment when estimating the outcome equation. 

We could use the expectation in Equation (6) as the basis of an estimation equation. Instead, for efficiency, we estimate the parameter vector Ω by maximum likelihood. To set up the likelihood, note that the expected number of impressions of message _k_ for firm _j_ at time _t_ across _all_ demographic buckets is simply the sum 

We can obtain an estimate of the implied probability that an impression picked at random from the pool is of type _d_ , 

Thus, the probability π( _Mkt_ ; Ω) that an impression picked at random from the pool will _Like_ the message given a guess of Ω is 

Intuitively, with probability � _kt_ ( _d_ ) � ϱˆ _dkt_ , an impression is of type _d_ , and with probability � ( _Like_ | _d_ ) � π _d_ ( _Mkt_ ; Ω), an impression will _Like_ the message conditional on being type _d_ ; hence, the unconditional probability a random impression will _Like_ the message is the sum-product of these marginals and conditionals across all _D_ types. 

The number of _Likes_ is a count variable for which we specify a binomial likelihood. Accordingly, the probability that _Qk jt_ out of the Ψ<sup>ˆ</sup> _k jt_ assigned impressions are observed to _Like_ the message, and that Ψ<sup>ˆ</sup> _k jt_ − _Qk jt_ of the remaining impressions are observed not to, is binomial with probability π( _Mkt_ ; Ω): 

Maximizing the implied binomial likelihood across all of the data, treating Ψ<sup>ˆ</sup> _k jt_ as given, then delivers estimates of Ω. The intuition for the selection correction here is the same as that encapsulated in Equation (6). We can repeat the same procedure using the number of comments on the message as the dependent variable so as to recover the association of message characteristics with commenting as well. This two-step procedure thus delivers estimates of the association of message characteristics with the two outcomes of interest. Standard errors are obtained by bootstrapping both steps 1 and 2 over the entire data set.<sup>13</sup> 

**_Discussion._** The approach outlined above essentially uses the EdgeRank approximation as a control function (Heckman and Robb 1986) that corrects for the selectivity in the second stage, where we measure the effect of message characteristics on outcomes.<sup>14</sup> Intuitively, we exploit the observed discrepancy in demographic distributions between the set of individuals to whom a message could have been served, _Njt_<sup>(</sup><sup>_d_),ver-</sup> sus those who were actually served, _nk jt_<sup>(</sup><sup>_d_). The discrep-</sup> ancy reflects the filtering by EdgeRank. The first stage essentially projects this discrepancy onto messagetype, time-since-release, page, and demographic characteristics in a flexible way. This relies on partial knowledge of the assignment/selection rule to develop a model of how the nonrandom assignment of posts to users is implemented on the platform. If we knew EdgeRank perfectly, this would be the efficient (and preferred) solution to the selection problem. Since we know EdgeRank only partially, we are worried about misspecification of the control function. The flexible semiparametric first stage along with the inclusion of the page demographic–specific fixed effect mollifies to some extent concerns about bias from this misspecification. We also tried several different alternative specifications with different link functions (including linear, Poisson, and negative binomial), obtaining qualitatively similar results but inferior fit corresponding to our preferred specifications. Below, we also show that the results we obtain from the EdgeRank approximation pass several sanity checks such as time-since-post having a negative effect on the probability of a post’s being served by EdgeRank, and the fact that time coefficients monotonically decline as time-since-release of the post increases as reported in several industry studies from comScore/Wildfire. The demographic-page fixed effects, which correspond to the demographicpage “affinity” level, also coincide with expected patterns (e.g., the demographic bin that has the highest affinity with the newborn clothing page is the one corresponding to male and females 25–34, no significant effect for older demographics—discussed below). Notwithstanding these aspects, to the best of our knowledge, the full details of EdgeRank are not 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

16 

known to any firm or researcher. In our view, a “perfect” solution to the selection problem is unlikely to be achieved without full knowledge of Facebook’s targeting rule. For approaches that have a similar flavor, see Manchanda et al. (2004), Nair et al. (2017) in the context of targeted marketing; Ellickson and Misra (2010) in the context of selectivity correction in an entry game; and, in particular, Ahn and Powell (1993) for semi/nonparametric control function approaches. 

# **4. Results** 

## **4.1. First Stage** 

The first-stage model, as specified in Equation (3), approximates EdgeRank’s message assignment algorithm. We run the model separately for each of the 

14 age–gender bins used by Facebook. These correspond to two gender and seven age bins. For a given bin, the model relates the number of users of demographic type _d_ who were shown message _k_ by firm _j_ at time _t_ to the message type ( _zk_ ), days since message (τ), and tie between the firm and the user. Table 5 presents the results. The intercepts (θ0<sup>(</sup><sup>_d_))indicatethat</sup> messages by companies in our data set are shown most often to females ages 35–44, females 45–54, and males 25–34. The lowest number of impressions are for the 65+ age group. The tie between a user and a firm is proxied by a fixed effect for each firm–demographic pair. This implies 800 × 14 fixed effects corresponding to 800 firms and 14 demographic bins. For brevity, we do not present all of the estimated coefficients. For illustration, we report the coefficients for two randomly 

**Table 5.** EdgeRank Model Estimates 

|||Female|||||
|---|---|---|---|---|---|---|
||F 13–17|F 18–24<br>F 25–34|F 35–44|F 45–54|F 55–64|F 65+|
|Intercept|5.528<sup>∗∗∗</sup>|6.071<sup>∗∗∗</sup><br>6.446<sup>∗∗∗</sup>|7.165<sup>∗∗∗</sup>|7.209<sup>∗∗∗</sup>|6.133<sup>∗∗∗</sup>|4.887<sup>∗∗∗</sup>|
|Page 1 fxed|−0.210|2.458<sup>∗∗∗</sup><br>2.685<sup>∗∗∗</sup>|1.544<sup>∗∗</sup>|0.888|0.813|0.489|
|efect—Newborn<br>clothing brand|||||||
|<br>Page 2 fxed<br>efect—Protein<br>bar brand|−0.573<sup>∗∗∗</sup>|1.285<sup>∗∗∗</sup><br>1.466<sup>∗∗∗</sup>|0.928<sup>∗∗∗</sup>|0.016|1.671<sup>∗∗∗</sup>|1.518<sup>∗∗∗</sup>|
|||Message type—App|is the base||||
|Link|0.010|0.045<sup>∗∗∗</sup><br>0.063<sup>∗∗∗</sup>|0.042<sup>∗∗∗</sup>|0.051<sup>∗∗∗</sup>|0.051<sup>∗∗∗</sup>|0.048<sup>∗∗∗</sup>|
|Photo|0.253<sup>∗∗∗</sup>|0.318<sup>∗∗∗</sup><br>0.340<sup>∗∗∗</sup>|0.309<sup>∗∗∗</sup>|0.297<sup>∗∗∗</sup>|0.267<sup>∗∗∗</sup>|0.249<sup>∗∗∗</sup>|
|Status update|0.100<sup>∗∗∗</sup>|0.161<sup>∗∗∗</sup><br>0.175<sup>∗∗∗</sup>|0.152<sup>∗∗∗</sup>|0.152<sup>∗∗∗</sup>|0.129<sup>∗∗∗</sup>|0.114<sup>∗∗∗</sup>|
|Video|0.033|0.041<br>0.061<sup>∗∗</sup>|0.041|0.021|0.024|0.030|
|�<br>(_d_)<br>_jt_ <sup>(fan number)</sup>|2.0×10<sup>−6∗∗∗</sup>|1.8×10<sup>−6∗∗∗</sup><br>7.2×10<sup>−6∗∗∗</sup>|1.9×10<sup>−5∗∗∗</sup>|1.9×10<sup>−5∗∗∗</sup>|3.8×10<sup>−5∗∗∗</sup>|8.5×10<sup>−5∗∗∗</sup>|
|_s_(�<br>(_d_)<br>_jt_ <sup>) signifcance</sup>|***|***<br>***|***|***|***|***|
|_R_<sup>2</sup>|0.78|0.78<br>0.77|0.78|0.78|0.78|0.77|
|||Male|||||
||M 13–17|M 18–24<br>M 25–34|M 35–44|M 45–54|M 55–64|M 65+|
|Intercept|5.486<sup>∗∗∗</sup>|6.118<sup>∗∗∗</sup><br>7.075<sup>∗∗∗</sup>|6.635<sup>∗∗∗</sup>|6.125<sup>∗∗∗</sup>|5.151<sup>∗∗∗</sup>|4.011<sup>∗∗∗</sup>|
|Page 1 fxed<br>efect—Newborn<br>clothing brand|0.156|0.932<br>1.673<sup>∗∗</sup>|1.082|0.722|0.209|0.111|
|<br>Page 2 fxed<br>efect—Protein<br>bar brand|1.867<sup>∗∗∗</sup>|2.423<sup>∗∗∗</sup><br>0.907<sup>∗∗∗</sup><br>Message type—App|0.670<sup>∗∗∗</sup><br>is the base|1.158<sup>∗∗∗</sup>|1.575<sup>∗∗∗</sup>|1.502<sup>∗∗∗</sup>|
|Link|−0.005|0.025<sup>∗∗∗</sup><br>0.033<sup>∗∗∗</sup>|0.034<sup>∗∗∗</sup>|0.038<sup>∗∗∗</sup>|0.049<sup>∗∗∗</sup>|0.030<sup>∗∗∗</sup>|
|Photo|0.226<sup>∗∗∗</sup>|0.284<sup>∗∗∗</sup><br>0.295<sup>∗∗∗</sup>|0.277<sup>∗∗∗</sup>|0.254<sup>∗∗∗</sup>|0.230<sup>∗∗∗</sup>|0.212<sup>∗∗∗</sup>|
|Status update|0.077<sup>∗∗∗</sup>|0.124<sup>∗∗∗</sup><br>0.126<sup>∗∗∗</sup>|0.120<sup>∗∗∗</sup>|0.106<sup>∗∗∗</sup>|0.103<sup>∗∗∗</sup>|0.084<sup>∗∗∗</sup>|
|Video|0.014|0.039<br>0.044<sup>∗</sup>|0.031|0.016|0.007|0.023|
|�<br>(_d_)<br>_jt_ <sup>(fan number)</sup>|3.6×10<sup>−6∗∗∗</sup>|1.0×10<sup>−6∗∗∗</sup><br>6.7×10<sup>−6∗∗∗</sup>|2.5×10<sup>−5∗∗∗</sup>|3.8×10<sup>−5∗∗∗</sup>|5.2×10<sup>−5∗∗∗</sup>|2.3×10<sup>−4∗∗∗</sup>|
|_s_(�<br>(_d_)<br>_t_ <sup>) signifcance</sup>|***|***<br>***|***|***|***|***|
|_j_  <br>_R_<sup>2</sup>|0.79|0.80<br>0.79|0.78|0.78|0.77|0.76|

_Notes._ Presented are the coefficients obtained from 14 generalized additive models for EdgeRank, calculated for each demographic bin. There are 14 demographic (gender–age) bins provided by Facebook. F 13–17 means all females between the ages 13 and 17. Time since message (τ) and page-level fixed effects are not included in the table and are presented graphically separately. App is the base for message type. ∗ _p_ < 0.05; ∗∗ _p_ < 0.01; ∗∗∗ _p_ < 0.001. 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

17 

**Figure 8.** Page-Level Fixed Effect Estimates from Generalized Additive Model Across 14 Demographic Bins 

**Figure 9.** Time Since Message Release (τ) Coefficients from EdgeRank Model (GAM) Box Plot Across Demographics 

<!-- Start of picture text -->
Newborn clothing brand<br>Protein bar brand<br>2<br>1<br>0<br>Page-level fixed-effect from GAM<br>Female 13–17 Female 18–24 Female 25–34 Female 35–44 Female 45–54 Female 55–64 Female 65+ Male 13–17 Male 18–24 Male 25–34 Male 35–44 Male 45–54 Male 55–64 Male 65+<br><!-- End of picture text -->

<!-- Start of picture text -->
–2<br>–3<br>–4<br>–5<br>–6<br>2 3 4 5 6 7 8 9 10 11 12 13 14 15 16<br>�<br>’s from<br>�<br>EdgeRank model<br>Coefficient of<br><!-- End of picture text -->

_Notes._ Shown are the coefficients on τ across all of the demographic bins. τ � 1 is the base case, and all coefficients are significant at the highest level of _p_ < 0.001. 

_Notes._ Shown are two randomly chosen page-level fixed-effect estimates from the EdgeRank models. Only the statistically significant estimates are shown. Newborn clothing brands are positively significant for 18–24 female, 25–34 female, 35–44 female, and 25–34 male. Protein bar brands have the highest fixed effect among 18–24 male demographics. 

coefficients are negative and significant and also more negative for higher values of τ, implying that EdgeRank prefers to show more recent messages. Finally, the coefficients for number of fans, �<sup>(</sup> _jt_<sup>_d_),arepositive</sup> and significant, but they have relatively low magnitude. This is because our model includes a smoothed term of the number of fans, _s_ (�<sup>(</sup> _jt_<sup>_d_)),whichsoaksup</sup> both the magnitude and nonlinearity. The smoothed fan-numbers are all significant. 

chosen firms in Table 5. The first firm is a “newborn clothing” brand and the second is a protein bar brand. For ease of visualization, these fixed effects are shown graphically in Figure 8 (only the statistically significant coefficients are plotted). For messages by the newborn clothing brand, the most impressions are among females in the age groups 25–34, 18–24, and 35–44. Among males, ages 25–34 receive the most number of impressions. For messages by the protein bar brand, impressions are more evenly distributed across the different demographic bins, with the male 18–24 group receiving the most impressions. These estimated coefficients are consistent with our expectations for how messages for the two brands would be targeted. 

The generalized additive model of EdgeRank recovers coefficients that make intuitive sense and are consistent with claims made in several industry reports (e.g., that photos have the highest EdgeRank weight). Further, the model fit appears to be good, especially given that we have used generalized cross-validation to guard against overfitting. 

# **4.2. Second Stage** 

In the second stage, we measure the effect of content characteristics on engagement using our selectivitycorrected model from the first stage. All results in this section are based on an analysis of the entire set of about 100,000 messages (i.e., the 5,000 AMTtagged messages as well as the messages tagged using NLP). The results for only the 5,000 AMT-tagged messages are qualitatively similar and are presented in Online Appendix 6. To present the results in a simple way, we first create the two composite summary variables corresponding to brand personality–related content and directly informative content. The brand personality–related variable is obtained by adding values of _REMFACT_ , _EMOTION_ , _EMOTICON_ , _HOLIDAYMENTION_ , _HUMOR_ , _PHILANTHROPIC_ , _FRIENDLIKELY_ , and _SMALLTALK_ , resulting in a composite variable ranging from 0 to 8. The directly informative composite variable is obtained by adding values of _BRANDMENTION_ , _DEAL_ , _PRICECOMPARE_ , _PRICE_ , _TARGET_ , _PRODAVAIL_ , _PRODLOCATION_ , and _PRODMENTION_ , resulting in a composite variable ranging 

The estimates for message type are roughly the same across demographic bins. For all demographics, the photo type has the highest coefficient (around 0.25), suggesting that photos are preferred to all other media types by EdgeRank. This is likely because users have historically engaged better with photos, causing Facebook to show photos more often. The next most preferred message type is the status update with coefficients averaging around 0.12 followed by videos and links. The baseline message type, apps, is the message type that is least preferred by EdgeRank. The rank ordering of coefficients for message type does not strictly follow the rank ordering of number of messages released by firms, which is shown in Table 2. Whereas links are posted more often, photos get more impressions relative to messages of other types, clearly highlighting the role of EdgeRank. Days since message (τ) are not presented in Table 5 because of space constraints. However, Figure 9 presents a box plot of the coefficients for τ across all 14 demographic bins. All 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

18 

**Table 6.** Brand Personality–Related vs. Directly Informative 

|Variable|Comment|Like|
|---|---|---|
|_Constant_|−6.214<sup>∗∗∗</sup>(0.080)|−5.968<sup>∗∗∗</sup>(0.069)|
|_Brand related_|0.010<sup>∗∗∗</sup>(0.001)|0.035<sup>∗∗∗</sup>(0.000)|
|_Directly informative_|−0.123<sup>∗∗∗</sup>(0.001)|−0.081<sup>∗∗∗</sup>(0.000)|
|_Message Length_|−0.001<sup>∗∗∗</sup>(0.000)|−0.001<sup>∗∗∗</sup>(0.000)|
|_Brand_×_Informative_|0.020<sup>∗∗∗</sup>(0.000)|0.007<sup>∗∗∗</sup>(0.000)|
|Firm fxed efect|Yes|Yes|
|McFadden_R_<sup>2</sup>|0.442|0.471|
|Nagelkerke_R_<sup>2</sup>|0.443|0.474|
|Log-likelihood|−1,808,507.09|−12,847,725.34|
|Deviance|3,429,051.88|25,380,357.63|
|AIC|3,618,470.19|25,696,906.67|
|_N_|658,428|658,428|

_Note._ Logistic regression for {Comment, Like} with composite summary variables for brand personality–related and directly informative content. ∗∗∗ _p_ < 0.001 

from zero to eight. Table 6 shows the result of logistic regression on engagement with these composite variables and interaction of those two variables as the _x_ -s. Figure 10 also shows a smoothed density plot of the proportion of messages that have brand personality content posted by 200 randomly chosen firms. Each line represents a firm. It seems that firms utilize three type of posts (mass points in the density): heavily informative content (density on the left); heavily brand 

**Figure 10.** (Color online) Firm-Level Content Density Plot (200 Firms) vs. Informative Content 

_Notes._ For each firm, we calculate and plot the proportion of the posts that are brand personality–related—e.g., if a firm posts a message that has 2 brand personality and 3 informative content, its value would be<sup><u>2</u></sup> 5<sup>�40%. The</sup><sup>_x_axis is the brand personality content % and</sup> the _y_ axis is density. 

related content (density on the right); and mix of both (density in the middle). 

We find that inclusion of more brand personality– related content has a positive and statistically significant effect on both types of engagement; further, inclusion of more directly informative content is associated with reduced engagement. Interestingly, the interaction between brand personality–related and directly informative content is positive, implying that the negative impact of directly informative content is lessened in the presence of brand personality–related content in the message. What could explain this result? One possible reason why engagement decreases as directly informative content increases is that too much of informative content all at once may be interpreted as direct selling, which spoils the experience of consuming the platform, analogous to the way advertisements are thought of as spoiling the TV-viewing experience. Another reason may be the disconnect that such content produces with the user’s frame of mind when logging into Facebook. For instance, it may be jarring to be served content about discounts, low prices, and sales when a user logs into the platform for social interaction and for checking updates from friends and family. Another possible reason is that that users might not engage publicly with directly informative content through socially visible _Likes_ , comments, and shares. Instead, they might respond to these directly by clicking on relevant informative posts, by clicking on any links provided, and by visiting the website. This may again be driven by the disconnect between directly informative content and the rest of the social content on Facebook. Finally, the improved engagement associated with brand personality–related content may be driven by the congruence of the brand personality with consumers’ own personalities and because the benefits of a brand become more persuasive when expressed through a brand personality. Such content seems to help firms in relationship building and to persuade consumers to engage with the brand via such relationships. These are merely conjectures. Investigating the underlying mechanism is beyond the scope of the current data; nevertheless, the sign of the effect is robust across specifications. 

While Table 6 provides an easy-to-digest summarylevel result about informative and brand personality content, Table 7 breaks up the results separately by each content type and is managerially more actionable from a content marketing standpoint.<sup>15</sup> We present results for both engagement metrics ( _Likes_ /comments) as well as for models with and without the EdgeRank correction. We exclude the 16 estimated τ coefficients from the table since they are all negative and statistically significant just as in the EdgeRank model in Figure 9. We also exclude demographic fixed effects and 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

19 

**Table 7.** Aggregate Logistic Regression Results for Comments and _Likes_ 

||NO ER|COMMENT|OR|ER COM|MENT|OR|NO ER|LIKE|OR|ER L|IKE|OR|
|---|---|---|---|---|---|---|---|---|---|---|---|---|
|_Constant_|−6.441<sup>∗∗∗</sup>|(0.077)|0.002|−8.186<sup>∗∗∗</sup>|(0.077)|0.000|−4.522<sup>∗∗∗</sup>|(0.054)|0.011|−6.157<sup>∗∗∗</sup>|(0.053)|0.002|
|_SMOG_|−0.036<sup>∗∗∗</sup>|(0.000)|0.965|−0.046<sup>∗∗∗</sup>|(0.000)|0.955|−0.030<sup>∗∗∗</sup>|(0.000)|0.970|−0.043<sup>∗∗∗</sup>|(0.000)|0.958|
|_MSGLEN_|0.000<sup>∗∗∗</sup>|(0.000)|1.000|−0.000<sup>∗∗∗</sup>|(0.000)|1.000|−0.000<sup>∗∗∗</sup>|(0.000)|1.000|−0.001<sup>∗∗∗</sup>|(0.000)|0.999|
|_HTTP_|−0.322<sup>∗∗∗</sup>|(0.002)|0.725|−0.382<sup>∗∗∗</sup>|(0.002)|0.682|−0.216<sup>∗∗∗</sup>|(0.001)|0.806|−0.282<sup>∗∗∗</sup>|(0.001)|0.754|
|_QUESTION_|0.451<sup>∗∗∗</sup>|(0.001)|1.570|0.474<sup>∗∗∗</sup>|(0.001)|1.606|−0.178<sup>∗∗∗</sup>|(0.000)|0.837|−0.166<sup>∗∗∗</sup>|(0.000)|0.847|
|_BLANK_|1.014<sup>∗∗∗</sup>|(0.003)|2.757|1.059<sup>∗∗∗</sup>|(0.003)|2.883|−0.660<sup>∗∗∗</sup>|(0.002)|0.517|−0.623<sup>∗∗∗</sup>|(0.002)|0.536|
|_ASKLIKE_|−0.082<sup>∗∗∗</sup>|(0.010)|0.921|0.029<sup>∗∗</sup>|(0.010)|1.029|0.414<sup>∗∗∗</sup>|(0.003)|1.513|0.451<sup>∗∗∗</sup>|(0.003)|1.570|
|_ASKCOMMENT_|0.741<sup>∗∗∗</sup>|(0.022)|2.098|0.828<sup>∗∗∗</sup>|(0.022)|2.289|0.406<sup>∗∗∗</sup>|(0.011)|1.501|0.476<sup>∗∗∗</sup>|(0.011)|1.610|
|||||Brand pe|rsonality–|related|||||||
|_REMFACT_|0.045<sup>∗∗∗</sup>|(0.002)|1.046|0.078<sup>∗∗∗</sup>|(0.002)|1.081|−0.025<sup>∗∗∗</sup>|(0.001)|0.975|−0.016<sup>∗∗∗</sup>|(0.001)|0.984|
|_EMOTION_|0.041<sup>∗∗∗</sup>|(0.002)|1.042|0.068<sup>∗∗∗</sup>|(0.002)|1.070|0.107<sup>∗∗∗</sup>|(0.001)|1.113|0.150<sup>∗∗∗</sup>|(0.001)|1.162|
|_EMOTICON_|−0.032<sup>∗∗∗</sup>|(0.005)|0.969|−0.066<sup>∗∗∗</sup>|(0.005)|0.936|−0.055<sup>∗∗∗</sup>|(0.001)|0.946|−0.080<sup>∗∗∗</sup>|(0.001)|0.923|
|_HOLIDAYMENTION_|−0.625<sup>∗∗∗</sup>|(0.014)|0.535|−0.605<sup>∗∗∗</sup>|(0.014)|0.546|−0.241<sup>∗∗∗</sup>|(0.004)|0.786|−0.195<sup>∗∗∗</sup>|(0.004)|0.823|
|_HUMOR_|0.024<sup>∗∗∗</sup>|(0.002)|1.024|0.066<sup>∗∗∗</sup>|(0.002)|1.068|0.021<sup>∗∗∗</sup>|(0.000)|1.021|0.047<sup>∗∗∗</sup>|(0.000)|1.048|
|_PHILANTHROPIC_|−0.010<sup>∗∗∗</sup>|(0.002)|0.990|−0.010<sup>∗∗∗</sup>|(0.002)|0.990|−0.024<sup>∗∗∗</sup>|(0.001)|0.976|−0.044<sup>∗∗∗</sup>|(0.001)|0.957|
|_FRIENDLIKELY_|0.021<sup>∗∗∗</sup>|(0.002)|1.021|0.041<sup>∗∗∗</sup>|(0.002)|1.042|0.049<sup>∗∗∗</sup>|(0.001)|1.050|0.085<sup>∗∗∗</sup>|(0.001)|1.089|
|_SMALLTALK_|0.032<sup>∗∗∗</sup>|(0.002)|1.033|−0.015<sup>∗∗∗</sup>|(0.002)|0.985|0.010<sup>∗∗∗</sup>|(0.001)|1.010|−0.021<sup>∗∗∗</sup>|(0.001)|0.979|
|||||Direct|ly inform|ative|||||||
|_BRANDMENTION_|0.034<sup>∗∗∗</sup>|(0.002)|1.035|−0.014<sup>∗∗∗</sup>|(0.002)|0.986|−0.052<sup>∗∗∗</sup>|(0.001)|0.949|−0.093<sup>∗∗∗</sup>|(0.001)|0.911|
|_DEAL_|−0.074<sup>∗∗∗</sup>|(0.002)|0.929|−0.091<sup>∗∗∗</sup>|(0.002)|0.913|−0.083<sup>∗∗∗</sup>|(0.001)|0.920|−0.115<sup>∗∗∗</sup>|(0.001)|0.891|
|_PRICECOMPARE_|−0.027<sup>∗∗∗</sup>|(0.002)|0.973|−0.014<sup>∗∗∗</sup>|(0.002)|0.986|−0.019<sup>∗∗∗</sup>|(0.000)|0.981|−0.003<sup>∗∗∗</sup>|(0.000)|0.997|
|_PRICE_|−0.076<sup>∗∗∗</sup>|(0.005)|0.927|−0.158<sup>∗∗∗</sup>|(0.005)|0.854|−0.101<sup>∗∗∗</sup>|(0.002)|0.904|−0.227<sup>∗∗∗</sup>|(0.002)|0.797|
|_TARGET_|−0.043<sup>∗∗∗</sup>|(0.002)|0.958|−0.050<sup>∗∗∗</sup>|(0.002)|0.951|−0.028<sup>∗∗∗</sup>|(0.001)|0.972|−0.011<sup>∗∗∗</sup>|(0.001)|0.989|
|_PRODAVAIL_|0.047<sup>∗∗∗</sup>|(0.002)|1.048|0.011<sup>∗∗∗</sup>|(0.002)|1.011|−0.007<sup>∗∗∗</sup>|(0.001)|0.993|−0.028<sup>∗∗∗</sup>|(0.001)|0.972|
|_PRODLOCATION_|−0.037<sup>∗∗∗</sup>|(0.002)|0.964|−0.020<sup>∗∗∗</sup>|(0.002)|0.980|0.010<sup>∗∗∗</sup>|(0.001)|1.010|0.031<sup>∗∗∗</sup>|(0.001)|1.031|
|_PRODMENTION_|−0.041<sup>∗∗∗</sup>|(0.002)|0.960|−0.096<sup>∗∗∗</sup>|(0.002)|0.908|0.047<sup>∗∗∗</sup>|(0.001)|1.048|−0.025<sup>∗∗∗</sup>|(0.001)|0.975|
|||||Message ty|pe—App|is the bas|e||||||
|—Link|0.017<sup>∗∗∗</sup>|(0.003)|1.017|0.063<sup>∗∗∗</sup>|(0.003)|1.065|−0.304<sup>∗∗∗</sup>|(0.001)|0.738|−0.277<sup>∗∗∗</sup>|(0.001)|0.758|
|—Photo|0.695<sup>∗∗∗</sup>|(0.003)|2.004|0.962<sup>∗∗∗</sup>|(0.003)|2.617|0.507<sup>∗∗∗</sup>|(0.001)|1.660|0.839<sup>∗∗∗</sup>|(0.001)|2.314|
|—Status update|0.862<sup>∗∗∗</sup>|(0.004)|2.368|1.085<sup>∗∗∗</sup>|(0.004)|2.959|0.035<sup>∗∗∗</sup>|(0.001)|1.036|0.297<sup>∗∗∗</sup>|(0.001)|1.346|
|—Video|0.498<sup>∗∗∗</sup>|(0.009)|1.645|0.760<sup>∗∗∗</sup>|(0.009)|2.138|0.341<sup>∗∗∗</sup>|(0.003)|1.406|0.695<sup>∗∗∗</sup>|(0.003)|2.004|
|Page fxed efect||Yes||Ye|s||Ye|s||Y|es||
|Demo fxed efect||Yes||Ye|s||Ye|s||Y|es||
|Time (τ) fxed Efect||Yes||Ye|s||Ye|s||Y|es||
|McFadden_R_<sup>2</sup>|0|.483||0.4|43||0.5|70||0.4|84||
|Nagelkerke_R_<sup>2</sup>|0|.483||0.4|43||0.5|71||0.4|87||
|Log-likelihood|−1,7|93,387.59||−2,467,|266.11||−9,103,|960.16||−17,746|,950.54||
|Deviance|3,18|2,136.46||4,530,|762.20||17,260,|257.77||34,548|,072.83||
|AIC|3,58|8,425.18||4,936,|182.23||18,209,|570.32||35,495|,551.08||
|_N_|65|8,428||658,|428||658,|428||658|,428||

_Notes._ Presented is the aggregate logistic regression on comments and _Likes_ for both EdgeRank-corrected (ER) and uncorrected (NO ER) models for all data. OR means “odds ratio” and shows the odds ratio for the estimates left of the column. We drop companies with less than 100 panels for fixed-effects estimation. ∗∗ _p_ < 0.01; ∗∗∗ _p_ < 0.001. 

page fixed effects for space. See Online Appendix 6 for different specifications and more details. 

Scanning through the results, firstly, we observe that the estimates are directionally similar, in most cases, with and without EdgeRank correction. However, the magnitudes often change, and the relative changes are different across content types. In some instances, there are directional changes for some coefficients. We find that high reading complexity (SMOG) decreases both _Likes_ and comments, whereas shorter 

messages (MSGLEN) are _Liked_ and commented on more, albeit with a small effect size. Having links (HTTP) is associated with lower engagement, whereas asking questions (QUESTION) significantly increased comments but at the cost of _Likes_ . Using blanks in the message to encourage comments has a similar effect of increasing comments but hurting _Likes_ . Interestingly, while the odds ratio of comments increases by 60% if a message asks a question, it increases by 188% if blanks are included, suggesting that blanks are more 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

20 

**Figure 11.** Message Characteristic Coefficients for Comments and _Likes_ 

<!-- Start of picture text -->
Logistic regression coefficients of message contents for Comments Logistic regression coefficients of message contents for  Likes<br>0.05 0.1<br>0<br>0<br>–0.05<br>–0.1<br>–0.10<br>EdgeRank –0.2<br>Logistic regression coefficients –0.15 No EdgeRank Logistic regression coefficients<br>Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention<br><!-- End of picture text -->

_Notes._ Shown are the coefficients of logistic regression for both EdgeRank-corrected and uncorrected models. Only the significant coefficients are plotted. For Comments, _HOLIDAYMENTION_ has been cut off for visualization. 

effective than questions if the goal is to increase comments. Asking for _Likes_ and comments increases both _Likes_ and comments. It is clear that even these simple content variables and message characteristics impact user engagement. 

The next 16 variables in the table are the brand personality–related and directly informative content variables. Figure 11 charts the coefficients for these variables in a bar graph and demonstrates the sharp difference between brand personality–related and directly informative content types. Looking at comments, a striking pattern is that most directly informative content has a negative impact, whereas much brand personality–related content has a positive impact. The directly informative content variables with the most negative impact are _PRICE_ , _DEAL_ , and _PRODMENTION_ , with _PRICE_ having the most negative impact. The content variables with the most positive impact are EMOTION, REMFACT, and HUMOR, which are all related to brand personality. Interestingly, _HOLIDAYMENTION_ discourages comments. One possible explanation is that near holidays, all Facebook pages indiscriminately mention holidays, leading to dulled responses. For example, during Easter, the occurrence of holiday mention jumped to nearly 40% across all messages released that day compared to the average occurrence of about 1%. A similar story could be true for _EMOTICON_ and _SMALLTALK_ (i.e., too common and thus have relatively worse impact). Looking at _Likes_ , fewer brand personality–related content variables have positive impact, but the results are qualitatively similar to the comments result in that all informative content variables but one have negative impact. Among all content, EMOTION has the most positive impact on _Likes_ , just as it was the second most successful content variable for comments. Conversely, PRICE information again had the lowest coefficient for 

_Likes_ . Remarkable facts ( _REMFACT_ ), which incited the highest number of comments, are slightly negative for _Likes_ . This is likely because not all remarkable facts are “likeable.” Pages mention tragic remarkable facts to increase awareness such as “Did you know that nearly 21,000 people die of hunger every day.” Most informative content variables continue to have a negative impact (i.e., reduce engagement), while the best content for engagement is concentrated on the brand personality side. The results also highlight that there exist differences between the impact of content on _Likes_ versus Comments. 

**_Assessing the Impact of Content._** To assess these estimates, we present marginal effects of each content type by exploring the impact of the presence of a content type on lifetime engagement with a message. To do this, for each message and each content that appear in the data, we calculate the probability of engagement with and without the content included and multiply that by the total number of impressions received by that message. That is, we calculate using the full model in Table 7, [ _P_ (engagement | content � 1)− _P_ (engagement | content � 0)]×LifetimeImpressions for each message, which gives the change in lifetime engagement associated with adding that content type. We report in Figure 12 the mean of these marginal effects across all of the messages in the data, split by content type and engagement type. 

Looking at Figure 12, we see that adding, say, emotional content would add about 70 more _Likes_ and five more comments on average, all things held equal; while adding, say, deal information into a message would reduce _Likes_ by about 60 and comments by about seven on average, all things held equal. To put this in perspective, we can compare to the mean lifetime _Likes_ and comments in our data set, which are 325 and 30, suggesting that these effects are meaningful. 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

21 

**Figure 12.** Average Marginal Impact of Each Content Type on Lifetime Comments and _Likes_ 

<!-- Start of picture text -->
Lifetime engagement change averaged Lifetime engagement change averaged<br>across all posts (comments) across all posts ( Likes )<br>5.0<br>2.5 40<br>0<br>0<br>–2.5<br>–5.0 –40<br>Note. Shown is the marginal impact of each content on lifetime engagement (comments and  Likes ) averaged across all of the messages in the<br>data.<br>averaged across all posts averaged across all posts<br>Lifetime engagement change Lifetime engagement change<br>Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention<br><!-- End of picture text -->

They also differ by post: for instance, the max number of lifetime _Likes_ and comments are 422,148 and 27,557, respectively. For this message, adding emotion would bring in 113,979 more _Likes_ and 6,062 more comments, all things held equal. Leading social analytics platforms such as Wildfire currently enable page owners to optimize factors such as when and what type (e.g., photo, status update) of messages to post. By providing some guidance on how changing additional aspects of a message can change engagement, the results above can form a useful input toward the creation of better social media marketing strategies. 

# **4.3. Shares, Click-Throughs, and Additional Exploration of Results** 

These results suggest that brand personality–related content increases engagement, while directly informative content in general reduces it (unless combined with brand personality–related content). Does this imply that firms do not benefit from using directly informative content? This conclusion would be incorrect, as directly informative content could drive profitable behaviors other than engagement. For instance, consumers who appreciate the economic/utilitarian aspect of informative, direct-response messages may directly proceed to purchase the product or take other conversion actions, which are beneficial to the firm. To the extent that we observe only engagement and not conversion/sales data, these outcomes are missed by the current analysis. While it would be ideal to augment our analysis with sales data, our data partner does not have data on purchase data, and most firms do not track such information at the post level. To assess these, we augment our data with two additional pieces of information. These additional data include: 

1. Total cumulative _clicks_ from the date of release until the last date of the data on all 106,000 messages. 

2. Total cumulative _shares_ from the date of release until the last date of the data on all 106,000 messages. When we say “clicks,” we mean a click by a user that takes him to an external website. Our data set can distinguish a click to an external website from a click on a message to see more details like “X people liked this” or to expand the comments for the message. Only the former are counted here. These clicks would likely be the first step in a series of actions by the user leading to eventual purchase or some form of conversion.<sup>16</sup> Hence, they help to explore the direct response effect of informative messages. The additional shares data form another engagement variable on Facebook and enable us to check the robustness of our findings reported for _Likes_ /comments.<sup>17</sup> 

We then run the full series of models in the paper again using clicks and shares as dependent variables. Figure 13 shows the results. The figure depicts the coefficients on the content attributes from running the model with shares and clicks, respectively, as the dependent variables. Looking at the shares model, we see that the basic findings from the other engagement models are replicated—attributes with brand personality–related content like emotion and humor have positive effects on sharing the post, while direct information like mentions of deals and prices and price comparisons in particular do not obtain many shares from users. 

The results for clicks are also presented below. In contrast to the previous results, we find that the effect of deal information is now highly positive. While presenting information about deals (i.e., discounts) does not seem to elicit _Likes_ , comments, or shares, we find evidence that it increases click-through rates. The results for other content attributes are qualitatively similar to those for _Likes_ and comments. The other attribute that 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

22 

**Figure 13.** Message Characteristic Coefficients for Shares and Click-Throughs 

<!-- Start of picture text -->
Logistic regression coefficients for shares (cross-sectional) Logistic regression coefficients for clicks (cross-sectional)<br>0.2<br>0.2<br>0<br>0<br>–0.2 –0.2<br>–0.4 –0.4<br>Share Click<br>–0.6<br>Cross-sectional logistic regression coefficients Cross-sectional logistic regression coefficients<br>Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention Remfact Emotion Emoticon Holiday Humor Philan Friendlikely Smalltalk Brandmention Deal Pricecompare Price Target Prodavail Prodloc Prodmention<br><!-- End of picture text -->

_Notes._ Shown are the coefficients of logistic regression for EdgeRank-corrected models for shares and click-throughs. Only the statistically significant coefficients are plotted. 

has a positive effect on click-through is the mention of a holiday in the post (likely reflecting the presence of discounts and deals at the firm’s website during holidays). Both suggest that such information, while reducing engagement, may set the consumer on a path to conversion. These results suggest a more nuanced interpretation of the effect of brand personality–related versus directly informative content. Brand personality– related content primarily drives engagement and seems key for long-term brand building, while directly informative content drives direct response and seems key to performance marketing. 

**_Content Design._** These results then imply guidelines for better content design. Content design is driven by the goals of the campaign for the firm. Our results imply a trade-off between directly informative and brand personality–related content as one between immediate leads (click-throughs) versus future visibility in the social media site and branding (from engagement). Since brand personality–related content drives engagement and certain directly informative content drives path-to-conversion and does not reduce engagement when combined with brand personality–related content, it seems combining both together, when feasible, would form the basis of improved content engineering. Using only brand personality–related content does drive engagement, but using only this kind of content involves foregoing some of the benefits of obtaining website traffic and direct response. Similarly, using directly informative content in messages helps the firm gain direct leads, but repeating only this kind of content in post after post may be counterproductive. Such content will not only have poor social reach but, since the EdgeRank algorithm uses a firm’s current engagement to determine the future reach of the firm’s posts, repeatedly posting information-exclusive content may eventually diminish the firm’s future reach. 

Thus, while some directly informative messages help facilitate clicks and potential conversion, the difficulty is that these may occur at the cost of reducing the size of future reached-fan-base. This seems the main tradeoff between these two content types on the Facebook platform. Combining characteristics thus achieves a balanced trade-off between reach and potential conversion. We documented earlier, in Section 2.1.3, that many posts use one content type or the other in their messages. Our current results suggest that this strategy may not be optimal and that the gains from improved content management along the lines suggested above may be substantial. 

# **4.4. Robustness and Sensitivity Analysis** 

## **4.4.1. Nonrandom Targeting of Posts by Firms to Con-** 

**sumers.** We concentrated on EdgeRank-induced selection as the main difficulty in inference since we believe that the specifics of the Facebook environment makes several other sources of confounds second order compared to the effect of EdgeRank. One concern may be that firms may target content directly to specific users or subaudiences on Facebook. In our context, such direct targeting is unlikely. In contrast to Facebook’s banner advertisements or sponsored posts, the Facebook organic page environment (to which our data correspond) does not allow companies to target specific audiences. That is, any post by a firm is a candidate for all of its fans, and Facebook determines which of these fans will see the post based on its proprietary algorithm. All targeting is implicitly implemented by Facebook via EdgeRank filtering. The only platform factor that can be controlled by the firm is the time of day of release of the message. 

Nevertheless, there are subtle ways in which targeting concerns may manifest themselves. One way is that firms observe that a particular type of content receives 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

23 

significant engagement and subsequently start posting content that is similar to that. Then, new content reflects past engagement, generating an endogeneity concern related to behavioral targeting. Alternatively, certain kinds of firms may systematically pick particular kinds of content, so it may be unobserved firm effects that we are picking up in our estimates, and not content effects—another source of targeting-induced bias. To check whether our results reflect selection of particular types of posts by high-performing firms, we evaluate the diversity of content posted by firms as well as serial correlation in posts. To the extent that the diversity of posts by firms is limited, it raises the concern that certain kinds of content attributes were not used by some low- or high-performing firms. Similarly, if there is high serial correlation in posts by firms, it may reflect limited content diversity or that firms are choosing posts based on the performance of a previous post. 

To evaluate this issue, we represent each post by a company by a binary vector of length 16 (eight directly informative and eight brand personality–related) in which 1 represents that the content attribute is present (and 0 otherwise). Next, all such vectors by the same firm are simply added up to form a vector indicating overall content creation for each firm. The Herfindahl index is then calculated for each firm.<sup>18</sup> The mean Herfindahl index is 0.089, and the median is 0.088, which is just above the minimal possible value of 1/16 � 0.0625. Other concentration measures, such as Gini coefficient, also report similar patterns, which suggests that firms in our data set post different types of content. 

Similarly, to assess the extent of serial correlation in post content released by firms, we again represent each post with a vector of length 16, with each entry in the vector representing a binary variable for the presence of the 16 content attributes. For each firm, messages are ordered by release date, then the XOR function is applied to all consecutive messages to measure content similarity.<sup>19</sup> A value of 1 for the XOR function means that a content attribute that was used in a previous post is not present in the current post, and vice versa. For example, if the first post released by a firm is the vector (1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0) and the second is (0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1), then the XOR vector comparing the two is (1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1). The mean of this XOR vector is 2/16 � 0.125. Computing the mean of such XOR vectors for all sequential pairs of posts for all firms in our data produced an average value of 0.32 (median 0.33). This suggests significant variation in content by firms in our data set. Finally, firm fixed effects are included in all specifications to guard against mixing up attributedriven differences in engagement with firm-specific effects. 

**Figure 14.** Proportion of Content Posted Split Into Hour-Bin 

<!-- Start of picture text -->
0.10<br>0.08<br>0.06<br>0.04<br>0.02<br>0 5 10 15 20<br>Hour of the day<br>split into hour-bin<br>Proportion of each content<br><!-- End of picture text -->

_Note._ Each line represents 1 of 16 content types. 

A related issue is a concern that firms may be optimizing the timing of the messages. For example, say a firm wants to give an emotional message better exposure than a humorous message. If the firm knows that more people are logged onto Facebook at 3 p.m. versus 8 a.m., the firm can post the emotional message at 3 p.m. and the humorous one at 8 a.m. Our model controls for demographics and impressions to mitigate this issue on a first-order basis. We additionally check our data for evidence that firms are targeting certain times of the day to post specific content mixes. Our data show no evidence to support such timing choices. Figure 14 presents the distribution of the time of post for each of the 16 content attributes. Each line represents a different content type. This graph shows that while the volume of content has significant time-of-day dependence (such as at 5 p.m.–6 p.m. when people leave their workplace), the mix of content does not show such dependence. All distributions appear similar. In fact, none of the<sup>�16</sup> 2 � pairwise Kolmogorov–Smirnov tests were able to reject the null that the lines came from the same distribution. The figure, coupled with high diversity of content, suggests that firms in our data set were not systematically selecting content attributes by time of day. One may wonder what explains this apparent lack of sophistication. One reason may be the lack of social media analytics tools that provided contentlevel analytics to companies during the time of the data collection. Social media analytics tools available in the market at the time of data collection only provided simple timing strategies such as what time of the day to post, as reflected in the data and controlled for in our model, but not which content attributes work well or when to post specific types of content. 

**4.4.2. Omitted Message Characteristics.** A final concern is that engagement is driven by unmeasured message characteristics that cooccur with included message characteristics, generating an omitted-variables problem. This concern is plausible, but it is second order in our view to the extent that we have included a very rich set of message characteristics. We have included and/or hard-coded a large number of message characteristics (including things like emotion and humor content, which are typically thought of as being 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

24 

in the unobservables). Our approach to this problem has been to convert unobservables into observables by collecting direct data on a relatively comprehensive set of message characteristics. We assess the extent to which these omitted variables are problematic by using the residuals from the first stage as an added control in the second stage (presented in Online Appendix 6). To see this, note that the residuals in Equation (3), ϵ<sup>(</sup> _k jt_<sup>_d_),representunobservedreasonsthat</sup> users in demographic bucket _d_ would be more likely to be targeted a message _k_ by EdgeRank. As robustness, we ask whether our results on the effect of message attributes change when we control for these unobservable drivers of attractiveness of each bucket for that message. To do this, note that from our first stage, we can obtain an estimate of the residual, denoted ϵˆ<sup>(</sup><sup>_d_)</sup> _k jt_<sup>. We</sup> rerun our second-stage estimation including the estimated ϵˆ<sup>(</sup> _k jt_<sup>_d_)-sascovariatesin</sup><sup>_Mkt_inEquation(5).We</sup> can interpret the revised results as the effect of message characteristics on engagement after “controlling for” the unobserved attractiveness of each bucket for that message. Results from these alternative models (Online Appendix 6) show that the main qualitative features of our results are robust across these specifications. 

**4.4.3. Alternative Specifications.** We also run other alternative specifications, which are presented in Online Appendices 6 and 7. First, we replicate the results using only the set of 5,000 messages directly coded up by the Amazon Mechanical Turkers. Second, we assess the extent to which the parameters are stable when we drop subsets of attributes. Third is the model that includes residuals from the first stage included in the second stage. Fourth, we also run a specification with page-level random effects. Lastly, to investigate how page types might change the impact of content on engagement, we repeated the main analysis with the same specification on subsetted data on each page type as described and categorized in Table 2. We find that the nature of our results remains unchanged. 

# **5. Conclusions** 

We document through a field study on Facebook that content engineering in social media can impact on user engagement as measured by _Likes_ , comments, shares, and click-throughs for messages. Our analysis reveals that brand personality–related content, such as emotional and humorous content, is positively associated with higher engagement. This suggests that firms gain from sharing their brand personality and information about their social initiatives on social media. Further, we find that directly informative content is associated with lower engagement on social media, but that certain types of informative content can induce higher click-throughs. Thus, brand personality–related content is primarily associated with positive engagement 

and seems key for long-term brand building, while directly informative content is primarily associated with direct-response and seems key to performance marketing. This presents a challenge to marketers who seek to build a large following on social media and who seek to leverage that following to disseminate information about new products and promotions. One takeaway from our study is that these strategies work better when directly informative content is combined with brand personality–related content to balance reach and engagement on the platform. 

Because of the scale of our study (nearly 800 firms and more than 100,000 messages analyzed), we believe our results generalize and have broader applicability than usual. Nonetheless, it is important to recognize several limitations of our study. First, we note that the results from any study on consumer response to content depend on the mix of content used in the study. For example, we find that messages mentioning holidays, especially by consumer product companies, have a negative effect on engagement. This may be due to excessive use of holiday messages by firms. It is possible that the effect may be positive if firms use these kinds of messages in moderation. Similarly, we find that emotional messages have a positive impact on engagement. Here again, it is possible that this effect may reduce in the future if firms start using emotional content excessively. Hence, it is important to interpret our results in the context of the content mix used by firms and redo the analysis in the event of large-scale changes in the content mix used by firms. Ultimately, we urge managers to strike the right balance between the directly informative content (meant to drive leads and sales) and the brand personality– related content (meant to engage the consumers), especially since EdgeRank uses firms’ current engagement level to determine future reach. 

Our analysis focuses on aggregate patterns in terms of how consumers respond to social media content. While we use firm-level fixed effects in our model to capture firm heterogeneity, our results on consumer engagement ultimately reflect aggregate patterns across nearly 800 firms. Investigating slope heterogeneity in our second-stage model across 800 firms is outside of the scope of this study. Individual firms should therefore investigate whether the aggregate patterns apply to their own business. Similarly, different customer types may have different content preferences that are not reflected in aggregate results. Our demographics-level analysis reflects one aspect of customer heterogeneity. However, consumer preferences can differ in many ways that are not captured by demographics alone. Ideally, individual user-level response data can capture customer heterogeneity precisely, but data limitations preclude such an analysis. We hope 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

25 

future work can shed more insights on heterogeneity in consumer content preference. 

We used several metrics for user engagement— namely, _Likes_ and comments on messages and whether users share messages with friends or visit the link in the message. Our use of _Likes_ , comments, shares, and click-throughs is motivated both by the widespread use of these metrics as marketing goals in social media settings, and also the availability of data. Future studies that evaluate other measures of interest can add value, particularly in validating the generalizability of our findings and in exploring mechanisms underpinning the effect we describe. As noted in the introduction, we do not address the question of how engagement affects product demand and firm’s profits so as to complete the link between ad-attributes and those outcome measures. Such data are still not widely available at the scale needed for this study. Although it is not the focus of our study, it is worth highlighting that several extant studies have studied the link between Facebook engagements and sales, albeit at a smaller scale. For example, based on randomized studies, comScore (2012) reports a 38% lift in purchase for fans exposed to Starbucks on Facebook through Facebook pages or Facebook paid advertising. Similarly, studies such as Goh et al. (2013), Rishika et al. (2013), and Sunghun et al. (2015) show that social media can be used to generate growth in sales, and ROI, consumer participation, retention, and profitability, connecting social media metrics such as “comments” to financial metrics. 

The competition for consumer attention across media outlets is intense, especially on social media platforms. Consumers, in turn, are overwhelmed by the proliferation of online content, and it seems clear that marketers will not succeed without engineering this content for their audience. We hope this study contributes to improve content engineering by firms on social media sites and, more generally, creates interest in evaluating the effect of content on business outcomes. 

# **Acknowledgments** 

For comments, the authors thank seminar participants at the Information Systems Symposium Conference (January 2013), Mack Institute Conference (spring 2013), Symposium on Statistical Challenges in Electronic Commerce Research Conference (summer 2013), Workshop on Information Technologies and Systems Conference (December 2013), INFORMS Conference (October 2014), and Workshop on Information Systems and Economics conference (December 2014). The authors thank a collaborating company that wishes to remain anonymous for providing the data used in the analysis. For helpful feedback, the authors thank David Bell, Jonah Berger, Cexun Jeffrey Cai, Pradeep Chintagunta, Pedro Gardete, Arun Gopalakrishnan, Raghuram Iyengar, Carl Mela, Navdeep Sahni, Olivier Toubia, and Christophe Van den Bulte. All errors are the authors’ responsibility. 

# **Endnotes** 

> **1** In an example widely reported during the time span of our data (2011–2012), General Motors curtailed its annual spending of $10 M on Facebook’s paid ads—a vehicle for acquiring new fans for the brand—choosing instead to focus on creating content for its branded Facebook page, on which it spent $30 M (Terlep et al. 2012). 

> **2** Content marketing to obtain better reach on Facebook via firms’ pages has parallels to search engine optimization (SEO) for obtaining improved organic listings on search engines. As of December 2013 (when this paper was written), industry-leading social media analytics firms such as Wildfire (now part of Google) did not offer detailed content engineering analytics about a wide variety of social media content with real engagement data. Rather, they provided simpler analytics such as reporting engagement by the time of the day or day of the week to post and split by inclusion of pictures or videos. More recently, the content engineering industry has mushroomed and become more sophisticated in its use of analytics. 

> **3** A firm that hosts Facebook pages might run an “A/B” test in which they randomly experiment with different message types on the platform; however, such randomization of content would not address the selection issue created by Facebook’s algorithm. Conditional on random allocation of posts by a firm, whether or not users actually see the posts in their News Feed is determined by Facebook’s EdgeRank algorithm. This breaks randomization because the subset of treated users that EdgeRank chooses to show the post to is a selected sample. The researcher or advertiser cannot solve this problem; only Facebook can. 

**4** Retailer picked randomly from an online search; not necessarily from our data. 

> **5** The majority of messages do not get any impressions or engagement after seven days. After 15 days, virtually all engagement and impressions (more than 99.9%) are accounted for. 

> **6** With recent advances in deep learning (LeCun et al. 2015) and neural network text mining (Goldberg 2016), step 1 can be automated and made more scalable—see Liu et al. (2017), for example. We take a more traditional text-mining approach in this paper and manually feature-engineer sentence-level attributes. 

**7** See http://www.netflixprize.com. 

> **8** The performance of NLP algorithms are typically assessed on the basis of accuracy (the total % correctly classified), precision (out of predicted positives, how many are actually positive), and recall (out of actual positives, how many are predicted as positives). An important trade-off in such algorithms is that an increase in precision often causes a decrease in recall or vice versa. This trade-off is similar to the standard bias-variance trade-off in estimation. 

> **9** We discuss later in Section 4.4 why other sources of confounds (like direct targeting by firms) are second-order in this setting, compared to the selection induced by EdgeRank-based filtering. Section 4.4 presents some sensitivity analysis and robustness to assess these other sources of potential endogeneity bias. 

> **10** As disclosed first at the 2010 “f8” conference. For the duration of our data collection, this EdgeRank specification seems to hold from what we can gather from public announcements by Facebook. 

> **11** We also tried Poisson and negative binomial link functions (since _nk jt_ ( _d_ )<sup>isacountvariable),aswellastheidentitylinkfunctionwith-</sup> out logging the _y_ variable. Across these specifications, we found that the identity link function with log( _y_ ) resulted in the best fit, possibly because of many outliers. We also considered specifications with numerous interaction of the covariates included, but found that they were either not significant or provided trivial gains in the _R_<sup>2</sup> . Lastly, removing the extreme outliers did not change the results qualitatively. 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

26 

> **12** Allowing ψ to be _d_ -specific as well in Equation (5) is conceptually straightforward. Unfortunately, this results in parameter proliferation and trouble with convergence; hence, we settled for a more limited specification with _d_ - _j_ specific intercepts. 

> **13** To estimate the models, we utilize the `R` libraries `lme4` and `nmle` , in particular, the functions `glmer` and `nmle` , which helps fit generalized linear mixed models and nonlinear mixed models with user-defined link functions, including the logit-binomial link function used here. To guard against an incidental parameter problem in the nonlinear fixed-effects model, we drop those firms with less than 100 observations (34 firms) in the fixed-effects specifications. A simulation study by Greene (2004) based on 1,000 units and panel length � 20 shows moderate to no bias for a variety of different nonlinear models. On average, in our data, each firm had more than 1,000 observations. For more details on estimation of nonlinear and mixed models, see Cameron and Trivedi (2013). For details on the `R` packages, see http://glmm.wikidot.com/faq. 

> **14** The analogy with the “control function approach” is in the broad sense of its original usage as a function that, when conditioned on, makes a set of endogenous variable appropriately exogenous in a potentially nonlinear regression equation Heckman and Robb (1986). Heckman and Robb (1986) recognize that control functions might depend on unknown parameters, and that to operationalize a control function procedure, these parameters must be estimated in a first stage, like here. 

> **15** Note that we could allow for demographic slope heterogeneity as we did in the first stage. However, that would mean a total of 33 coefficients × 2 ( _Likes_ /comments) × 14 (demographics) � 924 coefficients, which becomes hard to interpret. We ran this model and found some heterogeneity across different demographics, but the differences were mostly in the magnitude and not in the direction. 

> **16** Upon manually inspecting around 600 randomly chosen messages (100 per each page categories), the clicks mostly led to content consumption, subscription solicitation, direct purchase page, and deal pages. Content were similar across different page categories. 

> **17** We thank the journal’s review team for encouraging us to explore these ideas further. Unfortunately, we were unable to obtain ultimate sales/conversion information. Our data partner does not have data on purchase activity occurring on the third-party websites of its clients. These data reside only with the individual firms that run the websites. 

> **18** The index is a measure of diversity that ranges from 1/ _n_ to 1, where 1 means highly concentrated. For our case, it can range from 1/16 to 1, where 1/16 means all 16 contents are equally used. 

> **19** “Exclusive OR”—i.e., “True when inputs differ.” 

# **References** 

- Aaker DA (1996) _Building Strong Brands_ (Free Press, New York). 

- Aaker J (1997) Dimensions of brand personality. _J. Marketing Res._ 34(3):347–356. 

- Abernethy AM, Franke GR (1996) The information content of advertising: A meta-analysis. _J. Advertising_ 25(2):1–17. 

- Ahn H, Powell JL (1993) Semiparametric estimation of censored selection models with a nonparametric selection mechanism. _J. Econometrics_ 58(1–2):3–29. 

- Anand B, Shachar R (2009) Targeted advertising as a signal. _Quant. Marketing Econom._ 7(3):237–266. 

- Anderson S, Renault R (2006) Advertising content. _Amer. Econom. Rev._ 96(1):93–113. 

- Armstrong S (2010) _Persuasive Advertising_ (Palgrave Macmillan, London). 

- Ascend2 (2013) Marketing strategy report: Social media. Technical report, Ascend2. 

- Bagwell K (2007) The economic analysis of advertising. Armstrong M, Porter RH, eds. _Handbook of Industrial Organization_ , Vol. 3. _Handbooks in Economics_ , 10 (North-Holland, Amsterdam), 1701–1844. 

- Berger J (2014) Word of mouth and interpersonal communication: A review and directions for future research. _J. Consumer Psych._ 24(4):586–607. 

- Berger J, Milkman KL (2012) What makes online content viral? _J. Marketing Res._ 49(2):192–205. 

- Berger J, Schwartz E (2011) What drives immediate and ongoing word-of-mouth? _J. Marketing Res._ 48(5):869–880. 

- Bertrand M, Karlan D, Mullianathan S, Shafir E, Zinman J (2010) What’s advertising content worth? Evidence from a consumer credit marketing field experiment. _Quart. J. Econom._ 125(1): 263–306. 

- Butters G (1977) Equilibrium distributions of sales and advertising prices. _Rev. Econom. Stud._ 44(3):465–491. 

- Cameron AC, Trivedi PK (2013) _Regression Analysis of Count Data_ (Cambridge University Press, New York). 

- Chadwick Martin Bailey (2010) Consumers engaged via social media are more likely to buy, recommend. 

- Chandy R, Tellis G, Macinnis D, Thaivanich P (2001) What to say when: Advertising appeals in evolving markets. _J. Marketing Res._ 38(4):399–414. 

- Cialdini R (2001) _Influence: Science and Practice_ (Allyn and Bacon, Needham Heights, MA). 

- comScore (2012) The power of like 2: How social marketing works. Technical report, comScore, Reston, VA. 

- comScore (2013) The power of like Europe: How social marketing works for retail brands. Technical report, comScore, Reston, VA. 

- Creamer M (2012) Study: Only 1% of Facebook “fans” engage with brands. _AdAge_ . (January 27), http://adage.com/article/digital/ study-1-facebook-fans-engage-brands/232351/. 

- Ellickson PB, Misra S (2010) Enriching interactions: Incorporating outcome data into static discrete games. _Quant. Marketing Econom._ 10(1):1–26. 

- _eMarketer_ (2013) Which social media marketing tactics work best? (March 26), https://www.emarketer.com/Article/Which-Social -Media-Marketing-Tactics-Work-Best/1009756. 

- Gardete PM (2013) Cheap-talk advertising and misrepresentation in vertically differentiated markets. _Marketing Sci._ 32(4):609–621. 

- Gentzkow M, Shapiro J (2010) What drives media slant? Evidence from U.S. newspapers. _Econometrica_ 78(1):35–71. 

- Ghose A, Ipeirotis PG, Li B (2012) Designing ranking systems for hotels on travel search engines by mining user-generated and crowd-sourced content. _Marketing Sci._ 31(3):493–520. 

- Goh K-Y, Heng C-S, Lin Z (2013) Social media brand community and consumer behavior: Quantifying the relative impact of user-and marketer-generated content. _Inform. Systems Res._ 24(1):88–107. 

- Goldberg Y (2016) A primer on neural network models for natural language processing. _J. Artificial Intelligence Res._ 57:345–420. 

- Govers PC, Schoormans JP (2005) Product personality and its influence on consumer preference. _J. Consumer Marketing_ 22(4): 189–197. 

- Greene W (2004) The behaviour of the maximum likelihood estimator of limited dependent variable models in the presence of fixed effects. _Econometrics J._ 7(1):98–119. 

- Grossman G, Shapiro C (1984) Informative advertising with differentiated products. _Rev. Econom. Stud._ 51(1):63–81. 

- Hastie T, Tibshirani RJ (1990) _Generalized Additive Models_ (Chapman & Hall/CRC, Boca Raton, FL). 

- Hastie T, Tibshirani R, Friedman J (2009) _The Elements of Statistical Learning: Data Mining, Inference, and Prediction_ (Springer, New York). 

- Heckman JJ, Robb R (1986) Alternative methods for solving the problem of selection bias in evaluating the impact of treatments on outcomes. Wainer H, ed. _Drawing Inferences from Self-Selected Samples_ (Springer, New York), 63–107. 

- HubSpot (2013) State of inbound marketing. Technical report, HubSpot, Cambridge, MA. 

- Keller KL (1993) Conceptualizing, measuring, and managing customer-based brand equity. _J. Marketing_ 57(1):1–22. 

**Lee, Hosanagar, and Nair:** _Advertising Content and Consumer Engagement on Social Media_ Management Science, _Articles in Advance_ , pp. 1–27, © 2018 INFORMS 

27 

- Kihlstrom R, Riordan M (1984) Advertising as a signal. _J. Political Econom._ 92(3):427–450. 

- LeCun Y, Bengio Y, Hinton G (2015) Deep learning. _Nature_ 521(7553): 436–444. 

- Liaukonyte J, Teixeira T, Wilbur KC (2015) Television advertising and online shopping. _Marketing Sci._ 34(3):311–330. 

- Liu X, Lee D, Srinivasan K (2017) Large scale cross category analysis of consumer review content on sales conversion leveraging deep learning. Working Paper 16-09, NET Institute, New York. 

- Malik HH, Bhardwaj VS, Fiorletta H (2011) Accurate information extraction for quantitative financial events. _Proc. 20th ACM Internat. Conf. Inform. Knowledge Management_ (ACM, New York), 2497–2500. 

- Manchanda P, Rossi PE, Chintagunta P (2004) Response modeling with non-random marketing mix variables. _J. Marketing Res._ 41:467–478. 

- Mayzlin D, Shin J (2011) Uninformative advertising as an invitation to search. _Marketing Sci._ 30(4):666–685. 

- Milgrom P, Roberts J (1986) Price and advertising signals of product quality. _J. Political Econom._ 94(4):796–821. 

- Nair HS, Misra S, Hornbuckle WJ IV, Mishra R, Acharya A (2017) Big data and marketing analytics in gaming: Combining empirical models and field experimentation. _Marketing Sci._ 36(5):699–725. 

- Nelson P (1974) Advertising as information. _J. Political Econom._ 82(4):729–754. 

- Netzer O, Feldman R, Goldenberg J, Fresko M (2012) Mine your own business: Market-structure surveillance through text mining. _Marketing Sci._ 31(3):521–543. 

- Porter L, Golan GJ (2006) From subservient chickens to brawny men: A comparison of viral advertising to television advertising. _J. Interactive Advertising_ 6(2):4–33. 

- Resnik A, Stern BL (1977) An analysis of informative content in television advertising. _J. Marketing_ 41(1):50–53. 

- Rishika R, Kumar A, Janakiraman R, Bezawada R (2013) The effect of customers’ social media participation on customer visit frequency and profitability: An empirical investigation. _Inform. Systems Res._ 24(1):108–127. 

- Sahni NS, Wheeler SC, Chintagunta P (2016) Personalization in email marketing: The role of non-informative advertising content. Working paper, Stanford Graduate School of Business, Stanford, CA. 

- Sudhir K, Roy S, Cherian M (2016) Do sympathy biases affect charitable giving? The effects of advertising content. _Marketing Sci._ Forthcoming. 

- Sunghun C, Animesh A, Han K, Pinsonneault A (2015) Firms’ social media efforts, consumer behavior, and firm performance: Evidence from Facebook. _CORS/INFORMS Internat. Conf., Montreal, Canada_ , 14–17. 

- Terlep S, Vranica S, Raice S (2012) GM says Facebook ads don’t pay off. _Wall Street Journal_ (May 16), https://www.wsj.com/articles/ SB10001424052702304192704577406394017764460. 

- Tucker CE (2014) The reach and persuasiveness of viral video ads. _Marketing Sci._ 34(2):281–296. 

- Tucker CE (2016) Social advertising: How advertising that explicitly promotes social influence can backfire (June 1), https://ssrn .com/abstract�1975897. 

- Vakratsas D, Ambler T (1999) How advertising works: What do we really know? _J. Marketing_ 63(1):26–43. 

- Weiss M, Huber F (2000) _The Value of Brand Personalities: The Phenomenon of the Strategic Positioning of Brands_ (German University Publishing, Wiesbaden, Germany). 

- Wood SN (2006) _Generalized Additive Models: An Introduction with R_ (CRC Press, Boca Raton, FL). 

