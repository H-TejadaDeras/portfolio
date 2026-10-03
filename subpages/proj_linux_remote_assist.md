---
layout: default
---

# Linux Remote Assistance Setup
_June-July, 2026_

I wanted to have a way to remotely assist with computer issues without having to rely on Microsoft Quick Assist which has been becoming unreliable. In addition, we were in the process of transitioning the computers to using Linux, so we also needed an implementation that would work in Linux.

This setup was created with the help of various website guides and Claude. The setup was made with security in mind as this setup allows another user to control mouse movements and keystrokes in addition to being able to see sensitive information. In terms of security features, the setup requires the user to first setup the connection by running the start-remote-assist.sh script and then input their sudo password. Afterwards, both computers have to be in the same Tailnet so the remote computer can see the host computer. After that, the remote user must input the VNC password for the host machine and input user account credentials in order to view the screen of the host machine. This setup was designed in this way so there would be many different layers of security so bad actors will have a harder time getting in.

As for why did I get this to work with X Session manager, I chose to do so it would work with Xubuntu. I like how it looks.

The other main design decision in this setup was the choice to have the user setup the connection everytime by running the setup-remote-assist.sh script. This is better than having the port always open because the user using the host computer always knows what is happening rather than having their mouse randomly start moving because someone else had accessed the setup. This also makes it so the connection is not exposed at all times in the Tailnet (another security risk).

All the setup stuff and information can be found here: [https://github.com/H-TejadaDeras/linux-remote-assist](https://github.com/H-TejadaDeras/linux-remote-assist)