27.02.2018:

Hotend:

>>> M106
SENDING:M106
>>> M303 E-0 S210 C8
SENDING:M303 E-0 S210 C8
PID Autotune start
 bias: 122 d: 122 min: 206.43 max: 214.17
 bias: 120 d: 120 min: 206.43 max: 214.01
 bias: 121 d: 121 min: 206.43 max: 213.39 Ku: 44.29 Tu: 24.58
 Classic PID
 Kp: 26.57 Ki: 2.16 Kd: 81.64
>>> M303 E-0 S210 C8
SENDING:M303 E-0 S210 C8
 bias: 121 d: 121 min: 206.43 max: 213.65 Ku: 42.69 Tu: 24.41
 Classic PID
 Kp: 25.62 Ki: 2.10 Kd: 78.17
>>> M303 E-0 S210 C8
SENDING:M303 E-0 S210 C8
 bias: 121 d: 121 min: 206.43 max: 213.85 Ku: 41.49 Tu: 24.41
 Classic PID
 Kp: 24.90 Ki: 2.04 Kd: 75.97
Setting hotend temperature to 0.000000 degrees Celsius.
 bias: 121 d: 121 min: 206.43 max: 213.49 Ku: 43.64 Tu: 24.25
 Classic PID
 Kp: 26.18 Ki: 2.16 Kd: 79.36
 bias: 124 d: 124 min: 205.71 max: 213.96 Ku: 38.30 Tu: 25.56
 Classic PID
 Kp: 22.98 Ki: 1.80 Kd: 73.42
 
 restart:
 
 >>> M303 E-0 S210 C8
SENDING:M303 E-0 S210 C8
PID Autotune start
 bias: 122 d: 122 min: 206.43 max: 214.17
 bias: 120 d: 120 min: 206.43 max: 213.39
 bias: 120 d: 120 min: 206.88 max: 213.33 Ku: 47.32 Tu: 23.76
 Classic PID
 Kp: 28.39 Ki: 2.39 Kd: 84.31
 bias: 120 d: 120 min: 206.43 max: 213.44 Ku: 43.60 Tu: 24.25
 Classic PID
 Kp: 26.16 Ki: 2.16 Kd: 79.29
 bias: 120 d: 120 min: 206.43 max: 213.33 Ku: 44.26 Tu: 24.08
 Classic PID
 Kp: 26.55 Ki: 2.21 Kd: 79.94
 bias: 119 d: 119 min: 206.56 max: 214.06 Ku: 40.40 Tu: 24.58
 Classic PID
 Kp: 24.24 Ki: 1.97 Kd: 74.47
 bias: 122 d: 122 min: 206.43 max: 213.33 Ku: 44.99 Tu: 24.25
 Classic PID
 Kp: 27.00 Ki: 2.23 Kd: 81.83
 bias: 119 d: 119 min: 206.88 max: 213.54 Ku: 45.45 Tu: 23.92
 Classic PID
 Kp: 27.27 Ki: 2.28 Kd: 81.55
PID Autotune finished! Put the last Kp, Ki and Kd constants from below into Configuration.h
#define  DEFAULT_Kp 27.27
#define  DEFAULT_Ki 2.28
#define  DEFAULT_Kd 81.55

 
 
 Bed:
 
 >>> M303 E-1 S60 C8
SENDING:M303 E-1 S60 C8
PID Autotune start
 bias: 108 d: 108 min: 59.80 max: 60.17
 bias: 102 d: 102 min: 59.80 max: 60.16
 bias: 98 d: 98 min: 59.80 max: 60.16 Ku: 698.31 Tu: 14.09
 Classic PID
 Kp: 418.99 Ki: 59.47 Kd: 737.94
