---
layout: inner
date: '2017-02-20 22:03 +0100'
ads: false
comments: true
published: true
title: A note on pool swim activity data in Garmin Connect
categories: apps
tags: apps connectiq garmin
lead_text: title
---
This last week I have received 11 (!) times the same question: why is distance shown as 0 in Garmin Connect after syncing the activity?

Well the answer has been since quite a while in the [user guide](https://danipindado.github.io/downloads/pool_swim_user_guide.pdf){:target="_blank"}, and now I am reproducing the same info here so that it can more easily be found (and it is easier for me to forward all these people to the answer :) )

There are two ways of getting distance data into GC,


- you can just edit data in any web browser, 
- you can use the gpx trick, by using a [www.sportracks.mobi]([www.sportracks.mobi){:target="_blank"} account as interface. 

here below both methods are described. 


## Understanding data in Garmin Connect
ConnectIQ apps are not allow to override native fields in Garmin Connect. Therefore, the native distance fields will show distance = 0m.  Same applies for speed. Please note, that this is a Garmin decision. **There is nothing that developers can do right now to override native fields from within an app.**

<img src="{{site.baseurl}}/images/distance_1.png" width="100%">


Still measured distance, speed and interval information are shown in Garmin Connect. You can find these data in the statistics and intervals region. You will find a ConnectIQ section where you can find the data recorded by the app.
 
<img src="{{site.baseurl}}/images/distance_2.png" width="100%">
<img src="{{site.baseurl}}/images/distance_3.png" width="100%">
 
 And also in the app:
 
<img src="{{site.baseurl}}/images/distance_app.png" width="50%">



## Manually modifying data in Garmin Connect
edit the activity following the steps below:

<img src="{{site.baseurl}}/images/distance_4.png" width="100%">
<img src="{{site.baseurl}}/images/distance_5.png" width="100%">
 

Once you have set the proper distance, you'll see that native pace field will be also updated.

<img src="{{site.baseurl}}/images/distance_6.png" width="100%">


## Replacing native fields in Garmin connect (gpx method)
You need to have a sporttracks account for this, which is already synced with your Garmin account.
In [www.sportracks.mobi]([www.sportracks.mobi){:target="_blank"}, browse the activity. 
Select "export" and "gpx". 
A gpx file containing the activity will be downloaded.

<img src="{{site.baseurl}}/images/gpx_1.png" width="100%">
 

Upload the gpx file generated in previous step into Garmin Connect. 
In order to do this, go to "my activities", "manual upload". Select the file and upload it.

<img src="{{site.baseurl}}/images/gpx_2.png" width="100%">


The activity will be uploaded to Garmin Connect. 
This time, native fields show the correct information, because sportracks overrode the native fields with the ConnectIQ fields in the gpx file. The ConnectIQ fields are not available anymore.

<img src="{{site.baseurl}}/images/gpx_3.png" width="100%">

Feel free to use the comment section below to ask any questions. 
Remember that you don't need to create a Disqus account in order to comment: just write your comment, click on the "Name" field below, and the option "I'd rather post as a guest" will pop up.

Happy swimming!
Cheerio
