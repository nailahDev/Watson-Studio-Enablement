# Predicting Machine Failure: Exploring Device Data from Watson IoT Platform using Jupyter Notebooks 

1. Start from Watson Studio's main dashboard.  
![1](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Images/1.png)
<br></br>

2. Import a dataset (can be found in the current folder on this GitHub repository, named 'cc_applications.csv').  
![2](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Images/2.png)
<br></br>

3. Now we can find the dataset in the **Data Assets** panel.  
![3](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Images/3.png)
<br></br>

4. Create a new **Notebook**.  
![4](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Images/4.png)
<br></br>

5. Select the **From URL** tab to import a notebook.  
![5](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Images/5.png)
<br></br>

6. Type in a name for your notebook. In the **Notebook URL** field, type the following url:  
- [https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Predicting%20Machine%20Failure%20Notebook.ipynb](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Predicting%20Machine%20Failure%20Notebook.ipynb)

Then click **Create**.  
![6](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Images/6.png)
<br></br>

7. Now you can see the notebook. It will have all the details for developing the model and deployment steps.  
![7](https://github.com/nailahDev/Watson-Studio-Enablement/blob/master/02-Predictive%20Maintenance%20Notebook/Images/7.png)
<br></br>

8. After deployment of the model from the notebook, you can access the trained model from the **Models** panel. Select **Credit Card Approval Model**.    
![8](https://github.com/HebaNAS/IBM-Watson-Studio-Enablement/blob/master/02-CreditCardApprovalModel/imgs/8.jpg?raw=true)
<br></br>

9. To check the deployment, click on the **Deployment** tab.  
![9](https://github.com/HebaNAS/IBM-Watson-Studio-Enablement/blob/master/02-CreditCardApprovalModel/imgs/9.jpg?raw=true)
<br></br>

10. To test the model on new data, click on **Test** tab.  
![10](https://github.com/HebaNAS/IBM-Watson-Studio-Enablement/blob/master/02-CreditCardApprovalModel/imgs/10.jpg?raw=true)
<br></br>

11. Select raw input (you can choose to use the form interface as well), copy the data from this gist [https://gist.github.com/HebaNAS/6998045745a5689f42260cb1239d1024](https://gist.github.com/HebaNAS/6998045745a5689f42260cb1239d1024) and paste it in the input field, then hit **Predict**.  
![11](https://github.com/HebaNAS/IBM-Watson-Studio-Enablement/blob/master/02-CreditCardApprovalModel/imgs/11.jpg?raw=true)
<br></br>

12. Now you can see the model's prediction for the input we provided.  
![12](https://github.com/HebaNAS/IBM-Watson-Studio-Enablement/blob/master/02-CreditCardApprovalModel/imgs/12.jpg?raw=true)
<br></br>

13. You can choose to view the predictions in a Chart format.  
![13](https://github.com/HebaNAS/IBM-Watson-Studio-Enablement/blob/master/02-CreditCardApprovalModel/imgs/13.jpg?raw=true)
<br></br>
