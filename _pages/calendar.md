---
title: "Eseménynaptár"
permalink: /calendar
excerpt: "Találkozzunk!"
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/horse.png
---
Hamarosan!
<link href='assets/lib/fullcalendar.min.css' rel='stylesheet' />
<link href='assets/lib/fullcalendar.print.min.css' rel='stylesheet' media='print' />
<script src='assets/lib/jquery-3.3.1.min.js'></script>
<script src='assets/lib/moment.min.js'></script>
<script src='assets/lib/fullcalendar.min.js'></script>
<script src='assets/lib/gcal.min.js'></script>
<script>

  $(document).ready(function() {

    $('#calendar').fullCalendar({

      header: {
        left: 'prev,next today',
        center: 'title',
        right: 'month,listYear'
      },

      displayEventTime: false, // don't show the time column in list view

      // To make your own Google API key, follow the directions here:
      // http://fullcalendar.io/docs/google_calendar/
      googleCalendarApiKey: 'nG0t2D0x79B-DoBs1sTbw6PX',

      events: 'du05dgqv9ibe041aokilbh3pnk@group.calendar.google.com',

      /*eventClick: function(event) {
        // opens events in a popup window
        window.open(event.url, 'gcalevent', 'width=700,height=600');
        return false;
      },*/



    });

  });

</script>
<style>

  body {
    margin: 40px 10px;
    padding: 0;
    font-family: "Lucida Grande",Helvetica,Arial,Verdana,sans-serif;
    font-size: 14px;
  }

  #loading {
    display: none;
    position: absolute;
    top: 10px;
    right: 10px;
  }

  #calendar {
    max-width: 900px;
    margin: 0 auto;
  }

</style>

  <div id='calendar'></div>
