#### What can I beemind with GitHub?
Gitminder goals are Do More goals that track either commits or issues closed.  You can choose whether to track all your activity, or just activity in a particular repo.

#### Can I beemind work on a private repo?
Yes, if the Beeminder application has access permissions granted, that should not be a problem.  You can check the permissions [here](https://github.com/settings/connections/applications/d6afb85e6bcd6d1cbfe7) when signed into your GitHub account.

#### Beeminder isn't adding my recent activity to my goal.
There are a few possible reasons for this:
  - Your commits are not signed with an email address tied to your GitHub account.  You can check the emails associated with your account [here](https://github.com/settings/emails).
  - Beeminder does not have permission to access the repo containing that activity.  You can check the permissions [here](https://github.com/settings/connections/applications/d6afb85e6bcd6d1cbfe7).
  - Commits are made to a non-master branch.  Beeminder only looks at activity on the master branch.  (TODO: is this still true?)
  - Your GitHub-Beeminder authorization has failed, which you can revoke & reauthorize [here](https://www.beeminder.com/settings/account#account-permissions).  
