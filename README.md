<h1 align="center">Yelp-Scraping</h1>
<a href="https://www.yelp.com">
  <div align="center">
    <br><img align-"center" src="https://leakdetectives.biz/wp-content/uploads/2019/12/review-yelp.png" width='300'/>
  </div><br>
</a>

>This project is mainly used to collect business and customer data from Yelp.com for getting information of [Solar companies](https://www.yelp.com/search?find_desc=Solar&find_loc=New+York%2C+NY%2C+United+States/).

### Why is Yelp Important for Business?
Yelp is essential for business because it allows customers to leave reviews and feedback about their experiences. This helps other potential customers make informed decisions about whether or not to patronize a particular business. In addition, companies can use Yelp to track their customer satisfaction levels and make necessary improvements.

Yelp also provides businesses with an advertising platform. Companies can create ads that target potential customers in their area. This is a great way to reach new customers and grow your business.

Overall, Yelp is essential for businesses to connect with their customers and grow their business.

### Is Yelp Helpful?
As a business owner, you may wonder if Yelp is worth your time. After all, there are a lot of reviews on there, and it can be tough to keep track of them all. And what if someone leaves a negative review?

Well, Yelp can be quite helpful for businesses. First, it’s a great way to get your business name out there. People are always searching for companies on Yelp, so if you’re not listed, you could miss out on potential customers.

Yelp can also be a great way to get feedback from customers. You can see what people liked and didn’t like about your business and make changes accordingly. And if you do get a negative review, you can use it as an opportunity to improve your business.

So if you’re wondering whether or not Yelp is worth your time, the answer is yes! It’s a great way to promote your business and get customer feedback.
<a href="https://www.enterpriseappstoday.com/stats/yelp-statistics.html">
  <div align="center">
    <img align-"center" src="https://user-images.githubusercontent.com/83681204/133468776-bae63ce1-7e78-4e35-a14d-f5f329d8098b.jpg"/>
  </div>
</a>
I hope this blog will help you understand. - <a href="https://www.enterpriseappstoday.com/stats/yelp-statistics.html">
  Yelp Statistics 2024 By Business Category, Star Rating Distribution, Visitors, Platform, Country and Consumers
</a> 

## Yelp Scraper
> You can scrape a bunch of comprehensive information of companies for specific field such as company name, website link, phone number, located address, owner name, provided services and several contact informations.

- *Name:* Sunation Energy
- *Website link:* sunation.com
- *Phone number:* +1 (631) 892-7245
- *Located address:* 171 Remington Blvd Ronkonkoma, NY 11779
- *Services offered:* EV charging stations, Add solar panels, Solar rooftop panel installation, Solar system maintenance, Add to existing system, Solar system installation, Solar shingle installation, Solar system repair
- *Owner name:* Scott Maskin
- *Supported area:* [(40.727172, 73.814309), (40.582027, 73.769150), (40.582027, 73.423253), (40.609850, 71.856214), (41.290122, 71.856214), (41.290122, 73.497061), (40.922801, 73.769150), (40.752494, 73.814309), (40.727172, 73.814309)] (with coordinates from...)



| Number | Name          | Website           | Phone          | Address                    | Owner   |
|--------|---------------|-------------------|----------------|----------------------------|---------|
| 1      | Sunation Energy| sunation.com      | (631) 892-7245 | 171 Remington Blvd Ronkonkoma, NY 11779 | Scitt M.  |
| 2      | Exact Solar   | exactsolar.com    | (267) 748-0596 | 82 Walker Ln Newtown, PA 18940 | Doug E. |
| 3      | EmPower Solar | empower-solar.com | (516) 837-3459 |                            | Daid S.   |
|...|...|...|...|...|...|

## Cities Selector
> You can also get cities which located in service provided area.

### Coordinates Finder
You can get coordinates of cities using Google Search.

<a href="https://www.google.com/search?q=philadelphia+longitude+latitude">
  <div align="center">
    <img align-"center" src="https://raw.githubusercontent.com/BeautifulMoon211/Yelp-Scraping/refs/heads/auxiliary/coor_detect.png" width='80%'/>
  </div>
</a>

It is required to use [smtplib](https://mailtrap.io/blog/python-send-email/) for Google Search.
```
NEW JERSEY, WOODLAND TOWNSHIP: 39.8537, -74.5229
ILLINOIS, OAK BROOK DU: 41.840794, -87.952377
CONNECTICUT, MERIDEN NEW: 41.53666666666666, -72.79472222222222
WASHINGTON, OMAK: 48.411, -119.5276
NEW HAMPSHIRE, FRANKLIN: 43.4442, -71.6473
...
```

### Cities Selector
Based on coordinates from Yelp Scraper and Coordinates Finder, let's find cities which located in the area the company supported.

<a href="https://www.yelp.com/map/sunation-energy-ronkonkoma">
  </br><div align="center">
    <img align-"center" src="https://www.nature.org/maps-static-image?zoom=8&size=600x300&markers=40.871996,-72.998811" width='315px'/>
  </div></br>
</a>

```
These cities are in the blue box!!!
The totla number of cities :  177
Cities are :  ['LARCHMONT', 'GREAT NECK ESTATES', 'KINGS POINT', 'MAMARONECK', 'LAWRENCE', 'GREAT NECK', 'CEDARHURST', 'SANDS POINT', 'HARRISON', 'MANORHAVEN', 'THOMASTON', 'ELMONT', 'WOODMERE', 'LAKE SUCCESS', 'VALLEY STREAM', 'FLORAL PARK', 'PORT WASHINGTON NORTH', 'NORTH VALLEY STREAM', 'MANHASSET', 'PORT WASHINGTON', 'HEWLETT', 'NORTH NEW HYDE PARK', 'NEW HYDE PARK', 'RYE', 'FLOWER HILL', 'MUNSEY PARK', 'FRANKLIN SQUARE', 'MALVERNE', 'LYNBROOK', 'EAST ROCKAWAY', 'PORT CHESTER', 'LONG BEACH', 'ISLAND PARK', 'LAKEVIEW', 'ROSLYN', 'WEST HEMSTEAD', 'ROSLYN HEIGHTS', 'WILLISTON PARK', 'SEA CLIFF', 'ALBERTSON', 'ROCKVILLE CENTRE', 'LOS PADRES NATIONAL FOREST SANTA', 'LAND', 'MINEOLA', 'OCEANSIDE', 'EAST WILLISTON', 'GARDEN CITY', 'GLEN COVE', 'GREENWICH', 'EAST HILLS', 'HEMPSTEAD', 'BALDWIN', 'CARLE PLACE', 'OLD BROOKVILLE', 'OLD WESTBURY', 'UNIONDALE', 'ROOSEVELT', 'WESTBURY', 'FREEPORT', 'BROOKVILLE', 'NORTH MERRICK', 'BAYVILLE', 'SOUTH WESTBURY', 'EAST MEADOW', 'MERRICK', 'JERICHO', 'STAMFORD', 'NORTH BELLMORE', 'OYSTER BAY', 'BELLMORE', 'HICKSVILLE', 'LEVITTOWN', 'WANTAGH', 'SYOSSET', 'RIDGEFIELD', 'NEW CANAAN', 'SEAFORD', 'BETHPAGE', 'MASSAPEQUA', 'DARIEN', 'PLAINVIEW', 'NORTH MASSAPEQUA', 'LLOYD HARBOR', 'COLD SPRING HARBOR', 'MASSAPEQUA PARK', 'OLDBETHPAGE', 'FARMINGDALE', 'SOUTH FARMINGDALE', 'WILTON', 'HUNTINGTON', 'EAST FARMINGDALE', 'AMITYVILLE', 'MELVILLE', 'HUNTINGTON BAY', 'HUNTINGTON STATION', 'NORWALK', 'COPIAGUE', 'SOUTH HUNTINGTON', 'MANATI', 'WESTON', 'LINDENHURST', 'CENTERPORT', 'GREENLAWN', 'WYANDANCH', 'WESTPORT', 'WEST BABYLON', 'NORTHPORT', 'DIX HILLS', 'ELWOOD', 'DEER PARK', 'BABYLON', 'EAST NORTHPORT', 'NORTH BABYLON', 'WEST ISLIP', 'FORT SALONGA', 'EASTON', 'COMMACK', 'BRIGHTWATERS', 'FAIRFIELD', 'KINGS PARK', 'BRENTWOOD', 'BAY SHORE', 'ISLIP', 'HAUPPAUGE', 'CENTRAL ISLIP', 'TRUMBULL', 'SMITHTOWN', 'BRIDGEPORT', 'ISLIP TERRACE', 'ETOWAH MC', 'EAST ISLIP', 'NESCONSET', 'ST. JAMES', 'STONY BROOK', 'OAKDALE', 'STRATFORD', 'BOHEMIA', 'LAKE GROVE', 'LAKE RONKONKOMA', 'SETAUKET-EAST SETAUKET', 'CENTEREACH', 'WEST SAYVILLE', 'SAYVILLE', 'HOLBROOK', 'PORT JEFFERSON', 'BAYPORT', 'PORT JEFFERSON STATION', 'HOLTSVILLE', 'SELDEN', 'FARMINGVILLE', 'LONG BEACH LA', 'MOUNT SINAI', 'ORANGE NEW', 'PATCHOGUE', 'CORAM', 'MEDFORD', 'EAST PATCHOGUE', 'MILLER PLACE', 'SOUND BEACH', 'NORTH BELLPORT', 'MIDDLE ISLAND', 'BELLPORT', 'ROCKY POINT', 'RIDGE', 'SHIRLEY', 'MASTIC BEACH', 'MASTIC', 'CENTER MORICHES', 'RIVERHEAD', 'NORTHVILLE', 'EAST QUOGUE', 'MATTITUCK', 'HAMPTON BAYS', 'SOUTHAMPTON', 'NOYACK', 'SAG HARBOR', 'MONTAUK']
```

## Wordpress Detector
> If you append `/wp-admin` or `/wp-login.php` to the website's URL and it takes you to a login page, it is likely a WordPress site. Check whether the modified path is valid or not.

## Social Contact Scraper
> Parse any website and find the spicific pattern for social contact information. Scrape them as much as possible.
```
Social contact information: https://www.youtube.com/@sunationenergy
                            https://www.instagram.com/sunationenergy
                            https://twitter.com/SUNation_Energy
                            https://www.linkedin.com/company/sunation-energy
                            https://www.tiktok.com/@sunationenergy
                            leads@sunation.com
                            https://www.facebook.com/SUNationEnergy
```
