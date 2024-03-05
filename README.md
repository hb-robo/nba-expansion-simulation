It's 2024. The NBA is the most saturated with talent that it's ever been. Expansion is inevitable. 
But where does it lead? What cities mark the next locations in NBA history? What are the consequences of expansion as far as the redrawing of conference and division lines?
This is a small Python project that tries to answer some of those questions.

Leverages the following free data sets from SimpleMaps:
* https://simplemaps.com/data/us-cities
* https://simplemaps.com/data/world-cities

# TODO
* assemble list of cities in North America
  * find and map coordinates to each
  * find and map population data to each
  * find and map corresponding media market name to each
  * find and map (or calculate) media market size to each
    * if difficult to find, can calculate an estimate by following TV Market maps to sum populations within market lines
      * use relative rankings to adjust for minimum/maximums and overall order
* filter out sub-optimal expansion candidates
  * exclude cities smaller than another in its media market
  * exclude cities smaller in marketsize
* determine best expansion candidates for 2-team, 4-team, and 6-team expansion scenarios
* use hierarchical clustering to determine dividing line between conferences
  * must cut dendrogram to ensure N/2 teams per conference
* use clustering to determine dividing lines between divisions within conferences
  * explore benefits of 4-, 5-, 6-, and 8-team divisions, depending on number of teams
* generate / re-appropriate hypothetical team branding materials for chosen candidates
* generate map with superimposed team logos along with conference and division lines
* document results and methodology in README writeup along the way
