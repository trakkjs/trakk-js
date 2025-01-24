# Trakk.js `v0.12.1`

Automatic Documentation Generation - Real-Time Code Execution Flow - Testing / Debugging - Onboarding - for Front-End Applications

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/trakk-function.png" width=600/>
</div>

<br/>
<br/>

<p align="center">
  <br/>
  <br/>
  <strong style="font-size: 18px;"><code>yarn global add trakk-js</code></strong>
  <br/>
  <br/>
  <strong style="font-size: 18px;"><code>npm install -g trakk-js</code></strong>
</p>

<br/>
<br/>

<div id="toc">
  <ul style="list-style: none;">
    <summary align="center">
      <br/>
      <h2>Automatic Documentation Generation<br/><br/>Real-Time Code Execution Flow<br/><br/>Testing / Debugging<br/><br/>Onboarding<br/><br/>for Front-End Applications</h2>
      <br/><br/>
      <a href="https://trakkjs.com">Visit trakkjs.com for more</a>
      <br/><br/>
      <a href="https://github.com/trakkjs/trakk-js/issues/new">Found a bug ?</a>
      <br/><br/>
      <a href="https://github.com/trakkjs/trakk-js/issues/new">Have a request ?</a>
      <br/><br/>
      <a href="https://trakkjs.com/contact">Want to say Hi ?</a>
    </summary>
  </ul>
</div>

<br/>
<br/>

## Watch Video
Click here: https://trakkjs.com/api/media/demo.mp4

