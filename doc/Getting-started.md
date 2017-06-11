# Getting Started

Before you start working with [tasks](Tasks.md), make sure to perform the following actions: 

1. Enable the **Task Management** plugin. The plugin is bundled with IntelliJ IDEA and is enabled by default. If it is disabled, enable it on the [Plugins][1] ![][ext] page of the [Settings / Preferences Dialog][2] ![][ext] as described in [Enabling and Disabling Plugins][3] ![][ext].
2. [Set up integration](#its-integration) between IntelliJ IDEA and one or several issue tracking systems from the list of the [supported ones](#its-list).

Performing the following additional actions will provide you with the fully-featured tasks workflow: 

- Enable VCS integration for your project either on the [project level][4] ![][ext] or the [directory level][5] ![][ext].
- Set up the [issue navigation pattern][6] ![][ext] to connect your check-in comments with the issue tracker. This will give you the ability to quickly navigate from a specific commit in the [Version Control Tool Window][7] ![][ext] to the related issue in the browser.

##  <a name="its-integration"></a> Setting Up Integration with the Issue Tracking System
Integration between IntelliJ IDEA and an issue tracking system allows you to obtain the list of issues from your issue tracker and keep it up-to-date. 

To configure integration, do the following:

1. [Connect](#its-connect) to the issue tracking system server.
2. [Set up synchronization](#its-sync) between IntelliJ IDEA and the issue tracking system.

### <a name="its-connect"></a> To Connect to the Issue Tracking System Server
1. Open the [Servers][8] ![][ext] dialog box by doing any of the following: 
    - [Open the Settings dialog box][9] ![][ext]. Below the **Tasks** node, click **Servers**. 
    - In the [Open Task][10] dialog box, click ![settings](../img/settings.png). 
    - On the main menu, choose **Tools | Tasks & Contexts | Configure Servers**.
2. In the **Servers** dialog box, click the **Add** button and choose a server from the list of the [supported issue trackers](#its-list). The set of available options depends on the selected server type. In most cases, you need to specify at least the following: 
    - The URL address of your issue tracking server. 
    - Your account credentials specific for the selected server. 
    
    If you need to access the server via a proxy, click the **Proxy settings...** button and specify the proxy server settings in the [HTTP Proxy][11] ![][ext] dialog box.
    
    To allow access to the specified server for your team members, select the **Share URL** check box.

3. Optionally, if you want to set up the [issue navigation pattern][6] ![][ext], switch to the **Commit Message** tab, select the **Add commit message** check box and define the commit message syntax. 

4. Check whether the specified settings ensure successful connection to the server by clicking the **Test** button and click **OK** to apply your changes.

### <a name="its-sync"></a> To Set Up Synchronization between IntelliJ IDEA and the Issue Tracking System
You may choose whether you want IDEA to keep a cached list of issues and update it periodically in the background or to retrieve information on demand.

#### To set preferred synchronization method:

- [Open the Settings dialog box][9] ![][ext] and click **Tasks**. Do one of the following:
    - To synchronize the issues list in the background, select the **Enable issue cache** check box and specify the synchronization frequency and the cache size. IntelliJ IDEA will now periodically connect to the issue tracker and refresh the issues list.
    - To obtain the issues list on demand, clear the **Enable issue cache** check box. IntelliJ IDEA will now connect to the issue tracker upon your request, for example, when you start [opening a task](Tasks-opening.md).
    
        > If you are connected to a high performance issue tracker, choosing on-demand synchronization may be preferable.

## <a name="its-list"></a> Supported Issue Tracking Systems

- [Jira][12] ![][ext]
- [YouTrack][13] ![][ext]
- [Lighthouse][14] ![][ext]
- [PivotalTracker][15] ![][ext]
- [Redmine][16] ![][ext]
- [Trac][17] ![][ext]
- [FogBugz][18] ![][ext]
- [Mantis][19] ![][ext]
- [Generic server][20] ![][ext]
- [Asana][21] ![][ext]
- [Assembla][22] ![][ext]
- [Sprint.ly][23] ![][ext]
- [Trello][24] ![][ext]
- [GitLab][25] ![][ext]
- [Bugzilla][26] ![][ext]
- [GitHub][27] ![][ext]

---

🔙 [Working with Tasks and Contexts](../README.md)

[1]: https://www.jetbrains.com/help/idea/plugins-2.html
[2]: https://www.jetbrains.com/help/idea/settings-preferences-dialog.html
[3]: https://www.jetbrains.com/help/idea/enabling-and-disabling-plugins.html
[4]: https://www.jetbrains.com/help/idea/associating-a-project-root-with-a-version-control-system.html
[5]: https://www.jetbrains.com/help/idea/associating-a-directory-with-a-specific-version-control-system.html
[6]: https://www.jetbrains.com/help/idea/2017.1/handling-issues.html
[7]: https://www.jetbrains.com/help/idea/version-control-tool-window.html
[8]: https://www.jetbrains.com/help/idea/servers-2.html
[9]: https://www.jetbrains.com/help/idea/accessing-settings.html
[10]: https://www.jetbrains.com/help/idea/open-task-dialog.html
[11]: https://www.jetbrains.com/help/idea/http-proxy.html

[12]: http://www.atlassian.com/software/jira/
[13]: http://www.jetbrains.com/youtrack/
[14]: http://lighthouseapp.com/
[15]: http://www.pivotaltracker.com
[16]: http://www.redmine.org/
[17]: http://trac.edgewall.org/
[18]: http://www.fogcreek.com/fogbugz/
[19]: http://www.mantisbt.org/
[20]: https://www.jetbrains.com/help/idea/configuring-generic-task-server.html
[21]: https://asana.com
[22]: https://www.assembla.com/features/bug-tracking
[23]: http://sprint.ly/ 
[24]: https://trello.com
[25]: https://gitlab.com
[26]: https://www.bugzilla.org
[27]: http://github.com/

[ext]: ../img/ext-link.png

