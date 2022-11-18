# hackatum2022

## The challenge



## API

### Search for Sixt Stations

`https://api.orange.sixt.com/v1/locations?term=<SEARCH>&vehicleType=<TYPE>&type=station`

`<SEARCH>` free text search like "Garching"

`<TYPE> can be `car` or `truck`


### Station Details

`https://api.orange.sixt.com/v1/locations/<STATION_ID>`

`<STATION_ID>` id like `S_5252` from search endpoint


### Offers

`https://api.orange.sixt.com/v1/rentaloffers/offers?pickupStation=<STATION_ID>&returnStation=<STATION_ID>&pickupDate=<DATE>&returnDate=<DATE>&vehicleType=car&currency=EUR&isoCountryCode=DE`

`<STATION_ID>` id like `S_5252` from search endpoint
`<DATE>` e.g. `2022-12-14T14:00:00`
 
example: `https://api.orange.sixt.com/v1/rentaloffers/offers?pickupStation=S_5252&returnStation=S_5252&pickupDate=2022-12-14T14:00:00&returnDate=2022-12-16T14:00:00&vehicleType=car&currency=EUR&isoCountryCode=DE`


### Unlock / Lock / Blink Car

We have a Electric Renault Twingo outside. This car can be unlocked / locked / blink via API 

`https://api.orange.sixt.com/v2/apps/hackatum2022/twingo/unlock`

`https://api.orange.sixt.com/v2/apps/hackatum2022/twingo/lock`

`https://api.orange.sixt.com/v2/apps/hackatum2022/twingo/blink`


