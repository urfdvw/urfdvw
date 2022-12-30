## Projects in mind
The following projects are very long term goals.
The vision is there but the dots are not connected yet.
The possibilities are not proved yet.

### Serial virtual device
- Reason
    - Make circuitpython projects more interactive
- The audience:
    - lab, experiments, or just makers. 
    - This is going to be more like a platform than application
- The goal
    - Short-term goals
        - Virtual devices, such as buttons, slide bars, gauges, color picker, are running in the browser
            - including in and output or both
            - actually, serial plotter is one of this kind
        - Actuator code are running on the CircuitPython device
        - Communication can be done with USB serial
        - virtual device configure are on the browerser side
        - microcontroller 
    - Mid-term goals
        - Use windowed display to display the devices
            - Merge with CircuitPython Online IDE
    - Long-term/Questionable goals
        - Simple logics can be written in the devices
            - With JavaScript? or Just Python
        - Easy way to let user creat their own devices
        - Easy way to convert results to devilerables
            - such as code or display UI code
- A picture in mind
    - on the website, it is something looks like a TinkerCAD workspace
    - in the workspace, all the signals from microcontroller are on the left boader
    - all the signals to the microcontrollers are on the right
        - actually, not have to be a single device, might be multiple
    - virtual devices can be draged to the workspace,
        - each device have its in and out put
        - using lines to connect the signals
            - bool or number, or text
        - devices can be 
            - sink
                - meters
                - lights
                - displays
            - source
                - wave generator
                - pulse generator
                - botton
                - color picker
            - convertor
                - threshold
                - relay
                - p, i, d modules
                - looper
            - mixer
                - add
                - multiply
            - function block
    - Device configurations can be load and saved
    - microcontrollers need to have the same port configurations
        - name matching
    - Ideally, the browser can mimic a micropython device
        - code are generated first and then ran
        - in this way, the control code can be exported and ported to deviced directly.
            - for example, 
                - situation
                    - I have sensors to the the signals from the MCU and actuators to be the signals out of the mcu
                - test phase
                    - I can connect the block to make PID controler and test the parameters
                        - however the controller is a virtual device in the browser
                - deliver phase
                    - I can then use some mechnism to store the generated code directly in to the microcontroller.
                - if the graphycal cannot assist the developing process
                    - just don't bother with it. sink and source are good enough for interaction.
    - The browser can measure the rate of interaction
    - I am thinking more and more in Matlab/Simulink + Labview way.
        - This should help development of microcontroller systems
        - Or should help the processes that need microcontrollers. Like labs.
        - It should make things faster and easier to understand, without too much complexity.
        - It should not compete with current developing logic
            - such as try to be a new file system.

### Windowed JS framework
- Reason
    - could be a way to manage slightly larger frontend apps
- The audience: me
- Goal:
    - a framework that allows widows like a OS

### CircuitPython Online IDE based on vscode.dev
- Reason
    - vscode.dev have much better python IntelliSense, file management, and UI than my hand-crafted one
    - It looks like web-serial is supported in vscode extensions for cloud
- The audience: still Education
    - Otherwise, I am not motivated to make things online
- Goal:
    - pre-configured, aka, keep things simple
        - no installation of extension etc.
    - compatible with the whole vscode eco-system
        - users can install other extensions
        - users' experience can be transferred to other work, e.g., desktop-installed vscode.

### Github integration with CircuitPython Online IDE
- Goal:
    - Store the project with git.
        - this might be easier if vscode.dev version is done

### Hardware AHK
- Goal:
    - Use teensy 4.1 as the hardware.
        - because of the usb host Cpy Library.
    - Achieve some basic functions of Auto Hot Key.
    - Finally be part of the keyboard.

### SAMD21 Arduboy Port
- Goal:
    - Run Arduboy games on the XiaoExp
- Ref:
    - https://www.hackster.io/naveenbskumar/arduboy-extended-using-wio-terminal-28756e
