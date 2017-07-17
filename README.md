# TmapURLs

Tmap API URLs  (like Google Maps URLs)

## Map actions
### search
The search action displays results for a search across the visible map region. When searching for a specific place, the resulting map puts a pin in the specified location and displays available place details.

* Forming the Search URL<br/>
  https<i></i>://b1uec0in.github.io/tmapurls/search/?api=1&***parameters***

* Parameters<br/>
  * query (required): Defines the place(s) to highlight on the map. The query parameter is required for all search requests.<br/>
    * Specify locations as either a place name, address, or comma-separated latitude/longitude coordinates. Strings should be URL-escaped, so an address such as "City Hall, New York, NY" should be converted to City+Hall%2C+New+York%2C+NY.<br/>
    * Specify general search terms as a URL-escaped string, such as grocery+stores or restaurants+in+seattle+wa.



## Example
[https://b1uec0in.github.io/tmapurls/search/?query=37.5065731,127.0546535](https://b1uec0in.github.io/tmapurls/search/?query=37.5065731,127.0546535)<br/>
[https://b1uec0in.github.io/tmapurls/search/?query=SK테크엑스](https://b1uec0in.github.io/tmapurls/search/?query=SK테크엑스)

## Related Links
* Github project:<br/>
[https://github.com/b1uec0in/tmapurls](https://github.com/b1uec0in/tmapurls)

* API page:<br/>
[https://b1uec0in.github.io/tmapurls](https://b1uec0in.github.io/tmapurls)

* Google Maps URLs guide:<br/>
[https://developers.google.com/maps/documentation/urls/guide](https://developers.google.com/maps/documentation/urls/guide)

