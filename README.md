# Instagram Scrapy Scraper

> Some scrapy spiders useful to crawl instagram posts using public APIS (No TOKEN)

## Requirements
- Python
- Scrapy

## Spiders
- hashtag (crawl all the post given a hashtag)

## Usage

```python
scrapy crawl hashtag
```
Use the -L INFO to avoid a lot of debug messages

## Output
The scraper put its files under the *scraped* directory

### hashtag spider
File are put under *scraped/hashtag/hashtagname*, by date and hour of the day. This is because if you execute the crawler multiple times in the same hour the output is appended. Files contains a Json for each line.

For example :

```text
{"id": "1684344684669792291", "shortcode": "Bdf_pERD3Aj", "caption": "\"Non c'\u00e8 amore pi\u00f9 sincero di quello per il cibo\". Panino caldo e croccante con caciocavallo, zucchine grigliate e pesto di pomodori secchi. \ud83d\ude0b #myferrara #labellaferrara #volgoitalia #volgoemiliaromagna #volgoferrara #igersferrara #volgosapori #italia_in_grande #centrostorico #iconsigliati #visitferrara #cibobuono #cosebuone #qualit\u00e0 #passione #genuinit\u00e0 #freschezza #tagsforlikes", "display_url": "https://instagram.ffco2-1.fna.fbcdn.net/vp/71a6e1bc5183bbd9b1339f064b2bb1b9/5B231526/t51.2885-15/e35/25021917_402106523561566_9076772742774128640_n.jpg", "loc_id": 0, "loc_name": "", "loc_lat": 0, "loc_lon": 0, "owner_id": "5655088891", "owner_name": "tipicoh_ferrara", "taken_at_timestamp": 1515009554}
{"id": "1684875047875260104", "shortcode": "Bdh4O3fhi7I", "caption": "#roma #piazzanavona #pjmasks #sky #ballons #detail #thehub_lazio #lazio_illife #new_photolazio #yallerslazio  #arts_illife #vivolazio #volgolazio #lazio_super_pics #visit_lazio #italiaStyle20 #iconsigliati  #volgoarte #shotz_of_lazio", "display_url": "https://instagram.ffco2-1.fna.fbcdn.net/vp/20459e8002d4a61284bc7e03f0da5f8a/5B0B896A/t51.2885-15/e35/26065496_174719709946144_8885150857012707328_n.jpg", "loc_id": "336844629", "loc_name": "Piazza Navona", "loc_lat": 41.8988888889, "loc_lon": 12.4730555556, "owner_id": "256276180", "owner_name": "clapanama", "taken_at_timestamp": 1515072779}
```

## License
GNU GENERAL PUBLIC LICENSE Version 3