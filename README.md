# Computeless Video Transcoding Pipeline
This solution provides you with details to create a compute less transcoding pipeline.  


## Servers :
You might be using inhouse trancoders on compute instances or VMs to transcode your VOD content. This is very common practice and we can achieve them usinf simple EC2 instance. But then we need to ensure the availability and uptime of servers. 

## Serverlesss :
Serverless doesn't mean than there are no servers in your workflow, it just mean we are not managing any servers or their uptime. Using Lambda to create a transcoding job, checking status and updating status on Database are some jobs achieved using these serverless compute. What is I told you dont need event these compute to create end-to-end transcoding pipleine.

## Computeless :
Again similar to serverlss computeless dont mean we are not using any compute, it means we are not managing or interacting with any compute instances while executing workflow. Zero code written and executed on compute and hence COMPUTELESS. AWS Step Functions are going to help us to achieve computeless workflows. Now you can automate any workflow, but I am chosing Video Transcoding with AWS elemental Mediaconvert as their is a small catch. MediaConvert is not available in the list of service integrations provided by Step Functions.  
