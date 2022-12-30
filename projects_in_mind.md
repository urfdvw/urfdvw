## Projects in mind
The following projects are very long term goals.
The vision is there but the dots are not connected yet.
The possibilities are not proved yet.

### CircuitPython interactives
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
        - Configuration of virtual device maybe
            - saperated on the browser
            - or done by circuitpython commands to the browser
    - Mid-term goals
        - Use windowed display to display the devices
            - Merge with CircuitPython Online IDE
    - Long-term/Questionable goals
        - Simple logics can be written in the devices
            - With JavaScript? or Just Python
        - Easy way to let user creat their own devices
        - Easy way to convert results to devilerables
            - such as code or display UI code

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
