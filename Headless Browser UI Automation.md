Configuring headless browsers

Steps :
1. Go to Project -> Settings -> Desired Capabilities -> WebUI -> Chrome (headless)/ Firefox (headless).
![image](https://user-images.githubusercontent.com/107898121/224213620-d0e7e2ec-2afe-4447-9023-b55cb3420cda.png)

2. Click Add, provide Name, Type and Value of the property that you wish to configure.

3. To start Chrome maximized by default. Click Add on the command toolbar, then type in the following value:
* Name : args
* Type : List
* Value : []
![image](https://user-images.githubusercontent.com/107898121/224215274-4ed8b77d-8e2d-4395-8650-c310e3c8df36.png)

4. Then Click the small rectangle button
![image](https://user-images.githubusercontent.com/107898121/224215117-83db7dc5-9746-4ffc-b58d-17621f1e097d.png)

5. Click Add button, type in the following value:
![image](https://user-images.githubusercontent.com/107898121/224215425-5d590182-394f-4129-889b-07fdd8f3779c.png)

6. Click Apply and close.

7. Go to Test Suite, then click the drop-down beside the run button. 
8. Choose Chrome (headless)
![image](https://user-images.githubusercontent.com/107898121/224215749-39313e9d-64b4-4472-8820-f64f21df8a30.png)


