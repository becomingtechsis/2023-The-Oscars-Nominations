# The Oscars Nominations 2023

## Introduction
The Oscars also known as American Academy Awards are awards for artistic and technical merit for the American film industry and are considered by some to be the most prestigious awards in the US entertainment industry.
For this visualization, I'll be using the Infographic Designer custom visual to create an isotype chart. 


## Visualization
- Kept only the rows and columns needed for the dashboard
- Sourced for Images from the Oscars website.
•	Created two measures.
- 1) Nominations by film
```Nominations = COUNT(the_oscar_award[year_ceremony])```

-	2) Selected category (this will be used to display which category users have selected from the slicer)
```Selected Category =``` 

```VAR _ConCat =```

```CALCULATE (```

```CONCATENATEX (```

```VALUES (the_oscar_award[category] ),```

```the_oscar_award[category],```

```", "```

```)```
   
```)```

```VAR IsItFiltered =```

```IF ( ISFILTERED ( the_oscar_award[category] ), _ConCat, "all award categories" )```

```RETURN```

```"for " & IsItFiltered```

- 	I used images from the Academy Awards site and used PowerPoint to create my background.
- 	I also used the WhatFont add-in to try to match fonts as close as possible
- Used the Infographic Designer custom visual to create a bar chart. Then used one of the sourced images to turn it into an Isotype.
- Added a slicer and styled it to match the report.
- Added a shape because it has more formatting options to add text that informs users which categories they have selected.
- Created a Slicer Panel
- Used buttons to create the appearance of the slicer, and use bookmarks to make the slicer appear and disappear.
- De-selected Data in the bookmark options.
