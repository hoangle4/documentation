###ERROR
> [nodemon] Internal watch failed: ENOSPC: System limit for number of file watchers reached, 
It appears that my max ports weren't configured correctly. I ran the following code and it worked...

```
echo fs.inotify.max_user_watches=582222 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```
What this command does is to increase the number of watches allowed for a single user. By the default the number can be low (8192 for example). When nodemon tries to watch large numbers of directories for changes it has to create several watches, which can surpass that limit.

You could also solve this problem by:
```
sudo sysctl fs.inotify.max_user_watches=582222 && sudo sysctl -p
```
But the way it was written first will make this change permanent.
