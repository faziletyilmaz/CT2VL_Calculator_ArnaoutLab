# COVID Ct value to Viral Load Calculator 
## Arnaout-Lab

### This Docker container is calculating COVID Viral Load with given CT value 
### Calculation will be adjusted the user's RT_PCR 

Requirements:

- CSV data file
- Docker desktop app


#### Instructions

#### 1. Prepare your Raw data file from your RT_PCR output
- Create new **.csv** data file (you can use microsoft excel "save as" funtion)
- Each row should represents single sample reading (You must have at least 10 positive sample to adjust your equaiton without error )
- Each column shoud represents raw cycle intensities readings (42 colums for 42 cycle)

#### 2. Save your Data file

- Make a directory(folder) in your computer (name it ct2vl_data)
- Save your file in the ct2vl_data directory 

#### 3. Download Docker desktop app (if you don't have)

- https://www.docker.com/products/docker-desktop
- Follow the instructions

#### 4. Open your teminal 

- Spotlight search, or Applications/Utilities/Terminal 

- Run the following codes in order

1.Change your current directory "ct2vl_data"


	cd ../ct2vl_data

2.Pull the Docker container
	
	docker pull faziletyilmaz/ct2vl_user_adjusted
	
3.Run the docker container

	
	docker run -i -v $PDW/ct2vl_data:/data faziletyilmaz/ct2vl_user_adjusted


#### 5. Enter your Ct value

- Enter your Ct Value (sample: 34.67)
- It will give you the Viral Load!
 
 