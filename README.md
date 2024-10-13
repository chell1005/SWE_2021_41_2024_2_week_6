# SWE_2021_41_2024_2_week_6
+ Link for Week4 Assignment: <https://github.com/chell1005/SWE_2021_41_2024_2_week_4/blob/main/2019312939_%EA%B9%80%EC%98%81%EC%8B%9C.ipynb>
+ Description of my code
This is the code to determine whether input number is happy number or not, using ipynb and colab.
```
check = set()
  k = n
  while(k>0):
    t = 0
    while(k>0):
        t = t + (k%10)* (k%10)
        k = int(k / 10)
        check.add(int(k))
```
at this code, using 'check' set, the program remembers past numbers, cause when the number is not happy, it iterates, so the 'while' code will run permanantlyy.

+Week5 Assignment Description
At Week5, we learned about docker and learned how to use it. The assignment goal was to make a container that has Linux OS, git and python3 is installed, and is bind-mounted.
```
docker exec <container_name> cat /etc/os-release
```
this command checks what container's OS is. The goal was to install Linux OS, so the result must be Linux.
```
docker exec <container_name> git --versiondocker
```
```
exec <container_name> python3 --version
```
these two commands check what git and python3's version is. the goal was to install git and python in container, so when this command works, it can be said that they are installed.
```
docker inspect --format="{{ .HostConfig.Binds }}" <container_name>
```
this command is to check if the container is bind mounted. 
