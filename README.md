# Solar System Explorers
This is an example of how to use the people API from [solarsystem.nasa.gov](https://solarsystem.nasa.gov/people)

You can view the example here…
https://jimthoburn.github.io/solar-system-explorers/

And the source code is here…
https://github.com/jimthoburn/solar-system-explorers/blob/master/index.html

The example is using client-side JavaScript to fetch the API data, and present it on a web page.

## Example requests

### All people
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4```

### Featured people
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4:134```

### Tributes
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4:147```

### People tagged with “Saturn”
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&tags=saturn```

### Limit to 20 people per page
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&per_page=20&page=0```

### Get the next page
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&per_page=20&page=1```

### Order the data by name, ascending
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&order=name+asc```

### Order the data by name, descending
```https://solarsystem.nasa.gov/api/v1/site_staffs/?category=4&order=name+desc```

## Example data
The data that comes back from the API is a JSON object, which looks like this…

```
{
  "items": [
    {
      "title": "Science Program Manager",
      "name": "Adriana Ocampo",
      "short_description": "<p>&quot;When thinking about the great adventure that you have ahead, dream and never give-up, be persistent and always be true to your heart.&quot;</p>\r\n",
      "body": "<h3><b>Where are you from?</b></h3>\r\n\r\n<p>I was born in Barranquilla, Colombia, and I was raised in Argentina. My family and I moved to the United States when I was a teenager. I now live in Washington, DC.</p>\r\n\r\n<h3><b>Describe the first time you made a personal connection with outer space.</b></h3>\r\n\r\n<p>When I was a little girl I would go on the roof of my house and look at the stars and wonder how far they were away from me. I would also make \"spacecraft\" with the pots and pans from my mother's kitchen. I would dress my doll up as an astronaut, and my dog Taurus was my co-pilot.</p>\r\n\r\n<h3><b>How did you end up working in the space program?</b></h3>\r\n\r\n<p>As soon as I landed in the USA I asked: \"Where is <a href='http://www.nasa.gov/centers/hq/home/index.html' target='_blank'>NASA</a>?\" After my junior year in high school, and thanks to the Space Exploration Post 509 -- sponsored by the <a href='http://www.jpl.nasa.gov/' target='_blank'>Jet Propulsion Laboratory</a> (JPL), I was able to first volunteer at JPL and then work there as an employee during the summer. As I started college I continued to work at JPL. I majored in geology at the California State University at Los Angeles, earning a B.S. there in 1983. I then got my Master of Science in planetary geology from California State University, Northridge. I received both my degrees while working full-time at JPL as a research scientist. I'm currently finishing my Ph.D. at the University of Amsterdam in the Netherlands.</p>\r\n\r\n<p><span><blockquote>\n<div class='gradient_line_extra_margin clearfix'></div>\n<div class='quote'>\n\"Space exploration was my passion from </span><span>a very young age, and I knew I wanted to </span><span>be part of it. I would dream and design </span><span>space colonies while sitting atop the roof </span><span>of my family's home in </span><span>Argentina.\"\n</div>\n<footer>\n<cite>- Adriana Ocampo</cite>\n</footer>\n<div class='gradient_line_extra_margin'></div>\n</blockquote></span></p>\r\n\r\n<h3><b>Who inspired you?</b></h3>\r\n\r\n<p>My parents were my inspiration. They always encouraged me to reach for the stars and instilled in me the knowledge that education was the gateway to making my dreams come true. Space exploration was my passion from a very young age, and I knew I wanted to be part of it. I would dream and design space colonies while sitting atop the roof of my family's home in Argentina.</p>\r\n\r\n<h3><b>What is a Science Program Manager?</b></h3>\r\n\r\n<p>Some of my duties include being the New Frontiers lead program executive. New Frontiers includes the Juno mission to Jupiter, the New Horizons mission to Pluto and the asteroid sample return mission OSIRIS-REx. I am also the lead Venus scientist responsible for NASA's collaboration with ESA's Venus Express mission, JAXA's Venus Climate Orbit and the Venus Exploration Analysis Group (VEXAG), which develops strategic plans and assessments for the exploration of this planet.</p>\r\n\r\n<h3><b>Tell us about a favorite moment so far in your career.</b></h3>\r\n\r\n<p>A favorite moment would have to be my research that led to the discovery of the Chicxulub impact crater. The impact that formed this crater caused the extinction of more than 50% of the Earth's species, including the dinosaurs. I wrote my master's and Ph.D. theses on this crater and I have led six research expeditions to study this amazing event that changed the evolution of life on our planet.</p>\r\n\r\n<h3><b>What advice would you give to someone who wants to take the same career path as you?</b></h3>\r\n\r\n<p>\"Dream and never give up.\" When thinking about the great adventure that you have ahead, dream and never give-up, be persistent and always be true to your heart. Live life with gusto. I would like to share my mnemonic (<b>STARS</b>) with you from the Girl Scouts book \"Recipes for Success:\"</p>\r\n\r\n<p><b>STARS</b></p>\r\n\r\n<p><b>S</b>mile: Life is a great adventure<br />\r\n<b>T</b>ranscend to triumph over the negative<br />\r\n<b>A</b>spire to be the best<br />\r\n<b>R</b>esolve to be true to your heart<br />\r\n<b>S</b>uccess comes to those who never give up on their dreams</p>\r\n\r\n<h3><b>What do you do for fun?</b></h3>\r\n\r\n<p>I love nature and anything that has to do with flying. Also, I love exploring and living life like it is a grand adventure.</p>\r\n",
      "image_subtitle": "\"Some of my duties include being the New Frontiers lead program executive, which includes ... the recently selected asteroid sample return mission: OSIRIS-REx.\"",
      "image_src": "/system/site_staffs/images/1780_Ocamp_319.jpg",
      "link": "/people/1780/adriana-ocampo"
    },
    {
      "title":
      …
    },
    {
      "title":
      …
    },
    …
  ],
  "more": true,
  "total": 20,
  "page": 0,
  "per_page": 20
}
```

If another page with more items is available, the `more` property will be set to `true`. Otherwise it will be `false`.
