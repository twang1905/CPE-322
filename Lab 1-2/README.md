# Labs 1 and 2 - Command Line
I pledge my honor that I have abided by the Stevens Honor System.

# Assignment

### hostname
![](sc1_hostname.png)

### env
![](sc2_env1.png)

### ps
![](sc3_ps.png)

### pwd
![](sc4_pwd.png)

### git clone
![](sc5_git-clone.png)

### cd iot, ls, cd, and df
![](sc6_cd-iot.png)

### mkdir demo and cd demo
![](sc7_cat-file.png)

### nano file
![](sc7_nano-file.png)

### cat file
![](sc8_cat-file.png)

### cp, mv and rm
![](sc9_cp-mv-rm.png)

### clear
![](sc10_clear.png)

### man uname
![](sc11_man-uname.png)

### uname -a
![](sc12_uname-a.png)

### ifconfig
![](sc13_ifconfig.png)

### ping localhost
![](sc14_ping-localhost.png)

### netstat
pi@raspberrypi:~/demo $ netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  2      [ ]         DGRAM                    11909    /run/user/1000/systemd/notify
unix  4      [ ]         DGRAM                    6483     /run/systemd/notify
unix  2      [ ]         DGRAM                    9312     /run/systemd/journal/syslog
unix  17     [ ]         DGRAM                    9319     /run/systemd/journal/dev-log
unix  7      [ ]         DGRAM                    9321     /run/systemd/journal/socket
unix  2      [ ]         DGRAM                    15696    /tmp/dhcpcd-pi/libdhcpcd-wpa-746.0
unix  2      [ ]         DGRAM                    15697    /tmp/dhcpcd-pi/libdhcpcd-wpa-746.1
unix  4      [ ]         DGRAM                    9992     /var/run/wpa_supplicant/wlan0
unix  2      [ ]         DGRAM                    10007    /var/run/wpa_supplicant/p2p-dev-wlan0
unix  3      [ ]         STREAM     CONNECTED     13910    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     14328    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     11922    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     14880    
unix  3      [ ]         STREAM     CONNECTED     13553    
unix  3      [ ]         STREAM     CONNECTED     11362    
unix  3      [ ]         STREAM     CONNECTED     13492    
unix  3      [ ]         STREAM     CONNECTED     11689    
unix  3      [ ]         STREAM     CONNECTED     15325    
unix  2      [ ]         DGRAM                    9953     
unix  3      [ ]         STREAM     CONNECTED     14329    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     15620    @/dbus-vfs-daemon/socket-6aA7w8Qw
unix  3      [ ]         STREAM     CONNECTED     14960    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     11920    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     11521    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     14923    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     11700    
unix  2      [ ]         DGRAM                    9980     
unix  2      [ ]         DGRAM                    9886     
unix  3      [ ]         STREAM     CONNECTED     13494    
unix  3      [ ]         STREAM     CONNECTED     13884    
unix  3      [ ]         STREAM     CONNECTED     11650    
unix  2      [ ]         DGRAM                    10215    
unix  3      [ ]         STREAM     CONNECTED     13859    
unix  3      [ ]         STREAM     CONNECTED     11612    
unix  3      [ ]         STREAM     CONNECTED     14360    
unix  3      [ ]         STREAM     CONNECTED     13509    
unix  2      [ ]         DGRAM                    11299    
unix  3      [ ]         STREAM     CONNECTED     9879     /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     13512    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    11545    
unix  3      [ ]         STREAM     CONNECTED     15472    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     9900     /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     11607    
unix  3      [ ]         STREAM     CONNECTED     11964    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     13877    
unix  3      [ ]         STREAM     CONNECTED     9899     /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     14997    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     7166     /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    11372    
unix  3      [ ]         STREAM     CONNECTED     13923    
unix  3      [ ]         STREAM     CONNECTED     13851    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     9975     /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     9971     
unix  3      [ ]         DGRAM                    11375    
unix  3      [ ]         STREAM     CONNECTED     13917    
unix  3      [ ]         STREAM     CONNECTED     13531    
unix  3      [ ]         STREAM     CONNECTED     13850    
unix  3      [ ]         STREAM     CONNECTED     13433    
unix  3      [ ]         STREAM     CONNECTED     10222    /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     11591    
unix  3      [ ]         STREAM     CONNECTED     11530    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     10214    
unix  3      [ ]         STREAM     CONNECTED     13434    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    9997     
unix  3      [ ]         STREAM     CONNECTED     6567     /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     15540    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     15585    
unix  3      [ ]         STREAM     CONNECTED     15541    @/tmp/.X11-unix/X0
unix  2      [ ]         DGRAM                    13372    
unix  2      [ ]         DGRAM                    13366    
unix  3      [ ]         STREAM     CONNECTED     13889    
unix  3      [ ]         STREAM     CONNECTED     11701    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     13552    
unix  3      [ ]         STREAM     CONNECTED     15692    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     7131     /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     15327    
unix  3      [ ]         STREAM     CONNECTED     15471    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     14887    
unix  3      [ ]         STREAM     CONNECTED     15459    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     9841     
unix  3      [ ]         STREAM     CONNECTED     11745    
unix  3      [ ]         STREAM     CONNECTED     13953    
unix  3      [ ]         STREAM     CONNECTED     10223    /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     9970     
unix  3      [ ]         DGRAM                    11376    
unix  3      [ ]         STREAM     CONNECTED     14361    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     13530    
unix  2      [ ]         DGRAM                    11638    
unix  3      [ ]         STREAM     CONNECTED     13909    
unix  3      [ ]         STREAM     CONNECTED     15408    
unix  3      [ ]         STREAM     CONNECTED     9976     /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     12206    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     16398    /run/dhcpcd.unpriv.sock
unix  3      [ ]         STREAM     CONNECTED     15409    
unix  3      [ ]         STREAM     CONNECTED     14926    
unix  3      [ ]         STREAM     CONNECTED     13656    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     14927    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     14448    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     10062    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    12885    
unix  3      [ ]         STREAM     CONNECTED     15419    
unix  2      [ ]         DGRAM                    15422    
unix  3      [ ]         STREAM     CONNECTED     16815    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     15584    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     14964    
unix  3      [ ]         STREAM     CONNECTED     15420    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    13118    
unix  3      [ ]         STREAM     CONNECTED     13533    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     14972    
unix  3      [ ]         STREAM     CONNECTED     16399    /run/dhcpcd.unpriv.sock
unix  3      [ ]         STREAM     CONNECTED     12209    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     17608    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     17606    
unix  3      [ ]         STREAM     CONNECTED     15593    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    13126    
unix  3      [ ]         STREAM     CONNECTED     13913    /run/user/1000/pulse/native
unix  3      [ ]         DGRAM                    13237    
unix  3      [ ]         STREAM     CONNECTED     16726    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     15694    
unix  3      [ ]         STREAM     CONNECTED     15594    
unix  3      [ ]         STREAM     CONNECTED     12923    
unix  3      [ ]         STREAM     CONNECTED     15695    
unix  3      [ ]         STREAM     CONNECTED     17458    
unix  3      [ ]         STREAM     CONNECTED     14974    
unix  3      [ ]         STREAM     CONNECTED     15592    
unix  3      [ ]         STREAM     CONNECTED     12924    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     13260    
unix  3      [ ]         STREAM     CONNECTED     13907    /run/user/1000/bus
unix  2      [ ]         DGRAM                    9420     
unix  3      [ ]         DGRAM                    11911    
unix  3      [ ]         DGRAM                    11910    
unix  3      [ ]         STREAM     CONNECTED     15599    
unix  3      [ ]         DGRAM                    13238    
unix  3      [ ]         STREAM     CONNECTED     12877    
unix  3      [ ]         STREAM     CONNECTED     17607    
unix  3      [ ]         STREAM     CONNECTED     15598    
unix  3      [ ]         STREAM     CONNECTED     11914    
unix  3      [ ]         STREAM     CONNECTED     13474    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     15609    
unix  2      [ ]         DGRAM                    12853    
unix  3      [ ]         STREAM     CONNECTED     13109    
unix  3      [ ]         STREAM     CONNECTED     13172    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     10033    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     6937     
unix  3      [ ]         STREAM     CONNECTED     11899    
unix  3      [ ]         STREAM     CONNECTED     7078     
unix  3      [ ]         STREAM     CONNECTED     7004     
unix  3      [ ]         STREAM     CONNECTED     9882     /run/systemd/journal/stdout
unix  2      [ ]         STREAM     CONNECTED     12144    
unix  3      [ ]         STREAM     CONNECTED     11660    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     13365    
unix  3      [ ]         STREAM     CONNECTED     12207    /run/user/1000/bus
unix  2      [ ]         DGRAM                    11906    
unix  2      [ ]         DGRAM                    11908    
unix  2      [ ]         DGRAM                    7052     
unix  3      [ ]         DGRAM                    6484     
unix  3      [ ]         STREAM     CONNECTED     11520    
unix  2      [ ]         DGRAM                    6980     
unix  3      [ ]         STREAM     CONNECTED     6932     
unix  3      [ ]         STREAM     CONNECTED     11513    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     6985     
unix  2      [ ]         STREAM     CONNECTED     12153    
unix  3      [ ]         STREAM     CONNECTED     12155    
unix  3      [ ]         STREAM     CONNECTED     6986     
unix  3      [ ]         DGRAM                    6485     
unix  3      [ ]         STREAM     CONNECTED     13241    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     13358    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     6990     
unix  3      [ ]         STREAM     CONNECTED     13802    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     11787    
unix  3      [ ]         STREAM     CONNECTED     9974     /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     9973     /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     14873    
unix  3      [ ]         STREAM     CONNECTED     10154    
unix  3      [ ]         STREAM     CONNECTED     12284    
unix  3      [ ]         STREAM     CONNECTED     14956    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     19464    
unix  3      [ ]         STREAM     CONNECTED     12285    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     12182    
unix  3      [ ]         STREAM     CONNECTED     13641    
unix  2      [ ]         DGRAM                    12287    
unix  3      [ ]         STREAM     CONNECTED     12158    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     13642    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     15539    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     13896    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     15538    
unix  3      [ ]         STREAM     CONNECTED     12157    
unix  3      [ ]         STREAM     CONNECTED     18594    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     14959    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     13905    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     16730    
unix  3      [ ]         STREAM     CONNECTED     15560    
unix  3      [ ]         STREAM     CONNECTED     12195    
unix  3      [ ]         STREAM     CONNECTED     12256    /run/user/1000/menu-cached-:0
unix  3      [ ]         STREAM     CONNECTED     15582    
unix  3      [ ]         STREAM     CONNECTED     12188    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     19486    
unix  3      [ ]         STREAM     CONNECTED     13290    
unix  3      [ ]         STREAM     CONNECTED     11970    /run/user/1000/bus
unix  3      [ ]         DGRAM                    19482    
unix  3      [ ]         STREAM     CONNECTED     12187    
unix  3      [ ]         STREAM     CONNECTED     13607    @/tmp/.X11-unix/X0
unix  3      [ ]         STREAM     CONNECTED     14969    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    19485    
unix  3      [ ]         STREAM     CONNECTED     16731    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     13606    
unix  3      [ ]         STREAM     CONNECTED     16851    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     12203    
unix  3      [ ]         STREAM     CONNECTED     13603    
unix  3      [ ]         STREAM     CONNECTED     12255    
unix  3      [ ]         STREAM     CONNECTED     12200    
unix  3      [ ]         STREAM     CONNECTED     15364    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     14966    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     13609    
unix  2      [ ]         DGRAM                    13262    
unix  3      [ ]         STREAM     CONNECTED     13610    /run/user/1000/bus
unix  3      [ ]         DGRAM                    19484    
unix  3      [ ]         STREAM     CONNECTED     15580    
unix  2      [ ]         DGRAM                    13611    
unix  3      [ ]         STREAM     CONNECTED     14935    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     13619    
unix  3      [ ]         DGRAM                    19483    
unix  3      [ ]         STREAM     CONNECTED     15377    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     13282    
unix  2      [ ]         DGRAM                    19478    
unix  3      [ ]         STREAM     CONNECTED     13621    
unix  3      [ ]         STREAM     CONNECTED     12210    
unix  3      [ ]         STREAM     CONNECTED     10221    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     13622    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     15601    /run/dbus/system_bus_socket
