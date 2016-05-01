Records movies via MythTv and copies them to your Nas. Creates directories on your Nas with the name of your recorded movie. Wakes up your Nas via etherwake and shuts it down, too.

Create a crontab entry: 

30 * * * * /var/scripts/copy_movies_to_nas.sh >> /var/scripts/log/copy_movie_to_nas.log 2>&1

Create a directory under /var
mkdir -p /var/scripts/log

Copy script to /var/scripts
Change read and write modes: chmod 755 copy_movies_to_nas.sh
