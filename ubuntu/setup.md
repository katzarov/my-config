# Hardening

TODO there is some official ubuntu checklist/guide we can use ? https://www.reddit.com/r/Ubuntu/comments/1ap58d0/a_guide_on_hardening_ubuntu/ https://www.reddit.com/r/linuxquestions/comments/x9bbb5/hardening_ubuntu_how_to_be_safe/

## Install time

- enable lvm with encryption 

## Post install

### Ubuntu Pro

- make a free ubuntu pro account and enrolled machine for live kernel patch updates or something like so.

### Firewall

- sudo ufw default deny incoming
- sudo ufw default allow outgoing
- sudo ufw enable
- https://www.digitalocean.com/community/tutorials/how-to-set-up-a-firewall-with-ufw-on-ubuntu#step-8-checking-ufw-status-and-rules

# Other

- Firefox has tab sync across devices - can use that. https://support.mozilla.org/en-US/kb/sync#w_examples-of-sync-at-work
- check if can use apple's passwords app
- check out the keyring/chain

# What I learned:

- dont use snap for dev tools that require tight system integration, use apt
- flatpack > appimage > snap ? https://www.youtube.com/watch?v=4WuYGcs0t6I
- use snap for stuff like adobe reader
- using snap insteald of native browser - which sandbox env is used ? I learned the using a flatpak browser might be less secure.
- use xorg as i get gui glitches for some electron apps rihgt now.. There may be some global electron setting for fix with wayland...

# Audio

- PipeWire is basically the best
- not PulseAudio and not JACK

- pactl info => should not be found
- pipewire --version => should be found

## Guitar plugins

- Guitarix is best and supports NAM
- buuut this one is built around JACK..
- i already hate this whole thing... 
