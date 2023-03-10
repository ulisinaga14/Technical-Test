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

8. Run request, is it running well? 
9. Add listener to see the result. Thread Group -> Add -> Listener -> View Result Tree
![image](https://user-images.githubusercontent.com/107898121/224202082-fb60f491-179e-4954-be2a-b015cfbf67d1.png)

10. Click Start button to run the request. 
![image](https://user-images.githubusercontent.com/107898121/224202154-358c9685-7508-4b9b-94dd-2bd43c6c3314.png)

11. The request is running well.

12. Add Test Data. Thread Group -> Add -> Config Element -> CSV Data Set Config.
![image](https://user-images.githubusercontent.com/107898121/224202608-80cc1735-0772-418b-bbc5-e48d4a86d5cd.png)

13. Browse test data you can use. Click Browse button -> choose your test data with CSV extension.
![image](https://user-images.githubusercontent.com/107898121/224202873-422bc283-50f2-4d53-923f-75d19b0c2144.png)

14. Update value fields : {variable_name} according to the test data.
15. Go to Weather Request then update value fields.
![image](https://user-images.githubusercontent.com/107898121/224204261-59447121-38a0-40e4-b7b7-62dae4409ad7.png)

16. Go to Forecast Request then update value fields.
![image](https://user-images.githubusercontent.com/107898121/224204446-52c5ac6e-579c-49b6-a2c9-cd1661a93118.png)

17. Run and validate is the request is running well.

18. There is an error request.
![image](https://user-images.githubusercontent.com/107898121/224205034-83c78077-6830-4cc2-a4f8-8d77f86e1bc2.png)

19. Fix it and validate again.

20. The request is running well.
![image](https://user-images.githubusercontent.com/107898121/224205152-e7590bcc-807a-4a51-94d7-d72d6281b0da.png)






