# TravisLeaks :rocket:
A tool to find sensitive keys and passwords in Travis logs

![travis gif](https://user-images.githubusercontent.com/41824020/57980167-ef242900-7a44-11e9-8425-73560b1d1e0a.gif)

</br>

## Description
Read the Blog post [here](https://blog.shashank.co/2019/05/finding-leaks-in-travis-logs-automated.html)


Just enter the Travis user name of the organization. The script will automatically find out all jobs and then do two things:
1. Look for ED's keywords for potential leaks
2. Use the concept of entropy to find potential API keys in the logs 


## Requirements (using travisleak.py script)

> Python 3.X  
> ``` pip install requests ```

## Usage
> python travisleak.py travis_user_name

</br>

![travis_exe_1](https://user-images.githubusercontent.com/41824020/57980169-f2b7b000-7a44-11e9-97d9-80ce7635b546.png)

</br>

![travis_exe2](https://user-images.githubusercontent.com/41824020/57980170-f3e8dd00-7a44-11e9-9e03-f8e68aef96a9.png)

</br></br>

Credits:-


The keywords for the potential leak was taken from ED's blog post [here](https://edoverflow.com/2019/ci-knew-there-would-be-bugs-here/)


The concept of entropy was adapted from [here](https://github.com/dxa4481/truffleHog)



## Note
This tool still needs a lot of development. I would be glad if someone would like to contribute to this project.

## Goals
- [x] Better output format 
- [ ] Support CircleCI scans
