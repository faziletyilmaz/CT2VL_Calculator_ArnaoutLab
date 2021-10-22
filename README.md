# CT2VL_USER_ADJUSTED (Arnaout-Lab)
## COVID CT to Viral Load Calculator 
### This docker file is calculating COVID Viral Load with given CT value 
### Calculation will be adjusted the user's RT_PCR 

Requirements:

- CSV data file
- Docker desktop app


#### Instructions

#### 1. Prepare your Raw data file from your RT_PCR output
- Each row represents a sample (You must have at least 10 positive sample to adjust your equaiton without error )
- Each colum represents cycle intensities (42 colums for 42 cycle)

#### 2. Save your Data file
- Make a directory(folder) in your computer (name it ct2vl_data)
- Save your file as data.csv file (extension MUST be **.CSV**)

#### 3. Download Docker destop 

- https://www.docker.com/products/docker-desktop
- follow the instructions

#### 4. Open your teminal 
- Spotlight search, or Applications/Utilities/Terminal 

Run the following codes in order

cd ../ct2vl_user_adjusted 

 
 



