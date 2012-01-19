#Responsive Video

jQuery Plugin for a video player that scales to fit its container

##How to Use

Add video element to your html inside a container div that is styled to scale with the size of the browser window

	<div id="container">
        <video id="myVideo" width="640" height="360" poster="img/poster.jpg" controls autoplay>
            <source src="vid/video.mp4" type="video/mp4"  />
        </video>
    </div>
    
First, link to jQuery and then to vidobject.js. Next, create a new vidobject and apply any custom settings to it. Last, use vidobject to target the video element(s) on the page.

	<script src="http://code.jquery.com/jquery-1.7.min.js"></script>
    <script src="js/vidobject.js"></script>
    <script>
        var vidobject = new $.vidobject({
            player: 'swf/vidobject.swf',
            buttonColor: '#FFFFFF',
            accentColor: '#BBBBBB',
            backgroundColor: '#111111',
            scaleVideo: true,
            fullScreen: true
        });
        vidobject.embed("myVideo");
    </script>
    

Parameters are:
    
**player:** path to the vidobject.swf player
**buttonColor:** video controls button color (default is '#FFFFFF')
**accentColor:** video controls accent color (default is '#BBBBBB')
**backgroundColor:** video controls background color (default is '#111111')
**scaleVideo:** set to false if you don't want the video to scale  
**fullScreen:** set to false to disable full screen mode  


Responsive Video Object created by John Polacek  
Twitter: http://twitter.com/#!/johnpolacek  
Blog: http://johnpolacek.com
