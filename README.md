A linux script used to automatically sign in at a certain time

Tools:
- linux (I'm using Elementary OS)
- crontab
- xdotool


Instructions
1. install linux

2. download the file from github
    - move the crontabTest.sh file into /home/myUserName/Documents

3. make crontabTest.sh executable
    - in terminal type: chmod +x /home/myUserName/Documents/crontabTest.sh

4. install xdotool
    - in terminal type: sudo apt-get install xdotool
    - test if xdotool is working by typing: xdotool mousemove 10 10
    - (your cursor should jump to the top left corner)

5. in terminal type: crontab -e
    - watch this to learn about cron: http://www.youtube.com/watch?v=UlVqobmcPuM&t=2m0s

6. in crontab write:
    - 33 6 * * * /bin/sh /home/myUserName/Documents/crontabTest.sh
    - this will launch crontabTest.sh everyday at 6:33AM

7. Conclusion: at 6:33AM, the your cursor will move to position 10 10 (check the crontabTest.sh file), wait for 5 seconds, then click once.
