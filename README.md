# Roman Numerals Converter Application (Python Flask) deployed on AWS EC2 with Cloudformation and AWS CLI
## Description
The Roman Numerals Converter Application aims to convert the given number to the Roman numerals. The application is to be coded in Python and deployed as a web application with Flask on AWS Elastic Compute Cloud (EC2) Instance using AWS Cloudformation and CLI Services. 

## Problem Statement

- Your company has recently started on a project that aims to be one of the most used unit converters and formulas website. Roman Numerals Converter is the part of the project. So you and your colleagues have started to work on the project.

- As a first step of the project, you need to write program that converts the given number (between 1 and 3999) to the roman numerals. The program should convert only from numbers to Roman numerals, not vice versa and during the conversion following notes should be taken into consideration.
   
```
Roman numerals are represented by seven different symbols: I, V, X, L, C, D and M.
- Symbol       Value
- I             1
- V             5
- X             10
- L             50
- C             100
- D             500
- M             1000
- For example, two is written as II in Roman numeral, just two one's added together. 
Twelve is written as, XII, which is simply X + II. 
The number twenty seven is written as XXVII, which is XX + V + II.
- Roman numerals are usually written largest to smallest from left to right. 
However, the numeral for four is not IIII. Instead, the number four is written as IV. 
Because the one is before the five we subtract it making four. 
The same principle applies to the number nine, which is written as IX. 
There are six instances where subtraction is used:
- I can be placed before V (5) and X (10) to make 4 and 9. 
- X can be placed before L (50) and C (100) to make 40 and 90. 
- C can be placed before D (500) and M (1000) to make 400 and 900.
```

- User input can be either integer or string, thus the input should be checked for the followings,

   - The input should be a decimal number within the range of 1 to 3999, inclusively.
   
   - If the input is less then 1 or greater then 3999, user should be warned using the given html template.

   - If the input is string and can not be converted to decimal number, user should be warned using the given html template.

- Example for user inputs and respective outputs

```
Input       Output
-----       ------
3           III
9           IX
58          LVIII
1994        MCMXCIV
-8          Warning with "Not Valid! Please enter a number between 1 and 3999, inclusively."
4500        Warning with "Not Valid! Please enter a number between 1 and 3999, inclusively."
Ten         Warning with "Not Valid! Please enter a number between 1 and 3999, inclusively."
```
   
- As a second step, after you finish the coding, you are requested to deploy your web environment using Python's Flask framework.

- You need to transform your program into web application using the `index.html` and `result.html` within the `templates` folder. Note the followings for your web application.
   
   - User should face first with `index.html` when web app started.

   - User input should be taken via `index.html` using http post method
   
   - If user input is not valid, user should be warned using the `index.html` with template formatting.

   - Conversion result should be displayed using the `result.html` with template formatting. 

- After transforming your code into web application, you are requested to push your program to the project repository on the Github and deploy your solution in the development environment on AWS EC2 Instance using AWS Cloudformation Service to showcase your project. In the development environment, you can configure your Cloudformation template using the followings,

   - The application stack should be created with new AWS resources. 

   - The application stack should take the name of your Key Pair as a parameter from the user;
   
   - The application should run on Amazon Linux 2 EC2 Instance

   - EC2 Instance type can be configured as `t2.micro`.

   - Latest AWS Linux AMI should be used for template.

   - Instance launched by Cloudformation should be tagged `Web Server of StackName` 

   - The Web Application should be accessible via web browser and terminal from anywhere.

   - The Application files should be downloaded from Github repo and deployed on EC2 Instance using user data script within cloudformation template. 

   - Roman Numerals Converter Application Website URL should be given as output by Cloudformation Service, after the stack created.

- Lastly, try to deploy same infrastructure using AWS Cli Service to showcase your project. 

## Project Skeleton 

```
AWS_Roman-Numerals-Converter (folder)
|
|----readme.md         # Definition of the project          
|----roman_number.yml  # Cloudformation template
|----app.py            # Python Flask Web Application
|----templates
        |----index.html  # HTML template
        |----result.html # HTML template
```


### At the end of the project, following topics are to be covered;

- Algorithm design

- Programming with Python 

- Web application programming with Python Flask Framework 

- Bash scripting

- AWS EC2 Service

- AWS Security Groups Configuration

- AWS Cloudformation Service

- AWS Cloudformation Template Design

- AWS CLI Service

- AWS CLI commands, filters and queries

- Git & Github for Version Control System

