# Hello-App
# Tried to run locally - First install flask
-pip install flask 
# then run it 
- python hello.py 
# The application is running on server given
# we then created a repo and added this code by commiting and pushing the code to the repository
# I had created an jenkins cicd build which automatic triggers when the github code is updated or changed
Steps 
1. First configure the job by adding the Repository url of github in the source code management option
2. In the build steps select github hook trigger for Scm polling
3. Then in execute shell from build steps option type present working directory location where the pyhton file is located in the hello folder in order to display hello world onto the console output
4. Save & apply
5. In the github repo, go to the settings option and select webhooks and fill the payload url by typing the following [jenkinsprojecturl/github-webhooks], then select content type and the push event.
# Then we also deploy in onto aws by creating and ec2 instance connecting it through ssh and cloning the repository, then installing all the packages given in req.txt file and running the file. The hello world app is up and running.
# then we installed and enable grafana , and copied the localhost with 3000 port no and paste it in url tab the grafana was up and running with login page
# Then I monitored it using grafana created a folder in garfana then dashboard, then new visualization, then selected the style [graph], then added the url of application in add links checkbox, along with title and associated the folder that was created earlier.
7.The app was monitored using grafana 
