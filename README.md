# techChallenge

installing and starting npm
installing relevant dependencies
create index.js that renders the App
create sessionTimeout.jsx file that deals with session timeout	 
create sessionTimeoutprompt.jsx that shows a prompt and asks if the user wants to extend the session (f.ex: after 30min it logs out the user). It can be done by using Material UI (dialog). Countdown time can be accessed by using props. that's why we import this function into setTimeout.jsx 
  inside sessionTimeout.jsx:  
check whether user is authenticated or not by using hooks. create openSession and setOpenSession, if openSession is false clear everything (countdown time) and logout.
 create another hook for time countdown and setTimeCountdown to check the time left.
create a function that handles logout, if user logged out clear countdown and openSession. create another function handles with this-> when  user clicks to extend session buttton, again countdown and OpenSession values will be cleared 
create interval function that dealy with calculating interval or countdown. if user is autheticated and session is open ->then set a countdown value or time (that shows the duration of the session) and as long as session is open it counts down until reaching 0 value. 
Import sessionTimeout function into App.jsx. App.jsx deals with returning UI, and provides values for props of sessionTimeout.jsx (whether user authenticated or logged in or out)
