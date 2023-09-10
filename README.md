# 🎮 Eingabemodule

## SparkFun Qwiic Joystick

Der Qwiic Joystick von SparkFun scheint viel Zeit zum Antworten via I2C zu brauchen. Während dieser Zeit wird der ganze Prozess blockiert, es muss also gewartet werden. Dieses Problem wird schlimmer, wenn mehrere Anfragen hintereinander an den Joystick gesendet werden. Bei mir hat es dazu geführt, dass die FPS von 45 bis 47 auf 32 bis 35 gefallen sind. Daher habe ich zwischen den Anfragen zu X-, Y- und Button-Zustand jeweils eine Verzögerung von 20 ms eingebaut. Somit werden die Anfragen nacheinander mit zeitlichen Abstand ausgeführt. Die FPS sind dann auf 40 bis 43 gestiegen.
