# fake_instagram_account_detection
WORKING PRINCIPLE
1)The initial dataset contained data of 1000 real account and 200 fake account.The filename of the initial dataset is dataset-withoutoversampling.xlsx
2)To have a small amount of data for both classes(Fake and Real) , we have applied SMOTE oversampling algorithm.
3)The dataset after oversampling is stored in file named finaldataset.xlsx
4)The features contained in the dataset are 
             Column1.userFollowerCount: Number of followers for the account (integer)
             Column1.userFollowingCount: Number of accounts the user follows (integer) 
             Column1.userBiographyLength: Length of the user's biography text (integer)
             Column1.userMediaCount: Total number of media posts by the user (integer)
             Column1.userHasProfilPic: Binary indicator (1: has profile picture, 0: no profile picture)
			 Column1.userIsPrivate: Binary indicator (1: private account, 0: public account)
             Column1.usernameDigitCount: Number of digits present in the username (integer)
             Column1.usernameLength: Total length of the username (integer)
             Column1.isFake: Target variable indicating account type (1: fake account, 0: real account)
5)We have the python library instaloader to retrieve real time data of an account. And we input the retrieved data into our model to find whether it is fake account or real account.
6)Refer https://instaloader.github.io/ , to know more about instaloader

OUTPUT:
![image](https://github.com/jacobrajweb/fake_instagram_account_detection/assets/149454092/891bb2a4-ea72-4782-8238-a3ce44e8154c)

Now Enter the username , which you need to check 

The output looks like below , 

![image](https://github.com/jacobrajweb/fake_instagram_account_detection/assets/149454092/2c5f084d-58fe-4303-87e2-edc52631e7aa)
