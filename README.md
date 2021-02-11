<h1 align="center"> screencast</h1>
<h4 align="center">Record screen with 'byzanz-record' and 'python-xrectsel' in gif format</h4>

### Prerequisite
- [byzanz-record](git://git.gnome.org/byzanz):
It is a simple tool to record a running X desktop to an animation suitable
for presentation in a web browser.
    - Fedora
    ```
    sudo dnf copr enable vishalvvr/byzanz
    sudo dnf install byzanz -y
    ```
    Note: Default fedora package not support `exec` argument.
    - Ubuntu
    ```
    sudo apt-get install byzanz.
    ```    

- [python-xrectsel](https://github.com/digitronik/python-xrectsel):
It is a simple cli tool to capture geometry of a rectangular screen region.
    - pip
    ```
    pip install python-xrectsel --user
    ```
    Note: You can install it with source

### Usage
```
❯ ./screencast

  Screencast
  Record screen with byzanz-record and python-xrectsel in gif format.

  Usage: screencast [command]

  Commands:
  start    Start recording
  stop	   Stop recording
  toggle   Toggling between start and stop.
           Specially used for single key binding for start and stop screencast
  *         Help
```


I'm an i3 user, I use the following binding
```
bindsym $mod+Print exec sh <path>/screencast toggle
```

#### GNOME


  - Refer the following doc to add a keyboard shortcut.
  https://docs.fedoraproject.org/en-US/quick-docs/proc_setting-key-shortcut/
