# streaming-04-multiple-consumers

> Use RabbitMQ to distribute tasks to multiple workers

One process will create task messages. Multiple worker processes will share the work. 

## Before You Begin - Start A New Project

Follow this common workflow to start a new project by using this starter repo. 

1. In your browser, fork this repository into your own GitHub account. 
2. Clone your new GitHub repository down to your machine into your Documents folder.
3. Open your project folder in VS Code (if you haven't already).
4. In VS Code, if it doesn't already exist, add a useful .gitignore with a line for .vsode/ and .venv/ and whatever else doesn't need to go in the repo. Here's an example [.gitignore](.gitignore).
6. In VS Code, edit your README.md to record your commands, process, and notes so far.
7. Open a terminal in VS Code - PowerShell if Windows, zsh or bash if Mac/Linux.
8. Git add and commit with a useful message (e.g. "initial commit") and push to GitHub.

## Task 1. Create and Manage your Project Virtual Environment

We will use pika, which is not included in the Python Standard Library. We must install it. 
To keep our project separate from all other Python projects, we will create and manage a local project virtual environment.
We'll install our packages into the local project virtual environment.  
The steps in this common workflow are listed below.
For detailed steps, see [PROJECT_VIRTUAL_ENV.md](https://github.com/denisecase/streaming-03-rabbitmq/blob/main/PROJECT_VIRTUAL_ENV.md). 

1. Open your project folder in VS Code.
2. Open a terminal window in VS Code (PowerShell for Windows, zsh or bash for Mac/Linux). 
3. Use git pull first, to make sure you have the current project on your machine.
4. Use venv to create a new .venv environment in the repo on your machine. 
5. Activate your environment using the command for your operating system. 
6. Use pip to install necessary packages into your active project virtual environment.
7. In VS Code, edit your README.md and record your commands, process, and notes.
8. In VS Code, use View / Command Palette - then Python: Select Interpreter to use your .venv.
9. Use a terminal to Git add / commit / push to GitHub.
10. Verify your GitHub repository.   

## Read

1. Read the [RabbitMQ Tutorial - Work Queues](https://www.rabbitmq.com/tutorials/tutorial-two-python.html)
1. Read the code and comments in this repo.

## RabbitMQ Admin 

RabbitMQ comes with an admin panel. When you run the task emitter, reply y to open it. 

(Python makes it easy to open a web page - see the code to learn how.)

## Execute the Producer

1. Run emitter_of_tasks.py (say y to monitor RabbitMQ queues)

Explore the RabbitMQ website.

## Execute a Consumer / Worker

1. Run listening_worker.py

Will it terminate on its own? How do you know? 

## Ready for Work

1. Use your emitter_of_tasks to produce more task messages.

## Start Another Listening Worker 

1. Use your listening_worker.py script to launch a second worker. 

Follow the tutorial. 
Add multiple tasks (e.g. First message, Second message, etc.)
How are tasks distributed? 
Monitor the windows with at least two workers. 
Which worker gets which tasks?


## Reference

- [RabbitMQ Tutorial - Work Queues](https://www.rabbitmq.com/tutorials/tutorial-two-python.html)


## Screenshot

See a running example with at least 3 concurrent process windows here:
