README.md for SCRIPTS to get Ruby on Rails installed on your system.

So today is a good day, even though it is early morning 'New Day'.  I was able to isolate what the
problem was with the Ruby on Rails 'bundle install' command not running, actually the command would start and then hang.  I had fiddled with the Raspberry PI memory, set it to 256m instead of 64m (the default).  

Nothing worked till I came along the notes I found on this site: http://elinux.org/RPi_Ruby_on_Rails

Really great follow the steps and don't skip anything like I did...arrrg

So I thought if I had trouble maybe others were having trouble too, so I thought what could I do to fix this for me and maybe help someone else in the process.

Answer: Write a short script to run all the parts for Rails to Run on the Raspberry PI.
*Note: I am testing this on the Debian build so if you use another Linux version be aware to check the scripts prior to running, fork and pull request, fix my oops and mistypes as you find.  thanks in advance.

I am going to be writing the script then pulling a simple page, you can follow the instructions and create your own rails project reasonably quick, if you are like me and always testing to breakage...lol then you might try a few of your projects and clone down to your Raspberry PI device.

Fun, Fun, Fun - 
Roger Swanson
Charleston, SC 
@roger_swanson
http://rogerswanson.me
