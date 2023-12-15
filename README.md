# crontab
execute scheduled commands

#### Install
`sudo apt install cron`

#### Edit
`crontab -e`

#### Example
```
# m h  dom mon dow   command
* * * * * python /home/ubuntu/example.py
# this executes example.py every min
```
example.py
```
import os
os.system('wall testing')
```
```
*    *    *   *    *  Command_to_execute
|    |    |    |   |       
|    |    |    |    Day of the Week ( 0 - 6 ) ( Sunday = 0 )
|    |    |    |
|    |    |    Month ( 1 - 12 )
|    |    |
|    |    Day of Month ( 1 - 31 )
|    |
|    Hour ( 0 - 23 )
|
Min ( 0 - 59 )
```
