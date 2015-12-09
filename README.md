$HOME/.fonts directory

Setup conky:

Choose your Interface for TCP connections.
To see your interfeces use the command below.
Ip link show

Copy the ConkyWeather.ttf to $HOME/.fonts directory. If it's not exist
create one.
Copy the weather_conky directory to your $HOME.
Go to www.accuweather.com and search for your city. Copy the link.
Open get_weather in your favourite text editor. I recommend gEdit.
Serach the line which starts with address=
Insert the link in the adress line.Add running permission to the get_weather script. (I just modified this)
Chmod +X /weather_conky/get_weather
Execute it.
If it finished running just put the .conkyrc to your $HOME dir.
Execute Conky.
If you want make it auto start.
If you want a transparent gnome panel follow this:
Open a terminal.
Type:
su
cd /usr/share/gnome-shell/theme
gedit gnome-shell.css
Search for 'panel' (press ctrl + f )
you see soemthing like this:
#panel {
background-color: black;
font-weight: bold;
height: 1.64em;
}
now change the color to:
background-color: rgba(0,0,0,0.1);
Note: If you don't start it as super user you can't write in it.
Execute SU or run the gedit az super user with sudo.
Now log off your actual gnome session and relog to profit.

The wallpaper which is represented in the top picture is a work of Justin
Maller. Wisit his site to get one of these amazing works.

www.justinmaller.com
This conky is free to use.
- Patrik Zelena (zelena5@iit.uni-miskolc.hu)
