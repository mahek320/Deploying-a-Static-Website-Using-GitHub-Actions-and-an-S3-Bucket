## **🚀 Deploy a Static Website on AWS S3 Bucket using GitHub Action 🌐**


Step 1: 

i. Open your AWS account and create a S3 bucket    



<img src="https://github.com/user-attachments/assets/efdce017-4f8f-4382-94f6-d2b82d049919" width="500"><br>



ii. Uncheck the check box for block all public access    



<img src="https://github.com/user-attachments/assets/d17dcb60-5c7d-48ff-8d5b-b9554ec2eb57" width="500"><br>



iii. Click on the acknowledge checkbox    



<img src="https://github.com/user-attachments/assets/5231fc83-defd-4108-b85d-40c7955383be" width="500"><br>




iv. To enable static website hosting, navigate to the Buckets list and select the bucket you want to configure for static website hosting.    




v. Choose properties    




vi. Under Static website hosting, choose Edit.    




<img src="https://github.com/user-attachments/assets/b84fbdf3-112f-4ae7-bb9d-2911ce63bfa3" width="500"><br>    




vii. Under Buckets, choose the name of your bucket. 




viii. Choose Permissions. 




ix. Under Bucket Policy, choose Edit.  




<img src="https://github.com/user-attachments/assets/8205bc89-42a3-4bba-b447-f5116f66cf6d" width="500"><br> 




Step 2:    




i. Create a new repository in your GitHub account.    





ii. Go to settings >> secrets and variables >> actions >> add new repository secret





<img src="https://github.com/user-attachments/assets/ffe84591-1cb0-43aa-8faa-97f59b0b50e3" width="500"><br><br>    



<img src="https://github.com/user-attachments/assets/871d64a1-7bca-433a-af22-7a7b7a4491a8" width="500"><br>  





iii. Navigate to the main.yml file in your repository under .github/workflows, update the bucket name and AWS region, and remove any references to public. You can copy the main.yml file from the repository and modify it as needed.<br>  




<img src="https://github.com/user-attachments/assets/1824d73e-9821-4e3d-97b7-101f3ddeba33" width="500"><br>    



iv. Create an index file in the same repository **oustide** the .github/workflow folder. 

```yaml
<html xmlns="
http://www.w3.org/1999/xhtml"
>
<head>
<title>My Website Home Page</title>
</head>
<body>
<h1>Welcome to my website</h1>
<p>Now hosted on Amazon S3!</p>
</body>
</html>
```

   






v. Click on actions in the git repository.    




<img src="https://github.com/user-attachments/assets/0e108a6a-928e-4a6f-98bf-f46bd859bd2d" width="500"><br>    




vi. Once the job is successfully built.    




<img src="https://github.com/user-attachments/assets/a00fdefa-b38d-45ac-a311-4ca2c000df84" width="500"><br>     




vii. Under Static website hosting in your aws portal, click on the Endpoint URL post that copy paste the endpoint url in your web browser.    




<img src="https://github.com/user-attachments/assets/69c40996-6404-4497-9810-6f72a29795a0" width="500"><br> 











