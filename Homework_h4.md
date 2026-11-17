**H4 FEED ME:**

**x) Why would you want to use a feed reader (and RSS/Atom)? Couldn't you just browse to each website?**

Keeping track of information published across different websites can be challenging, particularly when following several blogs, news platforms, and technical publications. A feed reader makes this process easier by collecting new content from subscribed websites in one place through RSS (Really Simple Syndication) or Atom feeds.

**Benefits of Using a Feed Reader**

**Easy Access to Information:** Instead of visiting each website separately, users can view updates from all their selected sources through a single application. This makes information gathering quicker and more convenient.

**Better Control Over Content:** Users can follow the publications they are interested in and generally view articles according to their publication dates, rather than relying on social media algorithms to select and recommend content.

**Automatic Content Tracking:** Feed readers regularly check subscribed sources for newly published material. This means users do not have to remember to visit every website to check for updates.

**Greater Privacy:** Following website updates through feeds usually does not require sharing an email address, subscribing to newsletters, or registering accounts on multiple platforms.

**Improved Reading Experience:** Many feed reader applications offer a simplified view of articles, reducing distractions caused by advertisements, pop-ups, and other unnecessary website elements.

**Challenges of Visiting Websites Manually**

Checking websites individually requires regular effort and depends on users remembering which sources they want to monitor. It can also be difficult to identify whether a website has published anything new since the previous visit. This becomes increasingly impractical when following dozens of sources, such as cybersecurity blogs, technical forums, security research publications, and industry news websites.

**Conclusion**

A feed reader offers a practical alternative to manual browsing by making information collection more organised and less time-consuming. For cybersecurity professionals, it can be particularly valuable for following security researchers, monitoring emerging cyber threats, reading vulnerability disclosures, and keeping up with changes in the cybersecurity industry. Therefore, RSS and Atom feeds support continuous learning and help security professionals maintain awareness of the latest developments.

**y) Supreme court of Finland, [case Osuuspankkikeskus port scan KKO:2003:36](https://www.finlex.fi/fi/oikeuskaytanto/korkein-oikeus/ennakkopaatokset/2003/36).**

Background: The case involved a 17-year-old who used port-scanning software to examine the computer network of Osuuspankkikeskus (OPK). The purpose was to identify open ports and possible ways to access the network. However, the organisation's firewall blocked the attempted access.

Court decision: The Supreme Court considered the activity an attempted computer intrusion, even though the individual did not successfully enter the system. The case highlighted that attempting to gain unauthorised access can have legal consequences even when the security measures prevent the intrusion from succeeding.

Outcome: The individual received a fine and was ordered to pay compensation to the affected parties.

Conclusion: This case illustrates the legal risks associated with unauthorised network scanning when it is connected to an attempt to access protected systems. Port scanning is a useful technique in cybersecurity, but it should only be performed with appropriate permission. Security professionals must ensure that their testing activities remain within the agreed scope and do not violate applicable laws.

**a ) Install a feed reader. Show that it can read a feed (RSS or Atom). Include a screenshot of this.**

For this part, I installed **RSSGuard** on my machine. After installing, it looks like this before I added feed.

![Screenshot 1](images/screenshot-01.png)

**b ) Add the feed for Krebs.**

- Add account to set up feed.

![Screenshot 2](images/screenshot-02.png)

- Select local RSS option and click OK

![Screenshot 3](images/screenshot-03.png)

- Give appropriate title and click OK

![Screenshot 4](images/screenshot-04.png)

- Following screen will appear after your account is set up.

![Screenshot 5](images/screenshot-05.png)

- Now for adding feed, click on Feeds on menu bar and select the option as shown below

![Screenshot 6](images/screenshot-06.png)

- Paste the url and click on Discover button

![Screenshot 7](images/screenshot-07.png)

- The feeds will appear in the discovered feeds section. Click on Select all and click Import checked feeds. Close the window in the end.

![Screenshot 8](images/screenshot-08.png)

- The feeds will appear in the right panel as shown below.

![Screenshot 9](images/screenshot-09.png)

**c ) Add a feed for Schneier on Security. Find the blog, and locate the feed.**

I located Bruce Schneier's official cybersecurity blog, Schneier on Security, and identified its Atom feed.I added the feed to RSS Guard using the Discover Feeds option and successfully imported it into my existing feed reader. After updating the subscription, the application retrieved several articles published by Bruce Schneier, which were displayed in the article list.

Feed URL: [https://www.schneier.com/feed/atom/](https://www.schneier.com/feed/atom/)

**d ) Find and add two more security related feeds. Explain how you found them, and why you chose them.**

For this task, I searched for a while and found two blogs which caught my interest, The Hacker News and Dark Reading. Both provide regular updates about cybersecurity threats, vulnerabilities, hacking incidents, and developments in information security. I chose them because they are most discussed and most followed blogs among cybersecurity professionals and also offer insights on variety of topics from analytics and application security to mobile and cloud security, IoT and more.

**The Hacker News**

Website: [https://thehackernews.com/](https://thehackernews.com/)

Feed: [https://feeds.feedburner.com/TheHackersNews](https://feeds.feedburner.com/TheHackersNews)

**Dark Reading**

Website: [https://www.darkreading.com/](https://www.darkreading.com/)

Feed: [https://www.darkreading.com/rss.xml](https://www.darkreading.com/rss.xml)

**e ) Follow security feeds for a while. What did you learn? What are the benefits and downsides of following feeds with a reader, compared to some other methods of following cyber security scene?**

After using RSS Guard to follow cybersecurity publications such as Krebs on Security, Schneier on Security, The Hacker News, and Dark Reading, I gained a better understanding of current security issues and how cyber threats affect individuals and organisations.

What I Learned

Following these sources helped me understand that cyber threats are constantly changing. I learned about different types of attacks, security vulnerabilities, malware, and ransomware. I also realised that technical protection alone is not enough; organisations must pay attention to employee awareness, security policies, and regular software updates.

Benefits of Using a Feed Reader

- Brings information from several cybersecurity websites together in one place.

- Reduces the time spent checking individual websites for new articles.

- Makes it easier to follow different cybersecurity topics and developments.

- Provides a more organised reading experience with fewer distractions.

- Helps users regularly update their cybersecurity knowledge.

Limitations of Using a Feed Reader

- Subscribing to many sources can make it difficult to keep up with all the updates.

- Some feeds display only article headlines or brief descriptions.

- Not every website provides an RSS or Atom feed.

- There are fewer opportunities for discussion compared with social media and online communities.

- Users must check the accuracy and relevance of the information themselves.

Comparison with Other Information Sources

RSS readers are convenient for collecting updates from multiple websites, whereas social media platforms provide discussions and opinions from other users. Email newsletters offer selected information directly to an inbox, while visiting websites manually gives access to complete articles and additional resources. Each method can be useful depending on the user's needs.

Conclusion

Using RSS Guard was a practical way to explore different cybersecurity information sources and follow developments in the security field. I found that feed readers make information gathering easier and more organised, although they have some limitations. Combining RSS feeds with other sources, such as professional communities, newsletters, and social media, can provide a broader understanding of cybersecurity and emerging threats.

**f ) Port scan. How can criminals know what services your employer has?**
