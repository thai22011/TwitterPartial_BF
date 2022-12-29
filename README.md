# An Overview of The 5.4M Leaked Twitter Accounts

All Emails and Phone Numbers were removed for Privacy Reasons

## INTRODUCTION

A security vulnerability in Twitter's API was exploited to steal over 5.4 million user records containing private information, which were subsequently shared on a hacker forum, Breached. The data was originally sold for  $30,000 in July 2022 and is now available for free. Let's do a EDA to understand more about the leaked accounts. All emails and phone numbers were removed for privacy reasons.

## Source

This file has been downloaded from BreachForums. Please check us out.
Our database list is provided here: https://breached.co/databases // http://breached65xqh64s7xbkvqgg7bmj4nj7656hcb7x4g42x753r7zmejqd.onion/databases

## User Data Dictionary
<span style = 'font-size:12px'>
| Attribute | Type | Description |
| :-: | :-: |:-: |
| id | Int64 | The integer representation of the unique identifier for this User. This number is greater than 53 bits and some programming languages may have difficulty/silent defects in interpreting it. Using a signed 64 bit integer for storing this identifier is safe. Use id_str to fetch the identifier to be safe. See Twitter IDs for more information. Example: "id": 6253282
| name | String | The name of the user, as they’ve defined it. Not necessarily a person’s name. Typically capped at 50 characters, but subject to change. Example: "name": "Twitter API"
|screen_name | String | The screen name, handle, or alias that this user identifies themselves with. screen_names are unique but subject to change. Use id_str as a user identifier whenever possible. Typically a maximum of 15 characters long, but some historical accounts may exist with longer names. Example: "screen_name": "twitterapi"                      
| location | String | Nullable . The user-defined location for this account’s profile. Not necessarily a location, nor machine-parseable. This field will occasionally be fuzzily interpreted by the Search service. Example: "location": "San Francisco, CA" 
| url | String | Nullable . A URL provided by the user in association with their profile. Example: "url": "https://developer.twitter.com"                                                                                                                                                                                       | description | String | Nullable . The user-defined UTF-8 string describing their account. Example: "description": "The Real Twitter API."                                                                                                                                                                                          
| protected | Boolean | When true, indicates that this user has chosen to protect their Tweets. See About Public and Protected Tweets . Example: "protected": true                                                                                                                                                                                       
| verified | Boolean | When true, indicates that the user has a verified account. See Verified Accounts . Example: "verified": false                                                                                                                                                                                      
| followers_count | Int | The number of followers this account currently has. Under certain conditions of duress, this field will temporarily indicate “0”. Example: "followers_count": 21
| friends_count | Int | The number of users this account is following (AKA their “followings”). Under certain conditions of duress, this field will temporarily indicate “0”. Example: "friends_count": 32
| listed_count | Int | The number of public lists that this user is a member of. Example: "listed_count": 9274                                                                                                                                                                                       
| favourites_count | Int | The number of Tweets this user has liked in the account’s lifetime. British spelling used in the field name for historical reasons. Example: "favourites_count": 13
| statuses_count | Int | The number of Tweets (including retweets) issued by the user. Example: "statuses_count": 42                                                                                                                                                                                         
| created_at | String | The UTC datetime that the user account was created on Twitter. Example: "created_at": "Mon Nov 29 21:18:15 +0000 2010"                                                                                                                                                                                      
| profile_banner_url | String | The HTTPS-based URL pointing to the standard web representation of the user’s uploaded profile banner. By adding a final path element of the URL, it is possible to obtain different image sizes optimized for specific displays. For size variants, please see User Profile Images and Banners . Example: "profile_banner_url": "https://si0.twimg.com/profile_banners/819797/1348102824" |
| profile_image_url_https | String  | A HTTPS-based URL pointing to the user’s profile image. Example: "profile_image_url_https": "https://abs.twimg.com/sticky/default_profile_images/default_profile_normal.png"
| default_profile | Boolean | When true, indicates that the user has not altered the theme or background of their user profile. Example: "default_profile": false
| default_profile_image | Boolean | When true, indicates that the user has not uploaded their own profile image and a default image is used instead. Example: "default_profile_image": false
</span>


## Conclusion


# Citation
Use this bibtex to cite this repository:

```
@misc{thai22011_Crypto_Clustering_PricePrediction_2022,
  title={An Overview of The 5.4M Leaked Twitter Accounts},
  author={Thai Nguyen},
  year={2022},
  publisher={Github},
  journal={GitHub repository},
  howpublished={\url{https://github.com/thai22011/TwitterPartial_BF}},
}
```

# Contribution
No Contribution is required


# Requirements

`tabulate` needs to turn datadframe to a markdown

```
conda create -n twitter_env python=3.8 numpy pandas matplotlib seaborn statsmodels scikit-learn jupyter jupyterlab plotly
conda activate twitter_env
conda install -c conda-forge fbprophet
conda install -c conda-forge pandas-profiling
conda install -c conda-forge sweetviz
conda install -c conda-forge autoviz
conda install -c conda-forge dtale
conda install tabulate
```
