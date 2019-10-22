# nikeplus_scrape

Inspired by https://gist.github.com/niw/858c1ecaef89858893681e46db63db66

headers = {'appid': 'fuelband', 'Accept': 'application/json'}

r = requests.get('https://api.nike.com/sport/v3/me/activities/after_time/0?access_token=%s' % (token), headers=headers)

r.json()['paging']

r = requests.get('https://api.nike.com/sport/v3/me/activities/after_time/0?access_token=%s&page=2' % (token), headers=headers)

r = requests.get('https://api.nike.com/sport/v3/me/activities/after_time/1186083079000?access_token=%s' % (token), headers=headers)

curl -v -H 'Authorization: Bearer [token]' 'https://api.nike.com/sport/v3/me/activity/787021039?metrics=ALL'
