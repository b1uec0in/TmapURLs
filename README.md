# TmapURLs

Tmap API URLs  (like Google Maps URLs)

## Map actions
###search
The search action displays results for a search across the visible map region. When searching for a specific place, the resulting map puts a pin in the specified location and displays available place details.

* Forming the Search URL<br/>
  https://b1uec0in.github.io/tmapurls/search/?api=1&amp```parameters```

* Parameters<br/>
  * query (required): Defines the place(s) to highlight on the map. The query parameter is required for all search requests.<br/>
    * Specify locations as either a place name, address, or comma-separated latitude/longitude coordinates. Strings should be URL-escaped, so an address such as "City Hall, New York, NY" should be converted to City+Hall%2C+New+York%2C+NY.<br/>
    * Specify general search terms as a URL-escaped string, such as grocery+stores or restaurants+in+seattle+wa.



## Example
[https://b1uec0in.github.io/tmapurls/search/?api=1&query=4509961.60848102,14143597.62234898]()
[https://b1uec0in.github.io/tmapurls/search/?api=1&query=SK테크엑스]()

## References
* Github:<br/>
[https://github.com/b1uec0in/TmapURLs]()

* Google Maps URLs guide:<br/>
[https://developers.google.com/maps/documentation/urls/guide]()

