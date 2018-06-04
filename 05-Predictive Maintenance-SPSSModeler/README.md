# Build and compare models performances using IBM SPSS Modeler

In this how-to, you will go through the process of preparing data and building a predictive model using IBM SPSS Modeler.

The business use case for this how-to is to assess the risk of a loan application, hence, approving the application and giving the loan to a customer or rejecting the application.  
The dataset used in this how-to is free, open-source and available here: [Predictive Maintenance Data](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/04-Predictive%20Maintenance%20-%20Exploring%20SensorsWMLModeler/sensorData-Training%20set.csv).  

The dataset contains details about customers applying for loans. Examples of the details available are: checking status, duration, credit history, purpose, credit amount, savings status, employment, etc.

IBM SPSS is availble on [IBM Watson Studio](https://dataplatform.ibm.com/home?context=analytics) as one of many options to build predictive models.

If you want more flexibility in preparing your data and building your models than what Watson Studio's Automatic Modeler offers, but still want the ease of use of a GUI interface and less code writing and complexity, you can use IBM SPSS Modeler for exactly that.
<br></br>

>> To upload the dataset to IBM Watson Studio and start working with it, refer to the screenshot below. 
![a](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/0.1.png)
<br></br>

1. Create a **New Flow** from Modeler Flows in the main dashboard of IBM Watson Studio.  
![1](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/1.png)
<br></br>

2. Type a **Name** for your Modeler task, select **Modeler Flow** as flow type and select **IBM SPSS Modeler** as runtime.  
![2](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/2.png)
<br></br>

3. Let's start by importing our dataset. Click on **Import** on the left-side panel.  
![3](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/3.png)
<br></br>

4. Drag and drop **Data Assets** node into the Modeler canvas, Double-click the node on the canvas to start editing its properties. 
 
![4](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/4.png)
<br></br>

5. Click on **Change Data Asset** to define the source of our data.  
![5](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/5.png)
<br></br>

6. A list of all the data assets you have in this project will be listed. Let's select `sensorData-Training set.csv`, available [here](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/04-Predictive%20Maintenance%20-%20Exploring%20SensorsWMLModeler/sensorData-Training%20set.csv).  
 
After selecting the dataset, click **Ok**.  
![6](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/6.png)
<br></br>

7. Making sure the dataset is imported. Click **Save**.  
![7](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/7.png)
<br></br>

8. Let's check our data quality. Drag and drop **Data Audit** node.  
![8](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/8.png)
<br></br>

9. Connect the nodes.  
![10](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/9.png)
<br></br>

10. Let's run the flow to get the results of the data audit.  
![11](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/10.png)
<br></br>

11. Wait for the process to finish.  
![12](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/11.png)
<br></br>

12. In the right-side panel, under the **Outputs** tab, let's select the most recent output (most recent is always on top) to view the results of running the flow so far.  
![12](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/12.png)
<br></br>

13. We get an idea about some statistics of the data and the distribution of the features. We find that the data needs some kind of normalization.  
![13](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/13.png)
<br></br>

14. Let's go back to our Modeler and continue working there.  
![14](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/14.png)
<br></br>

16. We want to split our data into Train and Test sets, we will do so using the **Partition** node.  
![16](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/15.png)
<br></br>

17. Double-clicking on the **Partition** node to explore its properties. We'll leave everything as it is.  
![17](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/16.png)
<br></br>

18. We'll add **Auto Data Prep** to automatically find issues in our dataset and fix it.  
![18](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/17.png)
<br></br>

19. We'll do another **Data Audit** to check the results of the previous step.  
![19](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/18.png)
<br></br>

20. View the results.  
![20](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/19.png)
<br></br>

21. The data has been normalized and issues have been fixed.  
![21](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/20.png)
<br></br>

22. Now let's select a model, let's try **C&R Tree**.  
![22](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/21.png)
<br></br>

23. Double-clicking on the **C&R** node to change its properties. Check **Use custom field roles**, then select `Target_transformed` as the target(labels) column and select all other columns as **Inputs**. Click **Save**.  
![23](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/22.png)
<br></br>

24. Let's run the flow.  
![24](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/23.png)
<br></br>

25. Wait for the process to finish. It may take a few minutes.  
![25](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/24.png)
<br></br>

26. After the model runs, it will produce a new node that holds information about the performance of the model.  
![26](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/25.png)
<br></br>

27. Let's add an **Analysis** node to peek into the model results node.  
![27](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/26.png)
<br></br>

28. Connect the nodes.  
![28](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/27.png)
<br></br>

29. View the output.  
![29](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/27.png)
<br></br>

30. Information about how our model performed.  
![30](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/28.png)
<br></br>

31. I added a few other models for comparison. Feel free to try your own combinations.  
![31](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/29.png)
<br></br>

32. If we click on the **C&R Tree** model node again and choose **View model**, we will get more detailed information about different performance metrics.  
![36](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/30.png)
<br></br>
![37](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/31.png)
<br></br>
![38](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/32.png)
<br></br>
![39](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/33.png)
<br></br>

33. Checking another model's performance (LSVM) as we did in the previous step.  
![32](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/34.png)
<br></br>
![33](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/35.png)
<br></br>
![34](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/36.png)
<br></br>
![35](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/37.png)
<br></br>

34. We're satisfied with our second model, it has better overall performance. Let's click on its node **LSVM** and select **Save branch as model**.  
![40](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/38.png)
<br></br>

35. Type a name for your model and a machine learning service should be detected and added automatically. Then click **Save**.  ![41](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/39.png)
<br></br>

36. The model has been saved successfully.  
![42](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/40.png)
<br></br>

37. You can access it in the Models panel in the main dashboard.  
![43](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/05-Predictive%20Maintenance-SPSSModeler/Images/41.png)
<br></br>


You can easily iterate through these steps and do some tweaks in the configuration options of each step/node to achieve better accuracy.
