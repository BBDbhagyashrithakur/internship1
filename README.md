# internship1_Database Design



![flow3](https://github.com/BBDbhagyashrithakur/internship1/assets/159768548/6073dc12-221f-43e7-8d35-d2d9b6647a95)

User Table:

![Screenshot 2024-02-15 152437](https://github.com/BBDbhagyashrithakur/internship1/assets/159768548/7432fb0c-d996-4315-b833-e6b172c2fa91)

User_profile table:

![user_Profile](https://github.com/BBDbhagyashrithakur/internship1/assets/159768548/f82ee6e6-7502-4616-90cd-5c91bbb4b816)


Application table:

![user_application](https://github.com/BBDbhagyashrithakur/internship1/assets/159768548/93bf5e09-55ba-4c77-acf5-9a03d0d9bf71)

Company table:
 ![Company_table](https://github.com/BBDbhagyashrithakur/internship1/assets/159768548/8437ee43-9383-469a-aeb4-3f7f1fe629af)

 Company_post Table:
 ![Company_post](https://github.com/BBDbhagyashrithakur/internship1/assets/159768548/ca93046c-8e45-4496-bcc6-e9505c1ace5c)



  
### procedure which display the Company information:
 
	DELIMITER //
        create procedure CompanyInfo()
        begin 
               select job_desc,job_title,job_role from Company_post where job_title='Software Developer';
        END //
        DELIMITER ;
 

	call CompanyInfo() //calling the procedure
 
 

	
#### view: to dispaly the job description:

create view  UserInfo as
  select u_id,u_name,u_email from User;
  
    
         select * from UserInfo;//Calling view

## Features
 
- Login
- Registration
-student Profile
- TPO profile
- Student Application
- TPO Approch
- Comapny post
 

