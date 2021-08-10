# Nodemon + Go

<p align="center">
  <img src="preview.png">
  <br>
</p>

<br>

**Background**

Hey! When developing an application in the go language, it is necessary to restart it every time through the console in order to apply new changes, this is not convenient. I propose to sprinkle it. I will be using the npm nodemon package.

# Start 🚀

Install nodemon globally

    npm install -g nodemon

<br>

For easy launch of the application, I will create a Makefile.

    run: main.go
	    nodemon --exec "go run" main.go

Here to nodemon we pass the launch parameters and the application itself.

<br>

To run the application

    make run