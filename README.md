# lambda-basic-auth
lambda function to create basic and simple auth

## Step 1 

'Open AWS Lambda service in N. Virginia Region and click on Create Function. Then you need to Select Author from scratch. Provide your Desired Function Name and keep runtime as Node.js 10.x. Lastly type Create.'


## Step 2 

Select Lambda create your own and insert the index.js into the block. Then click on ‘Save’ on the top right corner. Click on ‘Actions’. And from the drop-down list select “Publish New Version” and provide a name for the version.


## Step 3 

Select “Add trigger”.

##Do the following in the trigger configuration.

Cloudfront from the drop-down list.

From Distribution Dropdown list Select the CloudFront you wish to use for basic authentication.

Keep Cache Behavior with ‘*’.

Select ‘Viewer Request’ From ‘CloudFront event’.

Tick the Acknowledgement Windows.


## Step 4 

Then open another Tab of AWS and Open IAM. Click on Roles and select the role you have created. Then click on the ‘Trust Relation’ Tab and edit with 'Trust-Relationship.json' in this repo


# Step 5 


Final Step: Activate AWS Lamda@Edge for Basic Authentication
For the last step, go back to Lambda Page and create ‘Add’. You are done and good to go.
Browse your URL of CloudFront or the domain associated with it. You will find it with basic authentication available. You need to test with all our browsers.

