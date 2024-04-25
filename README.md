# fake_instagram_account_detection

## WORKING PRINCIPLE

1. **Initial Dataset:**
   - The initial dataset contained data of 1000 real accounts and 200 fake accounts. 
   - Filename: `dataset-withoutoversampling.xlsx`

2. **SMOTE Oversampling:**
   - Applied the SMOTE oversampling algorithm to balance the dataset.

3. **Final Dataset:**
   - The dataset after oversampling is stored in a file named `finaldataset.xlsx`.

4. **Dataset Features:**
   - `Column1.userFollowerCount`: Number of followers for the account (integer)
   - `Column1.userFollowingCount`: Number of accounts the user follows (integer)
   - `Column1.userBiographyLength`: Length of the user's biography text (integer)
   - `Column1.userMediaCount`: Total number of media posts by the user (integer)
   - `Column1.userHasProfilPic`: Binary indicator (1: has a profile picture, 0: no profile picture)
   - `Column1.userIsPrivate`: Binary indicator (1: private account, 0: public account)
   - `Column1.usernameDigitCount`: Number of digits present in the username (integer)
   - `Column1.usernameLength`: Total length of the username (integer)
   - `Column1.isFake`: Target variable indicating account type (1: fake account, 0: real account)

5. **Data Retrieval:**
   - Utilized the Python library Instaloader to retrieve real-time data of an account.
     For more information about Instaloader, refer to [its documentation](https://instaloader.github.io/).

6. **Model Usage:**
   - Input the retrieved data into our model to determine whether it is a fake or real account.

   OUTPUT:
   ![image](https://github.com/jacobrajweb/fake_instagram_account_detection/assets/149454092/891bb2a4-ea72-4782-8238-a3ce44e8154c)

   Now Enter the username, which you need to check 

   The output looks like below:
   ![image](https://github.com/jacobrajweb/fake_instagram_account_detection/assets/149454092/2c5f084d-58fe-4303-87e2-edc52631e7aa)
