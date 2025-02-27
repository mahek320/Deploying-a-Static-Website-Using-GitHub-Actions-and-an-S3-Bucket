**Deploy a static website on AWS S3 bucket using GitHub action**

Step 1: 

i. Open your AWS account and create a S3 bucket


![Image 1](https://github.com/user-attachments/assets/efdce017-4f8f-4382-94f6-d2b82d049919)


ii. Uncheck the check box for block all public access 


![Image 2](https://github.com/user-attachments/assets/d17dcb60-5c7d-48ff-8d5b-b9554ec2eb57)


iii. Click on the acknowledge checkbox 


![Image](https://github.com/user-attachments/assets/5231fc83-defd-4108-b85d-40c7955383be)


iv. To enable static website hosting, navigate to the Buckets list and select the bucket you want to configure for static website hosting.


v. Choose properties 


vi. Under Static website hosting, choose Edit. 


![Image](https://github.com/user-attachments/assets/b84fbdf3-112f-4ae7-bb9d-2911ce63bfa3)


vii. Under Buckets, choose the name of your bucket.


viii. Choose Permissions.


ix. Under Bucket Policy, choose Edit. 


![Image](https://github.com/user-attachments/assets/8205bc89-42a3-4bba-b447-f5116f66cf6d)


Step 2:


i. Create a new repository in your GitHub account 


ii. Go to settings >> secrets and variables >> actions >> add new repository secret


![Image](https://github.com/user-attachments/assets/ffe84591-1cb0-43aa-8faa-97f59b0b50e3)


![image](https://github.com/user-attachments/assets/9c8a38c4-a255-4757-b4f7-7b5ac860f73d)


iii. Go to the main.yml file in your repository and change the bucket name and region and remove public from the code


![image](https://github.com/user-attachments/assets/0fed736e-628c-4f0d-9217-4066620edad9)


iv. Create an index file in the same repository


v. Click on actions in the git repository 


![Image](https://github.com/user-attachments/assets/0e108a6a-928e-4a6f-98bf-f46bd859bd2d)


vi. Once the job is successfully built


![Image](https://github.com/user-attachments/assets/a00fdefa-b38d-45ac-a311-4ca2c000df84)


vii. Under Static website hosting in your aws portal, click on the Endpoint URL post that copy paste the endpoint url in your web browser.


![Image](https://github.com/user-attachments/assets/69c40996-6404-4497-9810-6f72a29795a0)