## Contents
- [What does it do ?](#what-does-it-do-)
  - [Tracks Function Calls](#track-function-calls)
  - [Tracks Uncaught Errors](#track-uncaught-errors)
  - [Tracks Server Requests](#track-requests)
  - [Tracks User Interactions (with **Screenshots**)](#track-user-interactions)
  - [Filters through tracked events](#filter-tracked-events)
  - [Ignores unimportant events](#ignore-unimportant-events)
  - [Shows Statistics about your application's behaviour](#view-statistics)
  - [Generates Documentation Automatically](#generate-documenation-automatically)
- [Why should I use it ?](#why-should-i-use-it-)
  - [Onboarding](#onboarding)
  - [Debugging](#debugging)
  - [Testing](#testing)
  - [Automatic Documentation Generation](#documentation)
    - [See example](#generate-documenation-automatically)
- [How can I use it ?](#how-can-i-use-it-)
  - [How do I install `Trakk.js` ?](#how-do-i-install-trakkjs-)
  - [How do I load `Trakk.js` ?](#how-do-i-load-trakkjs-)
- [Will it work with my application ?](#will-it-work-with-my-application-) (Yes, it will :wink:)
- [Is it Free ?](#is-it-free-)
- [Will it change the contents of my application ?](#will-it-change-the-contents-of-my-application-)


<br/>
<br/>
<br/>

### This is your web application :


<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/intro-1.png" width=600/>
</div>

<br/>
<br/>

### This is your web application with `Trakk.js` loaded onto it :


<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/intro-2.png" width=600/>
</div>

<br/>
<br/>

## What does it do ?

`Trakk.js` is a UI panel that loads onto your application `locally`. It is a development tool meant to ease all stages of development of your application: Developing, Debugging, Testing, Documenting & Onboarding

Clicking on the `Trakk.js` toggle will open the UI Panel that will allow you to:

### Track Function Calls
`Trakk.js` tracks all function calls that are performed by your application and presents them in their order of execution, one underneath the other.
For each function call, `Trakk.js` will provide you with the following:
- Time of execution
- Order of execution
- Actual code snippet showing the line number where the function was defined
- Link to the file where that function was defined
- Looking at the function call that predeceded the current function call, will provide you with information about which function called the function you are currently looking at
- Whether it was called from within a loop* or not
- How many times it was called from within a loop* (in case it was called from within a loop*)
- The total duration of the loop*  (in case it was called from within a loop*)

<br/>
<br/>

<i><small>* a "loop" will not necessarily be a loop explicitly defined in your code, but could also be the result of anything that made that function be called repeatedly in a sequence (e.g. a user clciking on the same button repeatedly)</small></i>

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/trakk-function.png" width=600/>
</div>

<br/>
<br/>

Cliking on the link to the file where the function was defined in :

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/trakk-open-file.png" width=600/>
</div>

<br/>
<br/>

Will open up that file in a Code Viewer :

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/code-viewer.png" width=600/>
</div>

<br/>
<br/>

### Track Uncaught Errors
If your application throws unexpected errors that you are not catching, `Trakk.js` will present them to you with information about:
- the contents of the Error
- the function that threw the Error
- all the information about that function as described in the previous section

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/trakk-error.png" width=600/>
</div>

<br/>
<br/>

### Track Requests
`Trakk.js` will track all server requests performed by your application and present them to you in their order of execution with information regarding:
- Time of execution
- Order of execution
- All relevant information describing the request (type, method, url etc.)
- The server response
- Looking at the function call that predeceded the current request, will provide you with information about which function call performed the request you are currently looking at
- Whether it was called from within a loop or not
- How many times it was called from within a loop (in case it was called from within a loop)
- The total duration of the loop (in case it was called from within a loop)

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/trakk-request.png" width=600/>
</div>

<br/>
<br/>

### Track User Interactions
`Trakk.js` will track all user interactions with your application and present them to you in their order of occurence with information regarding:
- Time of execution
- **Screenshot** showing where the user action took place on the page
- All relevant information describing the event that took place

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/trakk-user.png" width=600/>
</div>

<br/>
<br/>

### Filter tracked events
The `Trakk.js` UI Panel will, by default, present you with **all** tracked events (functions, requests, uncaught errors & user interactions), one underneath the other, in their right order of occurence. But you can also **filter** through them and only view the "function" events, or just the "requests or just the "functions" and the "requests" etc..

### Ignore unimportant events
The `Trakk.js` UI Panel will, by default, track **all**  events (functions, requests, uncaught errors & user interactions) and show them in the UI. But you can choose to ignore some of them. For example, maybe there is a server request that your application keeps making, but you are not interested in it, so you want to ignore it from the `Trakk.js` UI panel and not have it show up there. You can do so by clicking on a "hide" button at the top right of that tracked event in the UI and it will never show up again until page refresh.

### View Statistics 
`Trakk.js` allows you to view statistics about your application's behaviour. `Trakk.js` tracks everything in real-time, so whenever you look at your application's statistics you are viewing all statistics up to this point. Everything in `Trakk.js` is updated constantly, in real-time. Regading Statistics, Trakk.s will provide you with information about :
- total number of function calls
- total number of requests
- total number of uncaught errors
- total number of user actions
- most frequest function call
- most frequent request
- most frequent user action
- most frequent uncaught error
- slowest function "loop"
- fastest function "loop"
- slowest request "loop"
- fastest request "loop"
- all unique function calls already performed
- all unique requests calls already performed
- all unique uncaught errors already thrown
- all unique user actions already performed
  
<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/stat-1.png" width=600/>
</div>

<br/>
<br/> 

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/stat-2.png" width=600/>
</div>

<br/>
<br/> 

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/stat-3.png" width=600/>
</div>

<br/>
<br/> 

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/stat-4.png" width=600/>
</div>

<br/>
<br/> 

### Generate Documenation Automatically 
`Trakk.js` allows you to automatically generate documenation with a click of a button

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/docs-1.png" width=600/>
</div>

<br/>
<br/>

The documentation will present the reader with all tracked events (in their right order of occurence) one underneath the other with all the information that was described in the previous sections for all possible tracked events.

The documenation will leave out all tracked events that you chose to ignore. See the [Ignore Unimportant Events](#ignore-unimportant-events) section.


The documentation comes in the form of an interactive, static & self-contained `HTML` file that will always work offline 

<div align="center">
  <img src="https://trakkjs.com/api/media/html-1.png" width=600/>
</div>

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/html-6.png" width=600/>
</div>

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/html-2.png" width=600/>
</div>

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/html-3.png" width=600/>
</div>

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/html-31.png" width=600/>
</div>

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/html-4.png" width=600/>
</div>

<br/>
<br/>

<div align="center">
  <img src="https://trakkjs.com/api/media/html-5.png" width=600/>
</div>

<br/>
<br/>

## Why should I use it ?

## Debugging

As a Front-End Application increases in size, it gets harder and harder to debug your code. It's hard to track what function is called when, where and why. Same for Server Requests, Uncaught Errors & User Actions.
Relying solely on **breakpoints** on your browser's devtools or **`debugger`** statements and **`console.log`s** in your code can become **cumbersome**.

`Trakk.js` provides you a nice, clean and very informative UI about what "event" took place, where in your code, when and why.

## Testing

You, the Developer of the application, or the Tester, wants to play around with the application and make sure that all appropriate code is executed at the right place and at the right time and for the right reasons. `Trakk.js` allows you to do that by providing you with a nice, clean and very informative UI about what "event" took place, where in your code, when and why.

## Onboarding

When a **newcomer** is asked to work on a front-end application they know nothing about, it's really hard for them to understand what code is executed when and why and where it originated from, while they are looking at the code or playing around the application as a user. 

`Trakk.js` allows newcomers to easily get onboarded on the applications they will be asked to work on, by providing them with a nice, clean and very informative UI about what "event" took place, where in the code, when and why, just by simply playing around with and testing the applicaiton in real-time.

`Trakk.js` allows you to easily and automatically generate **documentation** regarding the whole of your application's flow. What code was executed when, where and why and because of which user interaction with the page. A newcomer can go through that documentation and **study** it or use it as a **reference point** during their **onboarding**.

## Documentation

Writing documentation is not easy. Especially for large-scale applications that keep **evolving** and **changing**. It's easy to **leave things out** and it's even easier for documentation to become **outdated**.

`Trakk.js` allows you to generate documentation describing **the whole of your application flow**, the **complete code journey** combined **with all user interactions** (and **screenshots**) that took place at every point of the way. **With a click of a button**, every time your application is updated, you can then quickly generate new **accurate, up-to-date documentation** describing **in detail** everything that took place in your newly updated application flow. Because the documentation is generated automatically based on all code execution that took place, it is **imposible for it to leave things out or show outdated content**.

## How can I use it ?

### How do I install `Trakk.js` ?
`Trakk.js` only works **locally** because it is meant to **ease the development process** of the application

1. Install the latest verion of `Trakk.js` **globally** with either `yarn global add trakk-js` or `npm install -g trakk-js`
2. Make sure `Trakk.js` has been installed by running `trakkjs -v`

### How do I load `Trakk.js` ?

1. Go to your application's local root folder and set up your `trakk.config.json` as described <a href="https://trakkjs.com/docs#config" target="_blank">here</a>
2. From within your application's local rooter folder then simply run `trakkjs`. You application will then start locally with the `Trakk.js` UI Panel loaded on top of it

## Will it work with my application ?
Yes. `Trakk.js` is **`framework agnostic`**. As long as your application contains `.js`, `.jsx`, `.ts` or `.tsx` files, `Trakk.js` will track all of the code they contain.

## Is It Free ?
`Trakk.js` is currently in "test" mode, meaning that it is currently free and available for anyone to use and test by simply acquiring a Free API key from <a href="https://trakkjs.com" target="_blank">trakkjs.com</a>

## Will it change the contents of my application ?
No. `Trakk.js` doesn't affect or change any of your files or folders.


