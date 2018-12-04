# JoveDownloader
A javascirpt bookmark which can help you download the video from jove.com

Save the following script as a bookmark in your favorite browser. When you 
watch the video on jove.com, click it, a new tab which contains the video 
will pop up, then you can download it by 'save as' etc.


    javascript:JoveScript=document.body.getElementsByTagName(“script”);for(i=0;i<JoveScript.length;i++){if(VideoUrl=JoveScript[i].textContent.match(/\d{4,}_[\w-]+_\d+_\w[\d]*_Web\.mp4/)){window.open(‘https://www.jove.com/CDNSource/protected/'+VideoUrl.toString(),'_blank'); break;}}


Can only be tested in China, Sry.

Known bugs:
You can't download old videos on some pages because the URL patterns are different.
Will fix it later.
