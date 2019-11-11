---
layout: post
title:  "A Reality Check on Redfin Estimate and Zillow Zestimate"
date:   2019-11-10 16:06:00 -0800
---

> To calculate the Redfin Estimate, Redfin evaluates hundreds of data points using proprietary machine-learning software running on next-generation cloud technology.  
> -- <cite>[Independent Study Finds Redfin Estimate to be Most Accurate Among Top Automated Home-Value Estimates](http://press.redfin.com/news-releases/news-release-details/independent-study-finds-redfin-estimate-be-most-accurate-among)</cite>

# The Truth Behind the Ever-accurate Estimates

Many of us, including the past me, may perceive [Redfin Estimate](https://www.redfin.com/redfin-estimate) and [Zillow Zestimate](https://www.zillow.com/zestimate/) as two of the most popular, and seemingly handy, home valuation tools.
Both estimation models are stated to be highly accurate. As of this writing, Redfin Estimate is claimed to have a median error rate of 1.62% for on-market homes, and 6.28% for off-market homes. What contributed to the difference in error rates for on-market and off-market homes? Redfin explains that it was due to more data available for on-market homes, which sounds reasonable.
In comparison, Zillow Zestimate's median error rates are 1.9% and 7.5% for on-market and off-market homes, respectively. 

It looks like this might be just another success story of employing machine learning technology. However, I have been quite skeptical about whether an algorithm model could work so well for this particular task -- valuing homes.
After all, having the right data is the most critical factor for any Automated Valuation Model (AVM) to be successful. Even though Redfin having full access to [MLS](https://en.wikipedia.org/wiki/Multiple_listing_service) data, it cannot possibly know every detail about a home.
Variables like the condition of a home, whether there were upgrades, the materials used in construction or remodeling, etc., can drastically influence the home's market value. Yet, I can hardly believe that any data source could keep accurate and up-to-date data on such matters. 

So the cynical part of me wonders if there could be an alternative explanation for Redfin Estimate's high accuracy. Possibly listing agents use Redfin Estimate to price their listings? Or in the other direction that Redfin Estimate follows the listing prices? These possibilities are only my suspicion until recently; an unusual listing finally revealed how Redfin Estimate and Zillow Zestimate made their numbers.

On September 18, 2019, one listing in my local area caught my attention with a sudden price cut of a whopping 39% from $1,640,000 to $1,000,000.
It was shortly confirmed to be not a price error by a friend of mine who is a real estate agent. The house was bought only a year ago for $1,525,000. And according to the listing agent, more than $150,000 were spent on remodeling. So likely, the seller was not willing to sell the house anywhere near $1 million. Instead, it was just a bold strategy aiming to draw more attention and eventually to land more offers.
What was more interesting than this significant price reduction itself was the reactions from Redfin and Zillow -- both dropped their estimation numbers dramatically in response to the price cut.
Seeing this unexpected ripple effect, I took the first screenshot of the Redfin page on September 22, which shows that Redfin Estimate valued the house at $1,098,037.

{% include image.html
   url=""
   file="/assets/images/20191110/Screenshot_20190922-195630_Redfin.jpg"
   max-width="50%"
   description="Redfin Estimate at $1,098,037 on 09/22/2019" %}

The remarkable price drop indeed drew many interests.
A Redfin agent wrote in her tour insights: "There is a pandemonium of showings happening at this house."  It didn't take long before the listing agent updated the note declaring they had multiple offers in hands already.
On September 25, the predetermined offer review date, the listing went into "Pending Sale" status.
Oddly, but not surprisingly, it came back to the market on the following day, with the price raised again to $1,680,000 right after the relisting.

{% include image.html
   url=""
   file="/assets/images/20191110/Screenshot_20190927-004648_Redfin_Price_History.jpg"
   max-width="50%"
   description="Redfin Property History showing the price changes" %}

It was less appealing for me to judge what had happened to the back and forth changes on the listing. But given the earlier observation of how Redfin Estimate responded to the change in listing price, I was prepared to see Redfin updating its estimate to match the listing price again. And Redfin did what I expected precisely -- in the subsequent update, Redfin Estimate jumped up to $1,608,742. 

{% include image.html
   url=""
   file="/assets/images/20191110/Redfin_Estimate_0927_vs_0928.jpg"
   max-width="100%"
   description="Redfin Estimate at $1,095,499 on 09/27/2019 (left) vs. $1,608,742 on 09/28/2019 (right)" %}

As you can see from the above screenshots, even though the fine print said: "Estimate based on these comparable homes." and the marks on the map referenced to likely the same set of comparable homes, the results from Redfin Estimate on the two consecutive days differed significantly.
Not only did Redfin updated its estimated value to be roughly the same as listing price again, but it also revised the entire estimate history.
Why did Redfin change the history of its estimates? One likely explanation could be Redfin intended to smooth the curve so that it would, superficially, look more stable and thus more credible to home shoppers. After all, you cannot expect people to trust an estimation model if there were wild fluctuations in the estimate history chart.

For comparison, I checked Zillow Zestimate for the same listing.
Under my earlier impression, Zillow, as a platform, usually tends to be more transparent than Redfin, which is essentially a brokerage. But this time, Zillow disappointed me as well. The Zestimate value dropped to south of $1 million when the seller made the big cut and surged back to more than $1.6 million following the price change after the relisting, just like what Redfin did.
Unlike Redfin Estimate, though, the Zillow Zestimate history chart was kept mostly unchanged. When the Zestimate value was below $1 million, the history chart clearly showed a sharp fall. By the time Zillow Zestimate restored, the previous negative spike had disappeared.
It was still unpleasant for me to see this backward modification, but I would tend to accept it as an act of removing a short term anomaly.
Also, as you may notice from the long screenshots below, Zillow outlined a set of data models behind Zestimate, including comparable-home model, tax model, and off-market model.
This breakdown seemingly provided more transparency of how they determined Zestimate value for the house.
Ironically, on September 27, despite comparable home model valued the home at $1,838,860, tax model suggested $1,720,655, and off-market model suggested $1,490,230; Zillow Zestimate made a final call for $981,132, which did not correlate with any of the three.

{% include image.html
   url=""
   file="/assets/images/20191110/Zillow_Zestimate_0927_vs_0928.jpg"
   max-width="100%"
   description="Zillow Zestimate at $981,132 on 09/27/2019 (left) vs. $1,651,200 on 09/28/2019 (right)" %}

This series of unusual listing activities provided me with a chance to unearth what Redfin Estimate and Zillow Zestimate virtually are. But I was not the first one who spotted the sneaky truth about Redfin Estimate. 
During writing, I came across [a post on Reddit](https://www.reddit.com/r/RealEstate/comments/7z3d99/us_does_redfins_estimate_just_agree_with_whatever/) from 2018, a listing agent in Santa Monica, California, accidentally typed two extra zeros and listed an otherwise $6,495,000 home for $649,500,000. Though the listing agent shortly corrected the price, Redfin Estimate, until it got another update, valued the house at $679,230,279.
In [another blog post](http://www.bubbleinfo.com/2018/04/13/redfin-estimates-based-on-list-price/) from 2018, a $549,000 house in Carlsbad, California, was mistakenly listed 1000x more expensive at $549,000,000. Again, Redfin Estimate came up its magic number as $573,099,848. 

So the takeaway so far is that Redfin Estimate and Zillow Zestimate are not what they claimed to be. Instead, they primarily echo the asking prices to ensure a narrow disparity between their estimates and the listing prices. What are the harmful effects of this?

First of all, Redfin Estimate and Zillow Zestimate can badly mislead homebuyers.
Being advertised as powered by machine learning algorithms, people generally perceive the two estimators as neutral tools that ought to provide an independent and transparent view of home values. Quite the opposite, however, by having the estimates primarily determined by the listing price, Redfin Estimate and Zillow Zestimate are literally on the seller's side. They provide no added value but endorse whatever prices sellers may ask for, no matter how ridiculous they might be.
Given the proven track records of Redfin Estimate and Zillow Zestimate being highly accurate, it is inevitable that many homebuyers would consider these computer-generated estimates as reasonable market prices.
More than once, I had heard my friends comparing Redfin Estimate with the prices they had paid for their homes. They were so fixated on the algorithm generated estimates without knowing that it was mostly a repeat of the listing price. So they often felt contented in case they paid less than Redfin's valuation. 
Unfortunately, in some cases, especially when they bought under no competition from other offers, I did sense that they might get ripped off partly because of Redfin Estimate.

Secondly, Redfin's act of retroactively revising its entire estimates history is genuinely dishonest and fraudulent.
I was really shocked to learn that the history of Redfin Estimate is even subject to change afterward. Having an AVM making inaccurate predictions is not uncommon and sometimes acceptable. But Redfin blatantly invalidates what they had estimated in the past and smooths the history curve.
Not only does this give people a false impression that Redfin Estimate has always been accurate, but it also creates a delusion in people's mind that the housing market is more stable and less volatile than it actually is. It is incredible to see Redfin, a public traded company, can even act in such an unethical way.

# An Alternative to Automated Valuation Model

In the end, putting all the rants aside, I wondered if there could be a fix to the problem or an alternative means to get the fair market values of homes.

As I mentioned above, having up-to-date and accurate data is the key to a successful AVM. So will there be a fix to Redfin and Zillow's machine learning estimation models? I came across [a blog post](https://www.zillow.com/blog/zestimate-updates-230614/) from Zillow published on June 26, 2019, in which Zillow announced that Zillow Zestimate received an update called "'Seeing' your home features."
The idea is that Zillow can determine the quality of a home from the homeowner provided photos. In the example given by Zillow, they can 'see' the remodeled bathroom, the new quartz countertops in your kitchen or the beautifully landscaped backyard from photos, and factor them directly into the home's Zestimate value. This concept sounds compelling to me; at least it is aiming to tackle the data collection problem directly. However, it is not hard to imagine challenges like some home sellers may game the system using deliberately edited photos.
In the same post, Zillow also admitted that the listing information of the home, including the listing price, is also factored into Zillow Zestimate. Zillow claimed that Zillow Zestimate's median error rate fell below 2% as a result of these updates. 
For Redfin Estimate, I couldn't find any official public announcement from Redfin that admits taking into account the listing price in Redfin Estimate.
But we have already seen that, in both AVMs, the listing price is the most dominant factor that far outweighs any other data points about a home. 

So in the new era of real estate, what could be a possibly better source for getting the fair market values of homes other than consulting with a real estate agent? It occurs to me that [crowdsourcing](https://en.wikipedia.org/wiki/Crowdsourcing) could be a favorable candidate for this task. 

In my mind, we need an independent platform where people can offer their thoughts on any given home's fair market value. 
Experienced real estate agents who can check out the property in person are undoubtedly excellent sources for the task. But we don't necessarily need to restrict the opinions from nonprofessionals. Average internet users who are familiar with the local housing market could be quality resources as well.
The platform should set up proper incentives, but not necessarily monetary incentives, to motivate people to provide inputs. For instance, professional real estate agents may benefit from more exposure to potential clients. And nonprofessional users may enjoy competing with others for more accurate estimates and climbing on a leaderboard. Needless to say, the estimates from those with a better track record will appear more credible.
Ideally, we want multiple estimates from different persons on each listing so that we can present the estimated price in an aggregated form, like median or mean, in addition to showing the original individual numbers and their sources.
I would be very interested in seeing how such a platform may play out in practice. Maybe someday I will build one.
