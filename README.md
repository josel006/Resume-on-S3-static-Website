# Resume-on-S3-static-Website

## How to create a Resume on S3 Bucket with Static Website.
This repository contains the steps to help you to create your Resume on S3 Bucket with Static Website.
Login to AWS and go to S3 console and click create bucket. The name must be unique across all the S3 buckets.
-	Uncheck the “Block all public access settings” (acknowledge the popup window).
-	Scroll down and click on Create bucket.
-	Click on the newly created bucket and select the Properties Tab.
-	Scroll down all the way down and on the Static website hosting click on Edit.
-	For Static website hosting select Enable.
-	On the Index document select copy and past the “detailed-resume.html” file name that is on this repository, this file contains all setting for your resume.
-	On the Error document type “error-html” which is on the repository as well.
-	Scroll down and click on Save changes.
-	Go to the permissions Tab and go to the “Bucket policy” and click Edit.
-	On the repository open the file named staticwebsitebucketpolicy.json and copy the policy.
-	Paste the policy in the Bucket policy window and make sure to edit the line #9 with the name of your created S3 Bucket on the above steps.
-	Go back to the S3 Bucket and click on the Object Tab
-	Click the “Upload Button” and drag and drop the “detailed-resume.html file, style.css, error.html, headshot.jpg” into the Files and folders window, scroll down and hit on Upload and then hit Close.
-	Go to the S3 bucket and click on the “Properties Tab” and scroll all the way down to the Static website hosting and copy the URL for your Static Website and open it on the new window browser.
-	At this point you should be able to launch your Static Website Resume and to be accessible from all the internet.
