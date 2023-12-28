# Get-Help-in-the-Command-Line

<h2>Activity overview</h2>

As a security analyst, I won’t have all the answers all the time, but I can learn where to find them. One of the great things about Linux is that I can get help right through the command line.

In this lab activity, I’ll use the ```man``` and ```whatis``` commands to get information on other commands and how they work. I’ll also use the ```apropos``` command to search the manual page for a command with a specified string.

When working as a security analyst, I'll likely find it useful to know how to discover which command to use or information about what commands do.

<h2>Scenario</h2>

In this scenario, I have to find more information about commands that I need to use. I also need to discover which command to use to perform a certain task.

Here’s how I’ll do this task: First, I’ll explore a few commands I can use in the shell to learn more about other commands. Next, I’ll find an option I need to add to a command. Third, I’ll use a command to get a brief description of commands so I can identify their differences. Finally, I’ll identify the command I need to perform a task.

<h2>Task 1. Learn more about commands</h2>

In this task, I need to explore a few commands I can use in the shell to learn more about the functionality of other commands.

First, imagine I can’t quite remember what the ```cat``` command does and want a quick reminder.

1. Run the ```whatis``` command to get a short description of ```cat```.

![image](https://github.com/n8som/Get-Help-in-the-Command-Line/assets/110139109/ca1bada4-802d-42da-9839-ed86ead7194c)

Next, imagine that I want more details about ```cat``` and all of its options.

2. Use the man command to get more details about ```cat```.

The man command returns a general description of ```cat``` and information about each of its options:

![image](https://github.com/n8som/Get-Help-in-the-Command-Line/assets/110139109/7e929580-3569-4f27-b270-dace2a834013)

When the first page of information returned by ```man``` is displayed, the output pauses.

Note: I can output more information one line at a time by pressing the ENTER key or output the next page of the manual by pressing the space bar.

3. Press Q to exit this manual page.

Now, imagine I’ve remembered there’s a command that prints just the first part of a file, but I can’t remember the exact command. The ```apropos``` command is useful in these instances. I can use keywords with ```apropos``` to find a command.

4. Use ```apropos``` to find a command that returns the first part of a file:

```apropos -a first part file```

Note: There is no right and wrong when using apropos in terms of keywords. Think of it as a very focused search. It will only return commands that correspond to keywords I supply. Keep trying if the first returned command does not provide what I need. Also, keep in mind that using the -a option will limit results to only those commands that match all keywords supplied.

![image](https://github.com/n8som/Get-Help-in-the-Command-Line/assets/110139109/069bbfa9-b4ef-4c0e-b121-e1d8fccd70a2)

<h2>Task 2. Explore the useradd command</h2>

In this task, imagine that I want to set the expiration date for a temporary user account. I know that I need to use the ```useradd``` command for this, but I’m not quite sure how to complete the task. I realize it might involve adding an option to the command.

1. Use the most appropriate Linux command to get help on the ```useradd``` command and learn more about all of its options.

Note: I can output more information one line at a time by pressing the ENTER key or output the next page of the manual by pressing the space bar.

Using ```man useradd``` I find that ```-e``` will satisfy my need to complete the task.

![image](https://github.com/n8som/Get-Help-in-the-Command-Line/assets/110139109/e2ae4f8f-ffef-4883-8d09-2089fb67faf6)

Press Q to exit this manual page.

<h2>Task 3. Explore the rm and rmdir commands</h2>

In this task, I need to determine the difference between the ```rm``` and ```rmdir``` commands.

Imagine that I’ve used these commands before, but I can’t remember how they’re different.

- Use the most appropriate Linux command to quickly remind yourself what each command does.

Note: This task will require entering two commands, one with ```rm``` and one with ```rmdir```.

Here I see ```rmdir``` only removes empty directories.

![image](https://github.com/n8som/Get-Help-in-the-Command-Line/assets/110139109/b4e4569d-c738-4641-828b-7d32b66a8d5f)

<h2>Task 4. Determine which command to use</h2>

In this task, imagine that I need to create a new group but I can’t remember what command to use. I need to identify a command that will do this by searching for it through keywords. In this case, use the keywords ```create new group```.

- Use the most appropriate Linux command with these keywords to identify what command to use.

Here I find that ```groupadd``` is used to create a new group

![image](https://github.com/n8som/Get-Help-in-the-Command-Line/assets/110139109/850921d2-6d89-4405-a829-19d1f02bc050)

<h2>Conclusion</h2>

I now have practical experience in using basic Linux Bash shell commands to

- get a short description of a command,
- display the ```man``` pages for a command, and
- find commands based on keywords about their function.

This ability will be valuable as I navigate the Linux command line.