>>> M303 E-1 S60 C8
SENDING:M303 E-1 S60 C8
 bias: 101 d: 101 min: 59.80 max: 60.16 Ku: 719.69 Tu: 13.60
 Classic PID
 Kp: 431.81 Ki: 63.51 Kd: 734.03
 bias: 99 d: 99 min: 59.80 max: 60.16 Ku: 705.44 Tu: 14.09
 Classic PID
 Kp: 423.26 Ki: 60.08 Kd: 745.47
 bias: 101 d: 101 min: 59.80 max: 60.16 Ku: 719.69 Tu: 13.76
 Classic PID
 Kp: 431.81 Ki: 62.75 Kd: 742.88
 bias: 99 d: 99 min: 59.80 max: 60.16 Ku: 705.44 Tu: 13.11
 Classic PID
 Kp: 423.26 Ki: 64.59 Kd: 693.46
>>> M303 E-1 S60 C8
SENDING:M303 E-1 S60 C8
 bias: 101 d: 101 min: 59.80 max: 60.16 Ku: 719.69 Tu: 13.76
 Classic PID
 Kp: 431.81 Ki: 62.75 Kd: 742.83
PID Autotune finished! Put the last Kp, Ki and Kd constants from below into Configuration.h
#define  DEFAULT_bedKp 431.81
#define  DEFAULT_bedKi 62.75
#define  DEFAULT_bedKd 742.83
>>> M303 E-1 S60 C8
SENDING:M303 E-1 S60 C8
[ERROR] Can't read from printer (disconnected?) (SerialException): device reports readiness to read but returned no data (device disconnected or multiple access on port?)
Disconnected.
Connecting...
[ERROR] Could not connect to /dev/ttyUSB0 at baudrate 115200:
Serial error: [Errno 2] could not open port /dev/ttyUSB0: [Errno 2] No such file or directory: '/dev/ttyUSB0'
Connecting...
[ERROR] Could not connect to /dev/ttyUSB0 at baudrate 115200:
Serial error: [Errno 2] could not open port /dev/ttyUSB0: [Errno 2] No such file or directory: '/dev/ttyUSB0'
Connecting...
[ERROR] Could not connect to /dev/ttyUSB0 at baudrate 115200:
Serial error: [Errno 2] could not open port /dev/ttyUSB0: [Errno 2] No such file or directory: '/dev/ttyUSB0'
Connecting...
[ERROR] Saving failed for set port:'PronterWindow' object has no attribute 'rc_filename'
start
Printer is now online.
echo: External Reset
Marlin 1.1.8
echo: Last Updated: 2018-01-20 | Author: (Bob Kuhn, Anet config)
echo:Compiled: Feb 27 2018
echo: Free Memory: 12263  PlannerBufferBytes: 1232
echo:EEPROM version mismatch (EEPROM=V47 Marlin=V52)
echo:Hardcoded Default Settings Loaded
>>> M303 E-1 S60 C8
SENDING:M303 E-1 S60 C8
PID Autotune start
 bias: 105 d: 105 min: 59.80 max: 60.17
 bias: 99 d: 99 min: 59.80 max: 60.16
 bias: 99 d: 99 min: 59.80 max: 60.16 Ku: 705.44 Tu: 13.76
 Classic PID
 Kp: 423.26 Ki: 61.51 Kd: 728.17
 bias: 100 d: 100 min: 59.80 max: 60.16 Ku: 712.56 Tu: 13.93
 Classic PID
 Kp: 427.54 Ki: 61.40 Kd: 744.24
 bias: 102 d: 102 min: 59.80 max: 60.16 Ku: 726.82 Tu: 13.11
 Classic PID
 Kp: 436.09 Ki: 66.54 Kd: 714.48
 bias: 102 d: 102 min: 59.80 max: 60.16 Ku: 726.82 Tu: 13.76
 Classic PID
 Kp: 436.09 Ki: 63.37 Kd: 750.24
 bias: 98 d: 98 min: 59.80 max: 60.16 Ku: 698.31 Tu: 13.76
 Classic PID
 Kp: 418.99 Ki: 60.89 Kd: 720.76
 bias: 98 d: 98 min: 59.80 max: 60.16 Ku: 698.31 Tu: 14.09
 Classic PID
 Kp: 418.99 Ki: 59.47 Kd: 737.94
PID Autotune finished! Put the last Kp, Ki and Kd constants from below into Configuration.h
#define  DEFAULT_bedKp 418.99
#define  DEFAULT_bedKi 59.47
#define  DEFAULT_bedKd 737.94