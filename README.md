# COMP3040-A3

# Winnipeg Transit API

## Description: 

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
         https://api.manitoba-transit.com/schedule/json?stop=82578&date=2022-07-30 
    ```
     - sample response : 
    ```
         {
           "results":
           {
            [
             {
               "number": "850"
               "name": "Brandon",
               "time": "2022-07-30T02:53:42"
             },
             {
               "number": "500"
               "name": "Thompson",
               "time": "2022-07-30T04:58:02"
             },
             {
               "number": "20"
               "name": "Winkler",
               "time": "2022-07-30T05:38:36"
             }
           ],
            "status":"OK"
         }
    ```

 2. Browse list of bus number by bus stop
     - sample request :
    ```
         https://api.manitoba-transit.com/schedule/json?stop=82578 
    ```
     - sample response : 
    ```
         {
           "results":
           {
            [
             {
               "number": "850"
               "name": "Brandon"
             },
             {
               "number": "500"
               "name": "Thompson"
             },
             {
               "number": "20"
               "name": "Winkler"
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
