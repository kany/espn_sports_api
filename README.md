espn_sports_api
===============

ESPN Sports API

Setup Url with Key
url = 'http://api.espn.com/v1/sports/football/nfl/teams.json?apikey=7yqmdnm394k2k4sqyrhqwf7b'

Fetch url
resp = Net::HTTP.get_response(URI.parse(url))  

Parse url
result = JSON.parse(resp.body)

Response
{"sports"=>[{"name"=>"football", "id"=>20, "uid"=>"s:20", ....
