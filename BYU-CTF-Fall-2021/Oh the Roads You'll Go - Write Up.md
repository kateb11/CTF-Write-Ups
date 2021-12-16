## Oh the Roads You'll Go - Hard  

> Can you imagine Provo drivers in this intersection? I can't! Thank goodness it is x amount of miles from the Crabtree...  

![Intersection](crazy_roads.png)

> Flag is ctf{x} where x is the number of miles as the crow flies from the Crabtree Building to this intersection +/- 2 miles.

This OSINT challenge was actually pretty fun. We are given this screenshot from Google Maps and are tasked with finding its location. Looking at the image, we see that there are a few helpful hints, while the rest is pretty blurry or unhelpful. 
Something to note is that the SB (South Bound) letters on the are incorrect. If you look at the compass in the bottom right corner, you see that we aren't facing South. This could be important to identify and locate the road in Google Maps. 

After looking at everything in the image, we can use that information to locate this intersection. 

1. Phone Number on the Car
 - Looking up the area code we can narrow down the region where this intersection is 
 - Looking up the phone number we can find the business that it belongs to and where they are located. The business was located in Framington, which I though was going to be helpful but it wasn't. The area code was all we were supposed to need. 
2. Route Numbers
 - This intersection is on Route 16
 - There is a partly covered sign that starts with the number 2
 - Find where Route 16 intersects ith routes that start 2
3. Locate intersections on Route 16 that begin with 2 
 - Look at the Wikipedia article for Massachusetts Route 16
 - In this article we can see the different major intersections along Route 16
 - ONe of the major routes is 28 in Reading. Looking back at the picture we ca see that on the sign there appears to be the letters "Rea". It seems we are on the right track!
 ![Intersection](Route28.png)
 4. FInd the Intersection
 - Open Google Maps and locate where Route 16 intersects with Route 28 in Reading, Massachusetts
 - We found it!
 5. Calculate miles
 - Copy coordinates of intersection  
 - Google the BYU Crabtree coordinates
 - Enter both coordinates into an online tool that will calculate the distance as the crow flies
 ![Intersection](Distance.png)
 - Bam! There's your answer
 > ctf{2089}