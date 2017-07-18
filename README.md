# TmapURLs

Tmap API URLs  (like Google Maps URLs)<br/>
**[Google Maps URLs](https://developers.google.com/maps/documentation/urls/guide)** 처럼 URL 링크를 사용해 Tmap을 보여줍니다

## Map actions
### search
검색 결과를 맵에 marker로 표시하고 이름을 툴팁으로 띄웁니다.

* Search URL 형식<br/>
  https<i></i>://b1uec0in.github.io/tmapurls/search/?***parameters***

* Parameters<br/>
  * **query** (required): 맵에 표시할 장소.<br/>
    * *[latitude,longitude]* 형식을 사용하면 WGS84 좌표계를 사용해 장소를 표시합니다.<br/>
      name parameter가 지정되지 않으면 툴팁은 표시되지 않습니다.
    * *[keyword]* 형식을 사용해 주소나 키워드로 장소를 검색하여 표시할 수 있습니다.<br/> 
      name parameter가 존재하지 않는경우 장소의 이름이 툴팁으로 표시됩니다.

  * **query_place_id** (optional) : 맵에 표시할 장소의 id<br/>
    * place id는 장소의 고유 식별자입니다. Tmap POI ID 값을 사용합니다.
    * query parameter는 반드시 존재해야합니다. <br/>
      place id 검색이 실패하면 query를 사용해 다시 검색합니다.<br/>
      place id 검색이 성공하면 query는 사용되지 않습니다.<br/>
  
  * **name** (optional): marker에 표시할 이름.
    * query[keyword], query_place_id 로 검색한 경우 name parameter를 지정하지 않더라도 POI name 값이 표시됩니다.
    * query[latitude,longitude]로 검색한 경우 name parameter를 사용하지 않으면 marker에 이름이 표시되지 않습니다.

### !주의! ###
parameter value는 항상 url encode 해야합니다. (일부 브라우저는 자동으로 인코딩해주기도 하지만 그렇지 않은 경우를 대비해 항상 인코딩하십시오.)


## Example
[https://b1uec0in.github.io/tmapurls/search/?query=37.5065731,127.0546535&name=SK%20TechX](https://b1uec0in.github.io/tmapurls/search/?query=37.5065731,127.0546535&name=SK%20TechX)<br/>
[https://b1uec0in.github.io/tmapurls/search/?query=SK%ED%85%8C%ED%81%AC%EC%97%91%EC%8A%A4](https://b1uec0in.github.io/tmapurls/search/?query=SK%ED%85%8C%ED%81%AC%EC%97%91%EC%8A%A4)<br/>
[https://b1uec0in.github.io/tmapurls/search/?query=SK%ED%85%8C%ED%81%AC%EC%97%91%EC%8A%A4&query_place_id=6818494](https://b1uec0in.github.io/tmapurls/search/?query=SK%ED%85%8C%ED%81%AC%EC%97%91%EC%8A%A4&query_place_id=6818494)


## Related Links
* Github project:<br/>
[https://github.com/b1uec0in/tmapurls](https://github.com/b1uec0in/tmapurls)

* API page:<br/>
[https://b1uec0in.github.io/tmapurls](https://b1uec0in.github.io/tmapurls)

* Google Maps URLs guide:<br/>
[https://developers.google.com/maps/documentation/urls/guide](https://developers.google.com/maps/documentation/urls/guide)

