# fake-adduser
## Warning
* This script is Work-in-progress status. 
## Usage
* Update specified passwd, shadow and group files and create user's home directory in a specified location
* There are some applications (assuming some containerized applications) which are expecting that the user's accounts and their home directories are locally created -- and you may not want to create them for the users. This is a simple script with which you can create fake- passwd, shadow, group files and user's home directories.
  ```
  sudo ./fake-adduser <username>:<password>
  OR
  sudo ./fake-adduser <username> <password>
  ```
* Required setting should be configured before using the script
  ```
  DEFAULT_GROUP=""
  PATH_BASE=""
  PATH_PASSWD="${PATH_BASE}/etc/passwd"
  PATH_SHADOW="${PATH_BASE}/etc/shadow"
  PATH_GROUP="${PATH_BASE}/etc/group"
  PATH_HOME="${PATH_BASE}/home"
  ```
