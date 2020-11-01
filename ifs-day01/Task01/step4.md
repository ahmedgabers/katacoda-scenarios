Let's check how many packages are installed on the OS

`dpkg -l | wc -l`{{execute}}

`dpkg -l` lists the packages installed in our container

`wc -l` counts them

How many packages do we have on our host?

Save the output in a text file in Day01/ directory