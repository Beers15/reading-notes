[Home](README.md)
 
# Readings: Event Driven Applications
 
## Review, Research, and Discussion
 
---------------

1) Why is access control important?

  * It's an excellent security practice that ensures only individuals who meet the correct criteria can access certain resources or perform certain actions.

2) Describe an application that would need access control.

  * Almost any app with 2+ classifiable groups of users that has a need for varying levels of control over that app's actions could benefit from access control. A common example of software that uses access control is the linux filesystem. Each file on a Linux filesystem has an access control list that sets read/write/execute permissions for the owner, a user group other, or 'others' (DAC, not RBAC).

3) What is a role used for?

  * A role is used to determine if a user has permission to perform certain actions. Each role has a subset of capabilities stating what someone of that role is allowed to do. 

4) Why is role based access control more scalable than discretionary or mandatory access control? <sup>1<sup>

  * In RBAC, users are assigned roles upon creation, making it much easier to scale this kind of a system. By simply editing the ACL permissions could easily be changed compared to other types of AC as well. MAC requires 'system-enforcement' and defines permissions on a more case by case basis. DAC can require users to define permission for every single resource they own. These type of AC seem much more intensive and less automatic than RBAC does.

### Vocabulary terms

Referenced cited article below for answers<sup>1</sup>

Authorization

  * Ensuring a user has permission to perform an action that they are attempting to perform. 

Role Based Access Control

  * In this type of access control users have a role that determines what kind of actions they are able to take across an auth application.

Capabilities

  * Capabilities are the actions that are able to be taken on an auth application that has an ACL. Each role has a set of capabilities.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
  * Event driven programming

  * Event listeners, handlers, and emitters

  * The observer pattern

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

  * How to use combine OOP and EDP to create fluid programs (e.g. the gator+food example in the readings)

  * Using the event library in Node.js

  * Defining event listeners, handlers, and emitters in Node.js

3) What are you most excited about trying to implement or see how it works?
 
  * Creating event driven applications that can handle async events
 
#### Works Cited
 
<sup>1</sup> Risk, Erin, _Access Control Models: MAC, DAC, RBAC, & PAM Explained_, Twingate, Jul 29 2021, https://www.twingate.com/blog/access-control-models/
