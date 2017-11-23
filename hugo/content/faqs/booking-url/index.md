# Booking URL for a specific venue

If you are unable to add the Collins booking widget, it's possible for you to include a booking URL to your website instead. 

To create a booking URL for your venue, you will need to use a URL of the following form:

https://www.designmynight.com/book?venue_id=VENUEID&source=partner&format=modal

Where you have to replace 'VENUEID' with your unique Collins Venue ID. **To find your Collins Venue ID:**

Settings > Venues > Select your venue > in the URL, your venue ID will be included at the end in the URL:

eg: https://admin.designmynight.com/collins/venue-rules/5787a87595838bed3a8b4569

In this example, the booking URL for this venue would be: 

https://www.designmynight.com/book?venue_id=5787a87595838bed3a8b4569&source=partner&format=modal

# Booking URL for a specific booking type

If you are looking to create a booking link for a specific booking type (for example if you want to send a link out in a targetted mail out), you can create a URL of the following format: 

https://www.designmynight.com/book?venue_id=VENUEID&venue_group=VENUEGROUPID&type=BOOKINGTYPEID&source=partner&fixed_type=1

Where you have to replace 'VENUEID', VENUEGROUPID and BOOKINGTYPEID accordingly. **To find your Collins Venue Group ID:**

Settings > Venue Group > in the URL, your venue ID will be included at the end in the URL:

eg: https://admin.designmynight.com/collins/venue-groups/5524371d0df690ad7156f2ea

**To find your unique Booking Type ID:**


If you want to fix any other parameters (for example if this booking type runs only on a single time and date), you can include the following paraments in your URL:

&date=DATE **note: to be given in the form YYYY-MM-DD eg 2016-03-12**
&time=STARTTIME **note: to be given in the 24-hour form HH:MM eg 15:00**
&duration=DURATION **note: to be given in terms of hours eg 2.5 (which would be 2 hours 30 mins) **

So you will have something that looks like:

https://www.designmynight.com/book?venue_id=VENUEID&venue_group=VENUEGROUP&type=BOOKINGTYPEID&type_name=BOOKINGTYPEID&date=DATE&time=STARTTIME&duration=DURATION&source=partner

# Customising the 2nd iFrame of the Collins booking URL
You are able to customise the 2nd iframe on your Collins booking URL to better suit the feel of your website. 

## To do this, you would need to:

1. Tell us a URL of a stylesheet (that has to be on an HTTPS connection for us to load it) and what you want to use it for (eg app/website).

2. We add this CSS URL to our system for your venue group, with a name eg app

3. Then you should add `stylesheet=app` to the end of the URL you are going to send the user to.

4. When the URL loads, it will also load your CSS so you can override whatever is on the book page.