# Intelligent Transportation Systems Chart Redesign
<br>

## Why Intelligent Transportation Systems (ITS) Chart & Links to the Original Data: 
<b>You can access the original report from which I pulled the ITS work safety zone for freeway chart [here](https://rosap.ntl.bts.gov/view/dot/60122).</b> The chart of interest is on page 21 (PDF page 31) of the report. You can reference the source data via the links at the bottom of this page.

<b>I chose this visualization because it comes from a report I reviewed closely over the course my summer internship with the Government Accountability Office.</b> I worked on a project analyzing the impact of Intelligent Transportation Systems (ITS) technologies on improving traffic flow. ITS includes technologies such as ramp meters, connected vehicles, and CCTV, and its proponents note its ability to improve safety and mobility outcomes for road users. (Source: [ITS DOT](https://www.its.dot.gov/factsheets/benefits_factsheet.htm#:~:text=Some%20of%20the%20most%20prominent,priority%2C%20and%20traveler%20information%20systems)). As part of this work, I analyzed reports, data, and more that the Department of Transportation (DOT) had collected on ITS technologies as well as levels of technology deployment by various local, regional, and state transportation agencies — including its "Intelligent Transportation Systems Deployment Tracking Survey: 2020 Freeway Findings" report, the source of the chart I used for this exercise.

At first glance, ITS may seem somewhat abstract — and perhaps even boring: who really cares ramp meters on freeways? <b>But when you think about the ways that the built environment — and sitting in traffic — shape our daily lives, you begin to realize that those meters that let you merge more easily onto the interstate to get home after a long day at work really do matter.</b> While the original report and chart are intended for a technical audience, I  wanted to figure out a way to engage on-technical audiences in the subject, in addition to redesigning the chart for the report. I chose a graphic focused on the types of technologies transportation agencies deploy in work zones because I wanted to highlight how ITS can improve safety for various types of road users: in this case, road workers and drivers alike.

## Reenvisioning the Chart: 

When critiquing the visualization, I noted a number of the chart’s features that I thought could benefit from modification. Thinking through Stephen Few’s “Data Visualization Effectiveness Profile” method, <b>I found the chart’s perceptibility and intuitiveness limited.</b> This primarily owed to the fact that the original chart presents the data in a stacked bar chart, color-coding by year instead of having year on the x-axis, and placing the different ITS technology types on the y-axis. In essence, this flipped the way that I expected to see the data: I typically associate time-series data as a line chart, with years marking the x-axis. In turn, this layout made it difficult for me to compare across technologies and years, which forced me to take time inspecting the graph to glean its insights – something that a reader encountering this graph among a sea of others in the report might not do of their own volition. 

<b>While the graph was generally useful and complete for its target audience (technical readers), I did wonder if more clarification around novel or emerging technologies might be helpful, even for the informed reader.</b> At the same time, I didn’t want to bog the chart down with details or text popups that would be redundant. This was a tradeoff I considered while working through the sketches and Tableau redesigns for the technical audience. In the sketch, I considered putting a sentence of information describing each technology in the label popup when viewers hovered over each. However, in the final version in Tableau, I ultimately decided against this approach because I didn’t think it was an effective way to communicate this information: would chart viewers realistically take the time to hover over all of the lines (or even those of interest) for a sentence of information? Probably not.
<br>
<div class="flourish-embed flourish-chart" data-src="visualisation/11239803"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
<br>
This was a different story in thinking through a redesign for a non-technical audience that would be unfamiliar with any of the technologies. In this case, I realized that a useful and complete graph might have less information overall, but more description of select ITS technologies featured in it – and perhaps, with the time series element removed. A graph with high perceptibility and intuitiveness would still be one that presents the data in a familiar format (e.g., with time on the x-axis) to lend to easy understanding. 

<b>I also wanted to improve the aesthetics of the chart, in an effort to make in more engaging.</b> While the original blue color palette is visually appealing, I often found my eye drawn to the light blue color, which was the bar color for survey year 2013. The visual “hint” of the light blue is somewhat misleading, given more recent data and/or changes in the data over time are highlighted in the text writeup in the report for this chart. Thus, the aesthetics of the graph don’t highlight the story that the chartmaker wants to tell. To address this, I wanted to highlight in bright colors those technologies that a higher percentage of agencies deployed over time, which the report cites as “moveable” technologies (Portable CCTV and Portable Traffic Monitoring Devices) and Queue Detection Systems. This would engage the viewer’s eye in the most important information, which I would reinforce with a descriptive title highlighting the key takeaways. In essence, I wanted to leverage the themes in the report writeup as visual guides in the chart, to ensure that a report reviewer casually flipping through could glean the key takeaways without having to sift through the full context of the writeup. 
<br>

<div class="wrapper">
  <div class="column">
    <img src="C1- IMG-3653.jpg" width="400"/>
  </div>
  <div class="wrapper">
    <img src="C2- IMG-3654.jpg" width="400"/>
  </div><br>
</div>
<br>
When I started on my wireframe sketches, above, I found myself struggling to find a title that effectively captured the report’s key takeaways without being verbose. I also found myself repeatedly using the word “deployed,” across both the technical and non-technical audience chart, thinking that deployed would be apparent to the viewer. Deployed, as I intended it, meant the number of responding agencies that deployed a given technology. As I would soon discover in my interviews with a data engineer in his late twenties (Interviewee A) and a student in his mid-twenties (Interviewee B), <b> the use of the word “deployed” was a serious point of misunderstanding.</b> When asked what he thought “deployed” meant, Interviewee B said that it meant how many of a certain type of technology were in utilization in a given year, while Interviewee B stated that he wanted to know what “deployed” meant. This was a signal to me to remove, or clarify, this language in both graphs – especially in the non-technical graph – likely by adding a more descriptive y-axis title. To reinforce this, in the final version, I decided to add clarification on the survey sample in an annotation describing the sample size across years. 

While Interviewee A said that he was able to quickly deduce the two-tone color scheme of the non-technical chart, Interviewee B mentioned that he was confused by it. While I tried to lump the portable technologies into one color (blue) and the queue detection system into another (green), Interviewee B wasn’t sure why two lines were blue and one was green. Despite the positive feedback from Interviewee A, <b>this was a sign that, without a legend, the color scheme would be unclear for the technical audience chart.</b> Because I did not want to weigh the chart down with a legend, I decided to remove the two-tone color scheme and simply color the “unimportant” lines grey, and the lines of interest green, to indicate that they had increased. 

Interviewee A also mentioned that he did not like title of the technical chart, in particular, the phrasing “make deployment gains.” He suggested language that framed the increases in technology rates in terms of the agencies: e.g., “More agencies report deployment of XYZ.” This was a point well taken, as the word “deploy” and “deployment” were consistent points of confusion across the interviews.

The feedback for the non-technical audience chart was strong. <b>While I tried to design a simpler chart that was more descriptive in nature, Interviewee A noted that he thought that the chart felt overloaded and felt very technical.</b> Interviewee B also noted that a lay audience would not find the chart approachable and that he thought the chart would be best suited to someone with an interest in traffic engineering. I realized that I needed to simplify the chart much more than I had; simply altering the color scheme and adding text were not enough. In this vein, I decided to remove all but three lines: 2 high-performers (Queue Detection and Portable CCTV) and 1 lesser-used technology (Variable Speed Limits). This would allow me to narrow the scope of the chart, in the process highlighting more widely deployed, as well as emerging, ITS technologies in freeway work zones. 

Interviewee A also expressed that a nontechnical audience member probably wouldn’t feel that there were any “stakes” to the chart – the layout presented information, but there wasn’t a “why” to hook someone with little exposure to the topic. This was a point well taken when I was reconsidering the title of the chart. <b>I decided to emphasize how ITS can improve safety in work zones in the title, since road safety feels more relatable and less intimidating than technologies readers may have never heard of.</b> I then used annotations to describe what each of the three technologies were. 

The redesigned charts attempt to communicate data on the types of ITS technologies that transportation agencies use in freeway work zones to both a technical and nontechnical audience. For the technical audience graph, <b>the interviewees’ feedback allowed me to finetune the changes I had already begun implementing in the wireframes:</b>  transforming the stacked bar chart into a line chart and using color to highlight technologies that more agencies used over time. For the nontechnical audience chart, the interviewees’ feedback led me back to the drawing board. <b>Having sat with the data for a summer, I realized that I assumed that people might be more interested in ITS, but the interviews made me realize that I had to make the case for ITS if I wanted to engage people in the subject area.</b> I began to reimagine what would be manageable for someone with no background – or interest – in the topic. I continued to maintain a line chart format, but I settled upon a more general title that might draw readers in with the relatable theme of road safety. I then offered information on the selected technologies as annotations to provide context for the reader to go deeper. 

<br>
<br>

## Final Charts: 
### Technical Audience Chart: 
<div class='tableauPlaceholder' id='viz1663616168528' style='position: relative'><noscript><a href='#'><img alt='Increase in agencies reporting deployment of queue detection and portable technologies in freeway work zones State, regional, and local agencies managing freeways leverage different technologies to increase safety and mobility across survey years ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TechnicalAudience&#47;TechAudience&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TechnicalAudience&#47;TechAudience' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TechnicalAudience&#47;TechAudience&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object>
</div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1663616168528');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>
<br>
<br>
### Non-Technical Audience Chart: 
<div class='tableauPlaceholder' id='viz1663710777942' style='position: relative'><noscript><a href='#'><img alt='Technology can improve safety outcomes in freeway work zones — but transportation agencies prefer some over others ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;NO&#47;NONTechnicalAudience&#47;NonTechAudience-REAL&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='NONTechnicalAudience&#47;NonTechAudience-REAL' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;NO&#47;NONTechnicalAudience&#47;NonTechAudience-REAL&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object>
</div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1663710777942');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>
Source material for technology labels in Non-Technical Chart: 
<ul> Source material for technology labels in Non-Technical Chart: 
<li><a href="https://www.virginiadot.org/vtrc/main/online_reports/pdf/10-r20.pdf">Virginia DOT Report</a></li>
<li><a href="https://safety.fhwa.dot.gov/provencountermeasures/variable-speed-limits.cfm">FHWA Website</a></li>
<li><a href="https://www.its.dot.gov/infographs/queue_warning.htm">ITS DOT Queue Warning Graphic</a></li>
<li><a href="https://www.ison-tech.com/index.php/application/its">ISON Tech</a></li>
<li><a href="https://www.transportation.ohio.gov/programs/traffic-operations/its#page=1">Ohio DOT</a></li>
<br>
DOT ITS Survey Data:<br>
-[2020](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fwww.itskrs.its.dot.gov%2Fsites%2Fdefault%2Ffiles%2Fdoc%2F2020_FM_data.xlsx&wdOrigin=BROWSELINK)
<br>
-[2016](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fwww.itskrs.its.dot.gov%2Fsites%2Fdefault%2Ffiles%2Fdeployment-statistics%2Fdata%2F2016%2F2016_FM_data.xlsx&wdOrigin=BROWSELINK)
<br>
-[2013](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fwww.itskrs.its.dot.gov%2Fsites%2Fdefault%2Ffiles%2Fdeployment-statistics%2Fdata%2F2013%2F2013_FM_data.xlsx&wdOrigin=BROWSELINK) 

  
  
<br>
Finished? Return to the [homepage of the repository.](README.md)
