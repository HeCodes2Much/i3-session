i3session
=========

<p align="center">
  <img src="https://img.shields.io/badge/Maintained%3F-Yes-green?style=for-the-badge">
  <img src="https://img.shields.io/github/license/The-Repo-Club/i3-session?style=for-the-badge">
  <img src="https://img.shields.io/github/issues/The-Repo-Club/i3-session?color=violet&style=for-the-badge">
  <img src="https://img.shields.io/github/stars/The-Repo-Club/i3-session?style=for-the-badge">
  <img src="https://img.shields.io/github/forks/The-Repo-Club/i3-session?color=teal&style=for-the-badge">
</p>

`i3session` remembers what's running in your i3 workspaces by saving a session file (in ~/.i3/session).
It is then able to restore the running processes (and their simple orientation) to one or more workspaces.

Since `i3session` executes i3 commands sequentially (tree traversal), changing focus during restore will affect where clients open. By default, the `i3-nagbar` will appear during restore with a message to remind you of this.

**Note: The restore command does not remove the current contents of a workspace, so you'll want to (manually) clear a workspace before restoring to it.**

Saving a session
----------------

	% i3session save
	Saving...
	Session saved to ~/.i3/session


Restoring all workspaces
------------------------

	% i3session restore
	Restoring...
	Session restored from ~/.i3/session

Dependencies
------------

* python3
* perl-anyevent-i3
* i3-py (https://github.com/ziberna/i3-py)
* i3-nagbar
* xprop
* PyXDG

## License :scroll:
This Project is licensed under the GPL-3.0 License. Check license file for more info.
