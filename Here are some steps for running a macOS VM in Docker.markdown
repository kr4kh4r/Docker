Here are some steps for running a macOS VM in Docker:
Run the command :
`docker run -it \ --device /dev/kvm \ -p 50922:10022 \ -v /tmp/.X11-unix:/tmp/.X11-unix \ -e "DISPLAY=${DISPLAY:-:0.0}" \ sickcodes/docker-osx:big-sur`

Customize the installation by extracting the disk image, adding RAM and CPU, or sharing folders from the host machine 
