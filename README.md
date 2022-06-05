## Lab 7

[Home](https://liv-edi.github.io/cit281/)

In this lab we created our own GitHub organization for the CIT Minor, cerated our first GitHub repositories, cloned the repo to our local systems, created lab javascript file and initilaized folder as a Node.js folder, updated and commited lab JS file to practice error handling, and pushed our changes to GitHub.

Technologies used in this lab:
- VSCode
- Node.js
- GitHub
- git

The purpose of this lab was to gain experience ussing GitHub, git, committing changes to JS files, pushing changes to GitHub.

```
class CustomError extends Error {
    constructor(errName) {
        super(errName);
        this.name = "CustomError";
    }
}

function throwGenericError() {
    throw new Error("Generic error");
}

function throwCustomError() {
    throw new CustomError("Custom error");
}

try {
    console.log("Force generic error");
    console.log("Generic error try block");
    throwGenericError();
    //console.log("Generic error try block");
}
catch (err) {
    console.log("Generic error catch block");
    console.log(`Error: ${err.message}`);
}
finally {
    console.log("Generic error finally block");
}

try {
    console.log("Force custom error");
    console.log("Custom error try block");
    throwCustomError();
    //console.log("Custom error try block");
}
catch (err) {
    console.log("Custom error catch block");
    console.log(`CustomError: ${err.message}`);
}
finally {
    console.log("Custom error finally block");
}
```

<img width="655" alt="lab-07" src="https://user-images.githubusercontent.com/105889862/172033957-627d922e-fc54-4bb7-9008-6490d05d18a3.png">

