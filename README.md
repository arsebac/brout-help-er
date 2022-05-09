# brout-help-er
Helper tools that automatize identity theft, for educational-purpose only and after getting agreement of the target.

This tool will be enhanced with multiple scenarios and multiple level of automation

## Scenario 0 : Connect

We want to connect to Twitter and generate session cookies

Expected arguments : 


- ```--user``` Define Twitter username

- ```--pwd``` Define Twitter password

- ```--mfa``` Define Email or Phone number associated with the account. Not necessary if Twitter does not ask it

- ```--manual``` to force browser to be visible on first connection, so you can connect manually without defining user/password/phone

- ```--cookies``` Define cookies session persistance path. If this file exists, check if session is already connected

## Scenario 1 : RefaceAccount

For this scenario, we want Define PP, banner and description 
Expected arguments : 

- ```--picture``` Define image path or URL to use as Profile Picture

- ```--banner``` Define image path or URL to use as Banner Picture

- ```--description``` Define description url

- ```--user``` Define Twitter username

- ```--pwd``` Define Twitter password

- ```--mfa``` Define Email or Phone number associated with the account. Not necessary if Twitter does not ask it

- ```--cookies``` Define cookies session persistance path. If the file does not exists, connect to Twitter to generate session cookies

- ```--manual``` to force browser to be visible on first connection, so you can connect manually without defining user/password/phone


## Scenario 3 : CopyAccount

For this scenario, we want to copy PP, banner and description of a target Twitter account

Expected arguments : 

- ```--target``` Target Twitter account

- ```--rename``` Define new Twitter username

- ```--user``` Define Twitter username

- ```--pwd``` Define Twitter password

- ```--mfa``` Define Email or Phone number associated with the account. Not necessary if Twitter does not ask it

- ```--cookies``` Define cookies session persistance path. If the file does not exists, connect to Twitter to generate session cookies


## Scenario 4 : CopyTimeline

For this scenario, we want to create the same like/rt timeline of existing account
Expected arguments : 

- ```--target``` Target Twitter account

- ```--depth``` Define how many tweets should be copied. I.E, depth=5 means that CopyTimeline should copy only the 5 latest tweets

- ```--disable-like``` If 1 do not copy likes

- ```--disable-rt``` If 1 do not copy retweets

- ```--user``` Define Twitter username

- ```--pwd``` Define Twitter password

- ```--mfa``` Define Email or Phone number associated with the account. Not necessary if Twitter does not ask it

- ```--cookies``` Define cookies session persistance path. If the file does not exists, connect to Twitter to generate session cookies

## Scenario 5 : CheckFeasibility

This scenario will check some humans pattern that contains weakness that we could automatically exploit

Example : User A do a giveway and display the list of winners, and ask to MP User B to retrieve the gain. We can Copy winner of User A giveway and MP User B

- ```--target-tweet``` Target tweet

- ```--bank``` Target Twitter User B. If none are asked, this script will check every possibilty of a tweet

- ```--user``` Define Twitter username

- ```--pwd``` Define Twitter password

- ```--mfa``` Define Email or Phone number associated with the account. Not necessary if Twitter does not ask it

- ```--cookies``` Define cookies session persistance path. If the file does not exists, connect to Twitter to generate session cookies

