# jira-omnifocus

Since I Organize my tasks with OmniFocus, but at the same time I'm forced to use Jira with some Consumers, I was disappointed with the existing Solutions to sync them both.  For this reason, I created this native Plugin which has no extra requirements. Just copy the File to the OmniFocus Plugin Folder,  update user, password and jira_url and you are ready to go.

## Important
The Plugin Identifies the Tasks by the Ticket Number, which needs to be in Front of the Task Name.
But you can edit everything else behind this Number. Also, the Note, which is as default the Link to the ticket and the ticket description or move the tasks to the projects you want. If you remove the Tag, the Tasks will not longer touched by the plugin.

## What the plugin does:
 * It queries all Ticket which are Assigned to you and Open from Jira
 * Queries all Tasks with the given Tag (default Jira) from OmniFocus
 * Create new Tasks, or reopen Tasks if they appear in Jira
 * Closes all Tasks with the given Tag which not appear in Jira

## Multiple Instances
You can run Multiple Instances of this script, by copying it to a new name, update the label, identifier and in any case the used_tag variable.

## Footnote
I'm a Python Programmer and to be bold, not a fan of JavaScript. This Script works of course (don't worry) is smal and clean, but not perfect. I currently need 4 loops to check all the status. This can make of course the Script a bit slower. While I know easy ways in Python to optimize that, a JavaScript Developer would be welcome to optimize this in this JavaScript Plugin.
