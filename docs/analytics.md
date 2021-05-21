# How to enable Google Analytics on all pages
Google Analytics has been set on ATOM website to check statistics like:

**Number of users accessing the website**

<img src="http://127.0.0.1:8000/Google_NumUsers.png" alt="Flowchart of how to input data to output web portal pages">

**Location of visitors**

<img src="http://127.0.0.1:8000/Google_LocUsers.png" alt="Location of visitors">

**Which pages visitors click on the most**

<img src="http://127.0.0.1:8000/Google_VisPages.png" alt="Which pages visitors click on the most">

**Number of downloads from the website**

<img src="http://127.0.0.1:8000/Google_Downloads.png" alt="Number of downloads from the website">

**Number of accesses through computer and mobile devices**

<img src="http://127.0.0.1:8000/Google_Devices.png" alt="Number of accesses through computer and mobile devices">

To enable it on webpages, add these lines right after the `<head>` tag of each page, before enlisting the scripts and CSS content to the page.
```
  <!-- Global site tag (gtag.js) - Google Analytics -->
  <script async src="https://www.googletagmanager.com/gtag/js?id=UA-174267174-1"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag() { dataLayer.push(arguments); }
    gtag('js', new Date());

    gtag('config', 'UA-174267174-1');
  </script>

  <!-- Google Tag Manager -->
  <script>(function (w, d, s, l, i) {
      w[l] = w[l] || []; w[l].push({
        'gtm.start':
          new Date().getTime(), event: 'gtm.js'
      }); var f = d.getElementsByTagName(s)[0],
        j = d.createElement(s), dl = l != 'dataLayer' ? '&l=' + l : ''; j.async = true; j.src =
          'https://www.googletagmanager.com/gtm.js?id=' + i + dl; f.parentNode.insertBefore(j, f);
    })(window, document, 'script', 'dataLayer', 'GTM-WPM5389');</script>
  <!-- End Google Tag Manager -->
```


Here is the link to <a href="https://analytics.google.com/analytics/web/?authuser=1#/report-home/a174267174w241788037p225418234" target="_blank">Google Analytics</a>.
Dr. Safronova and Dr. Eigenmann have all the required permissions to manage everything.
