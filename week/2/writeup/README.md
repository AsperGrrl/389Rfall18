Writeup 2 - OSINT (Open Source Intelligence)
======

Name: Annette Keller
Section: 0201

I pledge on my honor that I have not given or received any unauthorized assistance on this assignment or examination.

Digital acknowledgement of honor pledge: Annette Keller

## Assignment 2 writeup

### Part 1 (45 pts)

1. What is kruegster1990's real name? 

Fred Krueger
From google search turning up umdcsec followers on stwty.com:
![Google search results turn up umdcsec Twitter followers](https://imgur.com/dNwozrd)

2. List all personal information (including social media accounts) you can find about him. For each, briefly detail how you discovered them.

   Google results:

   zara larsson web page, found with Google:
      https://zaralarsson115206071.wordpress.com/2018/08/12/kruegster1990/
      https://zaralarsson115206071.wordpress.com/2018/08/12/kruegster1990/
      https://zaralarsson115206071.wordpress.co

   Twitter web client referenced under his name with the UMD cybersecurity club 
      https://stwity.com/umdcsec/

   websites listed under his name with the UMD cybersecurity club 
      https://www2.idexpertscorp.com/knowledge-cent ..
      completing link: https://www2.idexpertscorp.com/knowledge-center/tag/kruegster1990
      "No entries were found" for kruegster1990
	
   Reddit:
      reddit/u/kruegster1990 (account exists with no posts)
      twicsy.com: tweeter kruegster1990 RT listed in widget of tweets on page
      https://r2.twicsy.com/i/Ad8Q2n
		
		
      text kruegster1990 links to: https://r2.twicsy.com/u/kruegster1990
      Other social media accounts found on checkusernames.com:
   
         Linked In Not Available
         Twitter Not Available
         Reddit Not Available
         Yelp Not Available
         Fiverr Not Available
         Wiki How Not Available
         Houzz Not Available
         Viadeo Not Available
         Hi5 Not Available
         Dribbble Not Available
         Instructables Not Available
         Funny Or Die Not Available
         Net Vibes Not Available
         APSense Not Available
         Dzone Links Not Available
         Zedge Not Available
         Active Not Available
         Toluna Not Available
         Biz Sugar Not Available
         Stock Twits Not Available
         Trend Hunter Not Available
         Active Rain Not Available
         Wall Inside Not Available
         Kiva Not Available
         Map My Run Not Available
         Visualize Us Not Available
         Fmylife Not Available
         PaperBack Swap Not Available
         Start Aid Not Available

   Google search turns up his profile on another twitter account tracker on 
      https://stwity.com/kruegster1990/

      The Twitter userid listed at the bottom is 1028770124772397061 & corresponds to user @kruegster1990 (twitter username is also listed with his profile entry with the UMD cybersecurity club)
	
      Twitter profile references his website, http://www.cornerstoneairlines.co
	
	
      Other info in media posted on cornerstoneairlines.co

      main page source:
         href for "Admin" link: http://142.93.117.193
	 <a class="nav-link" href="http://142.93.117.193">Admin</a>
	    --> doesn't resolve to a domain name on lookup
         email shown as kruegster@tutanota.com does link to that email
         Style sheet is /cover.css
            background image is '/wallpaper.jpg"
			
         Image Metadata: 
	    No interesting metadata in images linked to website
               photo of Fred Krueger: 
               https://i2.wp.com/pbs.twimg.com/profile_images/1028771026815995904/BVJ1ed66_200x200.jpg
               wallpaper.jpg is a stock image by Philippe Clairo in 2011

      No /src, /cgi-bin, /img, or /css subdirectories off web root
      404 Not Found status info
         reported by web server nginx/1/10.3 on Ubuntu
			
			
		
      Internet archive for cornerstoneairlines.co shows only robots.txt: 
	 cornerstoneairlines.co/robots.txt saved on 09/08/2018
            User-agent: *
            Disallow: /secret
         checked out cornerstoneairlines.co/secret
         found flag in a comment in index.html: 
            CMSC389R-{fly_th3_sk1es_w1th_u5}
			
			
      142.93.117.193 (link from "Admin" text on main page) 
         No /src, /cgi-bin, /img, or /css subdirectories off web root
         Does it have a /secret directory?
		
         142.93.117.193 --> has an Ubuntu Apache 12.4.18 web server on port 80
            Internet archive for http://142.93.117.193
            shows an assortment of websites, see 
            https://web.archive.org/web/*/http://142.93.117.193

      take break from OSINT for now

3. What is the IP address of the webserver hosting his company's site? How did you discover this? 

   142.93.118.186
   found searching https://centralops.net/co/DomainDossier.aspx for
      cornerstoneairlines.co

4. List any hidden files or directories you found on this website. Did you find any flags?

   found image wallpaper.jpg, style sheet cover.css, robots.txt and /secret
   in cornerstoneairlines.co/secret found flag in a comment in index.html

5. Did you find any other IP addresses associated with this website? What do they link to, or where did you find them?



6. If you found any associated server(s), where are they located? How did you discover this?


7. Which operating system is running on the associated server(s)? How did you discover this?


8. *(BONUS)* Did you find any other flags on your OSINT mission?

   --> come back to this later, if time, running the right tools in Kali


### Part 2 (55 pts)

*REPLACE THIS TEXT WITH A BRIEF EXPLANATION OF YOUR APPROACH TO SOLVING THIS CHALLENGE, AND THE OUTCOME*
