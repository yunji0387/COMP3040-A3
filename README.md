# COMP3040-A3

# Winnipeg Transit API

## Description: 
 1. Our API is straightforward, requiring simply a GET request to https://api.manitoba-transit.com/bus/number/list/json?stop=? When the user provides the bus stop number and the name of the bus stop is returned as the endpoint.

## Endpoints:

 1. Browse bus schedule by bus stop and date

 2. Browse list of bus number(differnt route bus) by bus stop

 3. Browse list of stop location by bus number
 
 4. List all bus number ??
 
 5. List total bus amount ??

## Description of resources - formatted as JSON:

 1. 

## Sample request with sample response:

 1. Browse bus schedule by bus stop and date
     - sample request :
    ```
         https://api.manitoba-transit.com/bus/schedule/json?stop=82578&date=2022-07-30 
    ```
     - sample response : 
    ```
         {
           "results":
           {
            [
             {
               "bus-number": "850"
               "bus-name": "Brandon",
               "arrival-time": "2022-07-30T02:53:42"
             },
             {
               "bus-number": "500"
               "bus-name": "Thompson",
               "arrival-time": "2022-07-30T04:58:02"
             },
             {
               "bus-number": "20"
               "bus-name": "Winkler",
               "arrival-time": "2022-07-30T05:38:36"
             }
           ],
            "status":"OK"
         }
    ```

 2. Browse list of bus number by bus stop
     - sample request :
    ```
         https://api.manitoba-transit.com/bus/number/list/json?stop=82578 
    ```
     - sample response : 
    ```
         {
           "results":
           {
            [
             {
               "bus-number": "850"
               "bus-name": "Brandon"
             },
             {
               "bus-number": "500"
               "bus-name": "Thompson"
             },
             {
               "bus-number": "20"
               "bus-name": "Winkler"
             }
           ],
            "status":"OK"
         }
    ```
 3. Browse list of stop location by bus number
     - sample request :
    ```
         https://api.manitoba-transit.com/bus/stop/list/json?number=850 
    ```
     - sample response : 
    ```
         {
           "results":
           {
            [
             {
               "stop-number": "82577"
               "stop-name": "Brandon-Killarney"
             },
             {
               "stop-number": "82578"
               "stop-name": "Brandon-Freedman"
             },
             {
               "stop-number": "82579"
               "stop-name": "Brandon-Dalhousie"
             }
           ],
            "status":"OK"
         }
    ```

## Group 07 - Members
 - [Kim, Gyuri (KIMG2)](https://github.com/gyuyuu)
 - [Anghan, Dharmit Kishorbhai (ANGHANDK)](https://github.com/dkanghan)
 - [Ahir, Md Ahiduzzaman (AHIRMA)](https://github.com/AhirGit)
 - [How, Yun Ji (HOWYJ)](https://github.com/yunji0387)

## Reference
 1. https://api.winnipegtransit.com/home/api/v3/services/destinations
 2. https://api.winnipegtransit.com/home/api/v3/services/routes
 3. https://api.winnipegtransit.com/home/api/v3/services/stops
