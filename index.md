---
layout: lesson
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
venue: "LHC Physics Center, Fermi National Accelerator Laboratory"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: "In Person"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "us"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the
latitude: "41.842258"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-88.245781"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "Synchronously January, 2023"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "24/7"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2025-01-13 # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2025-01-17   # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
email: ["emery.nibigira@cern.ch"]
---

<img class="plain"  src="fig/event.png" height=400>

## Welcome to the CMS Data Analysis School 2025 Generators Short Exercise!

This exercise introduces Monte Carlo event generators and how they are used in high energy physics,
focusing on the workflows used in CMS.

<!-- The information and exercises are based on the [2022 CMSDAS](https://twiki.cern.ch/twiki/bin/view/CMS/SWGuideCMSDataAnalysisSchoolLPC2022GeneratorsExercise#Task_1_Using_standalone_MG5) as well as the
[Generator HATS 2021](https://twiki.cern.ch/twiki/bin/viewauth/CMS/GeneratorsHATSatLPC2021).
It has been extended to cover new tools like [NanoGEN](https://twiki.cern.ch/twiki/bin/viewauth/CMS/NanoGen) and introduce generator-related systematic uncertainties. -->

<!-- this is an html comment -->

{% comment %} This is a comment in Liquid {% endcomment %}

> ## Prerequisites
> **Before going any further, please complete the [CMS DAS Pre-Exercises](https://fnallpc.github.io/cms-das-pre-exercises/) and then follow the instructions on the [setup page](setup.md).**
{: .prereq}

> ## Facilitators
> #### Lead Contact
> * [Emery Nibigira](#facilitators), University of Tennessee ([emery.nibigira@cern.ch](mailto:emery.nibigira@cern.ch))
> * [Steve Mrenna](#facilitators), FERMILAB ([stephen.mrenna@cern.ch](mailto:stephen.mrenna@cern.ch))
>  
> #### All Facilitators
> <table>
>   <tr>
>     <td align="center"><a href="https://github.com/enibigir"><img src="https://lpc.fnal.gov//CMSDAS2025/Emery_Nibigira.png" width="100px;" alt=""/><br /><sub><b>Emery Nibigira</b></sub></a><br /><a href="https://lpc.fnal.gov/fellows/2025/Emery_Nibigira.shtml" title="More about him">🖋</a></td>
>     <td align="center"><a href="https://github.com/smrenna"><img src="https://lpc.fnal.gov//CMSDAS2024/Steve_Mrenna.png" width="100px;" alt=""/><br /><sub><b>Steve Mrenna</b></sub></a><br /><a href="https://cms.fnal.gov/stephen-mrenna/" title="More about him">🖋</a></td>
<!-- >     <td align="center"><a href="https://github.com/akgrummer"><img src="https://lpc.fnal.gov//CMSDAS2024/Aidan_Grummer.jpg" width="100px;" alt=""/><br /><sub><b>Aidan Grummer</b></sub></a><br /><a href="https://github.com/akgrummer" title="More about him">🖋</a></td>
>     <td align="center"><a href="https://github.com/"><img src="https://lpc.fnal.gov//CMSDAS2024/Keith_Ulmer.jpg" width="100px;" alt=""/><br /><sub><b>Keith Ulmer</b></sub></a><br /><a href="https://github.com/" title="More about him">🖋</a></td>
>     <td align="center"><a href="https://github.com/"><img src="https://lpc.fnal.gov//CMSDAS2024/Kai_Yi.jpg" width="100px;" alt=""/><br /><sub><b>Kai Yi</b></sub></a><br /><a href="https://github.com/" title="More about him">🖋</a></td>
>   </tr>
>   <tr>
>     <td align="center"><a href="https://github.com/"><img src="https://lpc.fnal.gov//CMSDAS2024/Irene_Zoi.jpg" width="100px;" alt=""/><br /><sub><b>Irene Zoi</b></sub></a><br /><a href="https://github.com/" title="More about him">🖋</a></td>
>     <td align="center"><a href="https://github.com/"><img src="https://lpc.fnal.gov//CMSDAS2024/Sam_Bein.jpg" width="100px;" alt=""/><br /><sub><b>Sam Bein</b></sub></a><br /><a href="https://github.com/" title="More about him">🖋</a></td>
>     <td align="center"><a href="https://github.com/"><img src="https://lpc.fnal.gov//CMSDAS2024/Brunella_D_Anzi.jpg" width="100px;" alt=""/><br /><sub><b>Brunella D'Anzi</b></sub></a><br /><a href="https://github.com/" title="More about him">🖋</a></td>
>     <td align="center"><a href="https://github.com/"><img src="https://lpc.fnal.gov//CMSDAS2024/Nicola_De_Filippis.png" width="100px;" alt=""/><br /><sub><b>Nicola De Filippis</b></sub></a><br /><a href="https://github.com/" title="More about him">🖋</a></td>
>     <td align="center"><a href="https://github.com/"><img src="https://lpc.fnal.gov//CMSDAS2024/Ulascan_Sarica.jpg" width="100px;" alt=""/><br /><sub><b>Ulascan Sarica</b></sub></a><br /><a href="https://github.com/" title="More about him">🖋</a></td> -->
>   </tr>
> </table>
{: .testimonial}

> ## Mattermost Chat
> **The [Generators Short Exercise](https://mattermost.web.cern.ch/cmsdaslpc2025/channels/ShortExGenerators) channel will be available once you join the [CMSDAS@LPC2025](https://mattermost.web.cern.ch/cmsdaslpc2025/channels/town-square) team. Direction for how to join this Mattermost chat team can be found on the <a href="setup.html">setup</a> page.**
{: .discussion}

{% include links.md %}
