---

layout: col-sidebar
title: OWASP Vienna
tags: 
level: 4

region: Europe
meetup-group: OWASP-Vienna-Chapter
country: Austria
postal-code: 

---

## Welcome to the homepage for the OWASP Chapter in Vienna.
This is the page for the OWASP Chapter in Vienna Austria. Welcome!

## Local News
Please join our [mailing list](https://groups.google.com/a/owasp.org/forum/#!forum/vienna-chapter) or [Meetup](https://www.meetup.com/OWASP-Vienna-Chapter/) for the schedule of events.

## Please check our upcoming [Meetup](https://www.meetup.com/OWASP-Vienna-Chapter/) events:
 {% include chapter_events.html group=page.meetup-group %}

### Upcoming events
{% include chapter_events.html group=page.meetup-group %}

<script type='text/javascript'>
  $(function(){
    $(".timeclass").hover(function() {
      utc_str = $(this).text();
      ndx = utc_str.indexOf(':');
      st_hour_str = utc_str.substring(0, ndx);
      st_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(st_hour_str), parseInt(st_min_str), 0);
      start_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);

      ndx = utc_str.lastIndexOf(':');
      end_hour_str = utc_str.substring(ndx - 2, ndx - 1);
      end_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(end_hour_str), parseInt(end_min_str), 0);
      end_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);
      popstr = start_dt.toLocaleString(luxon.DateTime.TIME_WITH_SECONDS) + ' to ' + end_dt.toLocaleString(luxon.DateTime.TIME_WITH_SHORT_OFFSET);
      $(this).prop('title', popstr);
    });
  });

  
</script>
