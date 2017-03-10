For generating rules for admissions, the rules generated were all associations between rank and admit. 
I had to set the support and confidence parameters very low to get more than 1 result.

Looking at the graph visualization, it seems that by the transitive proprty you can derive any property involved in the rules 
from any other. The graph is a fully connected cluster.

----

The elect dataset produces a massive number of rules when minimum support is set to 0.02 or less. 1400 rules, specifically. 
They are all useless rules such as {KerryPct=58.37} => {State=New York}.

To find the states that Bush won I used the code: 

elect$State[elect$BushPct > 50]

which yielded 

[1] "Alabama"        "Alaska"         "Arizona"        "Arkansas"      
 [5] "Colorado"       "Florida"        "Georgia"        "Idaho"         
 [9] "Indiana"        "Kansas"         "Kentucky"       "Louisiana"     
[13] "Mississippi"    "Missouri"       "Montana"        "Nebraska"      
[17] "Nevada"         "North Carolina" "North Dakota"   "Ohio"          
[21] "Oklahoma"       "South Carolina" "South Dakota"   "Tennessee"     
[25] "Texas"          "Utah"           "Virginia"       "West Virginia" 
[29] "Wyoming"  

---

For the movies dataset, I found that while the range of years for all of the movies was 1938-2010, the range for the top 
50 movies is 1977-2010. (the 1977 movie is Star Wars: A New Hope)
