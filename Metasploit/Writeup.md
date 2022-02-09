# Metasploit 
Go to [room](https://tryhackme.com/room/rpmetasploit)
### Learn to use Metasploit, a tool to probe and exploit vulnerabilities on networks and servers.

![](https://sathisharthars.files.wordpress.com/2014/05/metasploit1.png)

## Task 1 - Intro 

- Kali and most other security distributions of Linux include Metasploit by default. If you are using a different distribution of Linux, verify that you have it installed or install it from the Rapid 7 Github repository. 
> No answer needed

## Task 2 - Initializing...

- First things first, we need to initialize the database! Let's do that now with the command: msfdb init
If you're using the AttackBox, you don't need to do this.
> No answer needed


- Before starting Metasploit, we can view some of the advanced options we can trigger for starting the console. Check these out now by using the command: msfconsole -h
> No answer needed


- We can start the Metasploit console on the command line without showing the banner or any startup information as well. What switch do we add to msfconsole to start it without showing this information? This will include the '-'
> -q


- Once the database is initialized, go ahead and start Metasploit via the command: msfconsole
> No answer needed


- After Metasploit has started, let's go ahead and check that we've connected to the database. Do this now with the command: db_status
> No answer needed


- Cool! We've connected to the database, which type of database does Metasploit 5 use? 
> postgresql


## Task 3 - Rock 'em to the Core [Commands]

- Let's go ahead and start exploring the help menu. On the Metasploit prompt (where we'll be at after we start Metasploit using msfconsole), type the command: help
> No answer needed

- The help menu has a very short one-character alias, what is it?
> ?
 
 
- Finding various modules we have at our disposal within Metasploit is one of the most common commands we will leverage in the framework. What is the base command we use for searching?
> search


- Once we've found the module we want to leverage, what command we use to select it as the active module?
> use

 
- How about if we want to view information about either a specific module or just the active one we have selected?
> info


- Metasploit has a built-in netcat-like function where we can make a quick connection with a host simply to verify that we can 'talk' to it. What command is this?
> connect


- Entirely one of the commands purely utilized for fun, what command displays the motd/ascii art we see when we start msfconsole (without -q flag)?
> banner


- We'll revisit these next two commands shortly, however, they're two of the most used commands within Metasploit. First, what command do we use to change the value of a variable?
> set


-Metasploit supports the use of global variables, something which is incredibly useful when you're specifically focusing on a single box. What command changes the value of a variable globally? 
> setg


- Now that we've learned how to change the value of variables, how do we view them? There are technically several answers to this question, however, I'm looking for a specific three-letter command which is used to view the value of single variables.
> get


- How about changing the value of a variable to null/no value?
> unset


- When performing a penetration test it's quite common to record your screen either for further review or for providing evidence of any actions taken. This is often coupled with the collection of console output to a file as it can be incredibly useful to grep for different pieces of information output to the screen. What command can we use to set our console output to save to a file?
> spool


- Leaving a Metasploit console running isn't always convenient and it can be helpful to have all of our previously set values load when starting up Metasploit. What command can we use to store the settings/active datastores from Metasploit to a settings file? This will save within your msf4 (or msf5) directory and can be undone easily by simply removing the created settings file. 
> save
