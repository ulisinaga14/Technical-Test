Peformance Test

Write Performance tests for the API Testing where you hit both APIs

Steps :
1. Open Apache JMeter,create new Thread Group. Test Plan -> Add -> Threads(User) -> Thread Group 
![image](https://user-images.githubusercontent.com/107898121/224200902-5e44149b-505a-40fa-a241-d84542cbf495.png)

2. Add API Weather Request. Thread Group -> Add -> Sampler -> HTTP Request.
![image](https://user-images.githubusercontent.com/107898121/224200341-7dea0244-77ab-43b6-b63d-c4ecd6eac771.png)

3. Give HTTP Request name, protocol, Server name (IP), HTTP Request, and Path
* HTTP Request name : Weather Data
* protocol : https
* Server name (IP) : api.weatherbit.io
* HTTP Request : GET
* Path : /v2.0/current
![image](https://user-images.githubusercontent.com/107898121/224200509-4736986d-6e29-4e9d-8747-333da24935f8.png)

4. Add Parameters. Click Add button -> fill parameter name and value.
* lat : 40.730610
* lon : -73.935242
* key : 634bf1d8955a47ea814c61d187f93364
![image](https://user-images.githubusercontent.com/107898121/224201084-c8690a26-f8e5-4950-98e1-bf196f323a7a.png)

5. Add API Forecast Request. Thread Group -> Add -> Sampler -> HTTP Request.
![image](https://user-images.githubusercontent.com/107898121/224201256-e3d85a7c-bb18-45a0-9da0-36634da1c5b0.png)

6. Give HTTP Request name, protocol, Server name (IP), HTTP Request, and Path
* HTTP Request name : Forecast Hourly 
* protocol : https
* Server name (IP) : api.weatherbit.io
* HTTP Request : GET
* Path : /v2.0/forecast/hourly
![image](https://user-images.githubusercontent.com/107898121/224201414-d81237ce-2b88-404f-bab4-2476d0ee3241.png)

7. Add Parameters. Click Add button -> fill parameter name and value. 
![image](https://user-images.githubusercontent.com/107898121/224201498-2d8e77bb-0500-4afd-bedf-b1c12176dfec.png)






