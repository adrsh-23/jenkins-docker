# Jenkins and Docker

### In this project

1. We create a dockerfile in order for us to launch a jenkins containing docker container
2. We used that container to launch the jenkins 
3. In jenkins 
  * We created job1
    > This job is used to get the code from the github and copy that file to a folder 
    > This file will be used the webserver container to get the code
    > To get the code we have used GITSCM to get the code whenever the developer pushes the code to github
    
  * In job2 
    > This job will create a docker container with patting enabled also we'll mount the volume containing the file 
    > We'll use the httpd image to host our webserver
    
  * In job3
    > This job will check whether the site is working or not properly
    > Here we'll use the concept of working site having 200 code
    
  * In job4
    > This job will check whether the container having the webserver has not stopped due to some problems
    > If it would have stopped so we'll create a new container quickly using this job
    
 4. All the above jobs are connected using the build pipeline

## Preview/ Images: 

<p style="float: left">
    <img src="/job1.PNG" />
    <img src="/job2.PNG" />
    <img src="/job3.PNG" />
    <img src="/job4.PNG" />
</p>
 

