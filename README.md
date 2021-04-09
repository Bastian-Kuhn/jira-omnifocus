# jira-omnifocus

Since I Organize my tasks with OmniFocus, but at the same time I'm forced to use Jira with some Consumers, I was disappointed with the existing Solutions to sync them both.  For this reason, I created this native Plugin which has no extra requirements. Just copy the File to the OmniFocus Plugin Folder,  update user, password and jira_url and you are ready to go.

## Important
The Plugin Identifies the Tasks by the Ticket Number, which needs to be in Front of the Task Name.
But you can edit everything else behind this Number. Also, the Note, which is as default the Link to the ticket and the ticket description or move the tasks to the projects you want. If you remove the Tag, the Tasks will no longer touched by the plugin.

## What the plugin does:
 * It queries all Ticket which are Assigned to you and Open from Jira
 * Queries all Tasks with the given Tag (default Jira) from OmniFocus
 * You can set even a Filter, by Ticket ID (Regexp)
 * Create new Tasks, or reopen Tasks if they appear in Jira
 * Closes all Tasks with the given Tag which not appear in Jira

## Features
 * Stand-alone Plugin without any requirements.
 * Sync Tickets from Multiple Jira Instances into OmniFocus
 * Sync Comments of all Jira Tickets you ever had a OmniFocus Task for

## Limitations for Comment Sync
 * Comments of Tickets, you never had a task for, are not found
 * If you archive to early in OmniFocus, comments will be reopened if the Ticket is still assigned to you. Our you can't sync comments any more, of tickets which are no longer assigned to you.  Reason is, that even the completed tasks is the reference of the plugin to look for comments. 

## Changelog
### Version 1.3
 * Tickets with children are no longer closed automatically

### Version 1.2
 * Added support to query multiple JIRA Instances

### Version 1.1
 * Added Function to add Jira Comments as subtask to the task



# Thanks to:
@snwfdhmp Martin Joly:Thanks for Updating JavaScript Code with new Features and Optimizations
