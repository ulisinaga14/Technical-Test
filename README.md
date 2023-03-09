UI AUTOMATION

Make above test as data-driven so that search items can be replaced with anything in step 4 and filtered result in Step 5 

Steps :
1. Create test cases for the search function, then create a script to search certain data.
![image](https://user-images.githubusercontent.com/107898121/224080985-203bcc2c-b429-445e-a55e-b1334a51e062.png)

2. Prepare the data to be tested, Click on Data Files -> New -> Test Data
![image](https://user-images.githubusercontent.com/107898121/224084104-6b2a61f4-2f2c-47d7-a239-8ed1dcdb9fe8.png)

3. Give the test data a name.
![image](https://user-images.githubusercontent.com/107898121/224084663-edbe8236-ffdf-4d61-8066-a856cb87cb69.png)

4. Click on the Browser button -> import your test data files
![image](https://user-images.githubusercontent.com/107898121/224085313-7f866a01-b99d-4526-ad36-14681742be5a.png)

5. Press CTRL + S to save your data

6. Go to Test Cases -> click on Variables -> add your variable name and the value.
![image](https://user-images.githubusercontent.com/107898121/224085943-252b4dba-89c1-481d-80eb-2c0d47e0b646.png)

7. Define variables in the test case.
* Double click "Apply for a number plate" input text -> double click String value type 
* choose variable -> define the variable -> click ok
![image](https://user-images.githubusercontent.com/107898121/224088413-524d9e81-a8d3-4417-b81f-83795092fa0d.png)

* Double click "Sydney Domestic Airport 2020" input text -> double click String value type
* choose variable -> define the variable -> click ok
![image](https://user-images.githubusercontent.com/107898121/224090268-83c2b71b-05c4-4523-bf11-3b1ef9f1f8f5.png)

* Go to script -> Delete this blocked script
![image](https://user-images.githubusercontent.com/107898121/224091128-3f7b789c-c383-49e4-811b-eb2acd70fc7e.png)

* Add the following script to create a variable on the object to be clicked on:

String service = 'Rockdale Service Centre'

TestObject service_name = findTestObject('Object Repository/Page_Find a Service NSW location  Service NSW/a_Rockdale Service Centre', 
    [('service') : service])

WebUI.click(service_name)

* Then paste to the script as bellow
![image](https://user-images.githubusercontent.com/107898121/224104590-02c87db4-8914-4c6c-aa66-0076352a2bf4.png)

8. Create Test Suites. Test Suites -> New -> Test Suite
![image](https://user-images.githubusercontent.com/107898121/224094036-82e4837e-ecc8-4074-ad3b-90705f0b7aea.png)

9. Give test suite name, click ok
![image](https://user-images.githubusercontent.com/107898121/224094834-4369d236-6c57-4128-8a7e-87c70fd470a9.png)

10. Add Test Case in the Test Suite
![image](https://user-images.githubusercontent.com/107898121/224095966-677fcb6c-2c7a-4bf3-9370-fc33f51da156.png)

11. Click Show Data Binding
![image](https://user-images.githubusercontent.com/107898121/224097270-d858adc0-bdc6-4469-919e-8d0b3a0c0de2.png)

12. Add test data you want to execute.
![image](https://user-images.githubusercontent.com/107898121/224098094-1477ee26-e341-452b-8b4b-f46673959dea.png)

13. Pick the Data Variable from column. Double click Type -> Choose Column (Do this for all variables)
![image](https://user-images.githubusercontent.com/107898121/224099270-85df941b-5694-4fb6-a498-2208f880c128.png)

14. Pick the Test Data from which file you want to take data file
* Double click Test Data -> choose Test Data (Do this for all Test Data) -> click ok
![image](https://user-images.githubusercontent.com/107898121/224101200-87ecf041-3e00-4b74-a321-b6f7120d98b2.png)

15. Select the column that corresponds to the value (Do this for all value)
* Double click value -> Choose column name -> click ok.
![image](https://user-images.githubusercontent.com/107898121/224101780-ca010510-6f89-4087-b2d6-8bc81c2628cf.png)

16. Press CTRL + S.

16. Run Test Suite. 
![image](https://user-images.githubusercontent.com/107898121/224108659-a49a70d7-1eaa-4f35-acf8-e0013836ab8c.png)








