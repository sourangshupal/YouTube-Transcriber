A Cloud function that summarizes Youtube videos with OpenAI

### Demo:

Given this URL: https://www.youtube.com/watch?v=zLJv37NKSx8

Run this snippet of code:

```python
import requests

url = "<DEPLOYED-ENDPOINT>"

payload = {'url': 'https://www.youtube.com/watch?v=zLJv37NKSx8'}
files=[

]
headers = {}

response = requests.request("POST", url, headers=headers, data=payload, files=files)

print(response.json())

```

To get the following output:

```json
{
    "summary": "\nAs an assistant, I would summarize this Youtube video as a guide to learning Python quickly and efficiently. The speaker shares their own experience with learning the programming language and offers a clear roadmap for beginners to follow. They recommend starting with real-world projects and understanding key concepts such as installation, variables, control flow, data structures, functions, debugging, virtual environments, modules and libraries, and APIs. The speaker also provides a custom GPT tool to help with learning and suggests using open AI's API to further develop skills and work on personal projects. Overall, the video offers a comprehensive plan for learning Python in about 2 weeks with dedication. ",
    "title": "How I Would Learn Python FAST in 2024 (if I could start over) - YouTube",
    "transcript": "this is how I would Learn Python if I had to start over python is currently the most popular language for data science and Ai and is relatively simple to get started with it's flexible and it has a whole bunch of libraries that you can leverage in this video I'm going to give you a complete road map to Learn Python and get up and ready as fast as possible but here's the catch because everybody says that it's simple to get started with everybody assumes that they can learn it with very little effort and they forget that it's still a programming language it requires time and effort not necessarily to learn the syntax which is simple but understanding basic program pramming Concepts and applying them in the real world that can be very challenging as a beginner you're going to understand individual Concepts like Loops control flow and functions but you might struggle to see how they all fit together in a larger program and this was the case for me because the first language that I learned was PHP and this was back in the day and I learned it superficially at the beginning because I needed to build a website and I relied heavily on a framework then I needed to Learn Python and I learned it at a high level because I needed to do some scraping so my initial interactions with programming languages were to solve real world problems and when you do that you specifically learn the tools that you need in order to get the job done but that's not comprehensive and you're always going to feel like you don't know enough and I constantly felt like this throughout the years even if I constantly worked on new projects even if I constantly learned new Concepts I learned new libraries and Frameworks and I got the job done regardless I always felt like I didn't know enough and I think this is the curse of being self-taught so if I would start all over again and I would Learn Python I would still start by working on real projects because this giv gives you a clear purpose but I do some things differently and the first thing that I would do differently would be to have a clear road map that I can follow and this is in terms of Concepts that I need to know Concepts that I know that I need to cover and refresh before starting working on a project let's cover these main Concepts starting from the basics to intermediate and advanced topics that are all fundamental when you get started cuz for the basics you won't need to revisit them but for the intermediate and advanced topics you need to revisit them multiple times so that they make sense and the first up is installation setup and Basics and I recommend that you install python via the Anaconda distribution and this is the best option if you're interested in working on data science and AI related projects because it has all the necessary libraries up and ready and you'll need to write code using an ID and for this I recommend vs code even learning vs code properly will require some time so that you get used to the interface but it's worth it because this is the standard now now that you have these you need to learn about python variables and naming conventions then you can run your first hello world script and experiment with Python's interactive shell and now we can start with simple Concepts that are the foundation to everything you get strings numbers and booleans you need to look at string operations and methods you need to understand string immutability and advanced formatting also integers floats and you need to understand how to perform type conversion for example next you can get into data structures understand how lists dictionaries tools and sets how they actually work and you need to understand their individual particularities I recommend that you write this code yourself always type the code never copy paste from examples from chat GPT or stack Overflow you need to always write every character don't use Auto formatting or co-pilot because you're learning the basics it's important to take your time as you do when you're first learning how to write you focus a lot on calligraphy then right because you need to establish good patterns straight from the start and the mind has time to grasp all of these Concepts and it's the same with coding coming back to data structures looking to nested data structures both lists and dictionaries we're going to work a lot with these so you need to understand how they work Now's the Time to learn control flow eil statement Nest statements and tary operators for writing more concise statements also forign wild Loops because these are super important to understand and both are very straightforward and the last basic concepts that you need are list and dictionary comprehensions these look beautiful and you're going to use them a lot all of these Concepts you can go through them in maybe a day or two and these are just the basics but even for these Basics you need to revisit them every now and then now you have the habit of writing code yourself so keep going again don't copy paste code or autocomplete or Auto format if you make a mistake and the code doesn't work it's most probably a misspelling or some bad indentation or something simple next you can start looking at python functions you got to learn how to write basic functions with parameters and return values this will also lead you to understand variable scope and variable Lifetime and if your code doesn't work it's most probably because you're not closing a parenthesis or you have some bad indentation but you got to keep writing it yourself you need that practice in order to form your coding memory now it's also the best time to learn Lambda functions the syntax and use cases where they're best to be used and also you need to look into how to read from and to files and by now you covered a lot of ground in terms of Basics you made errors along the way so it's time to learn how to debug you need to look into reading and interpreting error messages and also use break points and set trays to perform step through debugging also you need to handle type errors and exceptions and use try accept statements it's actually try accept else finally statements also learn about common debugging strategies and best practices and this is important because you're going to do this a lot especially when you're using a lot of GPT created code and the last foundational topics for learning python are comments and dog strings writing effective comments alongside your code and dog strings for documentation is crucial in order to remember what you did and also for others to know what you did when they actually review your code it might feel that it's time consuming that you can do it later but believe me if you don't comment your code immediately and create the do strings for your functions you're going to forget and two months down the line you're going to come back to your spaghetti code and you're going to understand nothing from it up until now you probably spent a week or so learning these so you can go ahead and tell your friends that you learned python in a week and it's good to believe that you did but deep down you're going to know differently so you need to continue and you can continue with the following you need to understand python virtual environments because you won't always be working in your base Anaconda environment you need to learn why you need them how to create and manage virtual environments you need to look into virtual m p EnV and pipm they serve similar purposes but you got to find out the differences also learn about best practices when it comes to working with different project dependencies now your probably noticed that throughout the video I'm using a custom GPT that I've created specifically for the purpose of learning python I Incorporated the full detailed road map in it and I think it can support you on your path I think you can learn all of these Concepts fast and this GPT can guide you with further resources and clarifications I'll put a link down in the description for it and I really hope that it will help you let me know down in the comments if you do use it and if it helped you because based on that I may create other tutors that can help you on other topics and now that you learned a lot you need to learn a little bit more and by this I mean p modules and libraries and I'm talking about specifically the standard python libraries you're going to use math daytime random OS CIS ref for regular Expressions subprocess URL lib and a lot more that you can see here so cover these ones in detail so that you know exactly what you can leverage when you actually need it and now we only have one big chapter that you need to dive very very deep in and this is something that you're going to be using all of the time in your professional career apis restful apis and HTTP methods such as get post put and delete you got to look into the structure of an API request and the response you can work with Postman it will definitely help you a lot you got to learn how to work with Json data and send authenticated requests you need to spend as much time as needed here and you need to start using apis for example such as open ai's API because if you do so you're also going to be able to call yourself an AI engineer but really working with apis will also give you the ability to start working on your own projects where you can leverage some data from providers and this is the complete road map that you need to follow in order to start your python Journey with a little bit of dedication I think you can cover all of these in about 2 weeks but after these two weeks I think you're going to be ready to start working on a real project knowing that you're equipped with a broad understanding of python again you can use the custom GPD that I set up because you can also suggest ideas that you can work on so that you can solidify your python knowledge and I'm going to put the links down in the description and that's it for me for now hit the like button subscribe and I'll see you in the next one",
    "url": "https://www.youtube.com/watch?v=zLJv37NKSx8"
}

```


## Deployment 

### Install Chocolatey Windows

Docs :- https://docs.chocolatey.org/en-us/choco/setup/#more-install-options
CMD

```bash
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "[System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

POWERSHELL

```bash
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

Install Pulumi:

```bash
choco install pulumi
```

The infrastructure is written with Pulumi.

To deploy it, you need to run the following commands

```bash
pulumi config set gcp:project <YOUR-GCP-PROJECT>
pulumi config set gcp:region <YOUR-GCP-REGION>
pulumi up
```
