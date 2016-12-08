# vcmiserver-docker-minimal

VCMI server image without game assets or mods.

To run the server use:

`$ docker run -d  -v /root/vcmiserverdata:/mnt:ro --name=vcmi3031 --restart=always --cpu-period=50000 --cpu-quota=25000 --memory=50M --memory-swap=80M -p 3031:3030 -t -i arseniyshestakov/vcmiserver-docker-full`

Server have very low requirements and shoudn't use a lot of RAM even after dozens of months.

Your "vcmiserverdata" directory on container's host must contain "Data", "Maps", "Mods" folder as well as "modSettings.json" file.

