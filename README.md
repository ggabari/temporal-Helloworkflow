## Deploying a Golang Application with a Temporal CLuster for data persistency
Prequisites:
<ul>
<li>An EC2 Instance</li>
<li>Install git</li>
<li>Install golang</li>
<li>Install docker</li>
<li>Install docker-compose</li>

Thereafter clone this repository.

To begin, we set up the temporal server using docker-compose which can be found by navigating to the docker folder.
<li>while in the folder, run "docker-compose up -d" to run in detached mode, after all the dependencies have been set up, and image has been created</li>
Access the EC2 IP address on port 8080 and the result should look like the image below.

![Screenshot (241)](https://user-images.githubusercontent.com/64992501/216762510-851b00a5-0129-4dc5-b9f9-9a63f4d943bf.png)

<li>It shows no workflow, because we haven't run the command "go run ./worker/main.go"</li>

<li> Now run the command "go run ./worker/main.go" for the worker to be up </li> 
After it has successfully initialized, open a new terminal and run the next command. 
<li>"go run ./starter/main.go", to execute the Helloworkflow</li>
Then refresh your browser, the output should look like the images below.

  
![Screenshot (243)](https://user-images.githubusercontent.com/64992501/216762973-92f5c746-6ca2-4577-9790-9f21e419a8da.png)


<li>Then on the terminal navigate to the starter/ and edit output message in "main.go" file to validate the effectiveness of the workflow.</li>
  

  

# temporal-Helloworkflow
# temporal-Helloworkflow
# temporal-Helloworkflow
