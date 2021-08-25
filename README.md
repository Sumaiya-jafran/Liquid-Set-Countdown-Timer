# Liquid-Set-Countdown-Timer (works)
set countdown timer in your store header for announce product sale or another things you want

create a section named "timer.liquid"
create a file in assets named "timer.css"
create a file in assets named "timer.js"

then call .css and .js file in theme.liquid  in the following way:

<link rel="preload" href="{{ 'timer.js' | asset_url }}" as="script">
<link rel="stylesheet" href="{{ 'timer.css' | asset_url }}" type="text/css" media="print" onload="this.media='all';onLoadStylesheet()">
  
  
  we can add these two file(.css and .js) in another way too:
   {{ 'timer.css' | asset_url | stylesheet_tag }} 
   {{ 'timer.js' | asset_url | script_tag }}  
