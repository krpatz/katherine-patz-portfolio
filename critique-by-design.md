| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Assignment: Critique and Re-design

## Step one: the visualization

Link to the original data visualization: https://makeovermonday.vercel.app/dataset/2022w36

I chose this visualization mostly out of personal curiosity around the topic. I am a 27 year old from Oklahoma and have found many of my former friends and classmates have gone on to get married, whereas I have not. When I saw the visualization, I thought it was straightforward and simple, but could definitely be improved upon. Also, the data itself was simple and clean, so I didn't feel intimidated about using it. 

## Step two: the critique
  I thought that the original data visualization was successful in being simple and stripped down- there was no unnecessary business, no confusing usage of color. It is easy to understand the upward pattern. But I thought this visualization was too stripped down- so much so that it doesn't even have a title, and it doesn’t label any of the dots for readers to reference what state they are from, and there is no baseline to compare the dots to. In addition, since one of the axis displays age, I thought it would be more intuitive to put age on the Y axis, as it is the dependent variable (the level of population density is affecting the age). 
  
  The intended audience of the graph was likely that of the American public, or anyone interested in exploring the differences between American states. While this data may have truthfully displayed the data, it was difficult to interpret and doesn't really leave audience members with any key takeaways. I also think there was something to be explored in terms of correlation vs causation with this data set. Instinctively, I assumed that higher population density is not what causes later ages in getting married, and was more likely a combination of things like education level, cost of living, political/social values, etc. 
  
  This critique helped me decide what I wanted to focus on for my redesign. I knew I wanted to explore if there are any interesting trends within the data set that I can highlight. I wanted to flip the axis. I also wanted to find some sort of average/trend line within this data set for audience members to use for comparison. I also wanted to provide a disclosure about correlation vs causation to increase truthfulness. 

## Step three: Sketch a solution

  This was probably where I spent the most amount of time on this assignment. Being very new to Tableau and not the most comfortable building data visualizations, I spent a lot of time trial and error-ing, trying to figure out how to get the image in my head onto the screen. After getting my data organized in a workbook, I played around a bit with different graph variations, but decided ultimately the scatter plot was the best as I could display a logarithmic trend line and see where different data points (the states) sat in relation to the trend line. I also scaled the X axis (population density) to better fit the logarithmic trend line, as before the majority of the data points were clustered in the lower, left hand side and were difficult to distinguish from one another. I then used Gen AI (claude) to help identify at which points states most closely followed the trend line, and found that states with pop density > 100 followed the trend line more closely than those with density < 100, and decided I wanted to make that my key takeaway, and had my title reflect this. Before the class critique/feedback session, I was still unsure how to add in a line at 100 and kind of grey out the variables I didn’t want to highlight.

  <img width="618" height="559" alt="Screenshot 2026-11-10 at 5 12 13 PM" src="https://github.com/user-attachments/assets/b7c2cb5b-f178-465f-bd56-8d53bdbcc471" />

This was the draft I had completed when coming into Tuesday’s class for feedback (the trend line was also visible)  
  
## Step four: Test the solution

When I asked my peers “Can you tell me what you think this is describing?”, everyone was easily able to determine that my visualization was illustrating the correlation between state population density and average female marriage age, and that higher population density correlated with higher average marrying age. One MISM student with a background in product management asked why the 100 marker for population density was chosen to be highlighted. I mentioned that the title and subcaption of the visualization helps explain. When I asked “Does any part of this feel particularly unintuitive?,” all students agreed the visualization was straightforward, uncluttered, and easy to interpret. When I asked “Is there anything you would change or do differently?”, the same MISM student recommended relying less on the title to explain my data, and more on the visualization itself to tell the story. I shared a similar opinion and wondered if this was something I could highlight via color or call outs in the chart. Another MISM student with a background as a system analyst questioned why not all of the points on the scatter plot were labeled with the state they represented. But we both agreed that displaying the names of ALL states would make the visualization too busy. The product manager MISM wondered if the size of the dots could indicate how close or far away from the trend line a data point is? While I thought this was a good idea to explore, I decided it was too easy for readers to incorrectly assume a larger sized data point meant the size of population density was larger. 

For my final redesign, I knew I had some work to do so that the visualization itself could better tell the story of the data without the reader needing to reference the title. 

## Step five: build the solution

<div class='tableauPlaceholder' id='viz1794514558413' style='position: relative'><noscript><a href='#'><img alt='Population Density Correlates with Women&#39;s Average Marrying Age in Dense US States, but not so much in Sparse Ones.States with a population density &gt; 100 show stronger correlation and fewer outliers compared to those with density &lt; 100.  ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ma&#47;MakeoverMondayChallenge_17945119353290&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='MakeoverMondayChallenge_17945119353290&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ma&#47;MakeoverMondayChallenge_17945119353290&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>             
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1794514558413');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

For my final redesign, I knew I wanted readers to be able to better intuit the key takeaway from the visualization rather than from the title. I also wanted to more clearly display the importance of the population density of 100 mark. I was able to accomplish this by highlighting the line that marks a population density of 100 on the scatterplot in red, and also using colors to differentiate the groups of states that had either a population density of > 100 or of < 100.

Compared to the original data visualization on MakeoverMonday, I believe my visualization, although also being a scatterplot, has a clearer point of view and a key take away for readers, uses the axis more intuitively to reflect the displayed variables, utilizes color in an intentional way, and takes more care not to relate any causation to correlation.

## References

Few, Stephen. “Data Visualization Effectiveness Profile.” Perceptual Edge. Accessed November 12, 2026. https://www.perceptualedge.com/articles/visual_business_intelligence/data_visualization_effectiveness_profile.pdf. 

## AI acknowledgements
AI Disclosure: I used Claude to help identify how to display a trend line in Tableau, and also to explore where the logarithmic trend was the strongest and weakest within the data set. 

