Steps to demonstrate the HTTP Push Demo sample application:

 1) Open the rimpublic.property file, which is located in the MDS\Servers\MDS1\config subdirectory
    of the BlackBerry JDE installation directory.
    Ensure the "push.application.reliable.ports=100" line is NOT commented out.
 2) Launch the MDS Simulator: Execute run.bat in the MDS subdirectory of the BlackBerry JDE installation directory.
 3) In the BlackBerry JDE, open the samples.jdw workspace (located in the "samples"
    directory under the BlackBerry JDE installation directory).
 4) Press F5 to build the samples.jdw workspace and launch the BlackBerry Simulator.
 5) Launch the browser from the BlackBerry Simulator's home screen.
 6) Enter an address (e.g. www.rim.com) and retrieve the web page.
 7) Exit the browser.
 8) Launch the HTTP Push Demo from the BlackBerry Simulator's home screen.
 9) Launch the HTTP Push Demo Server by executing the run.bat file, located in the
    "samples\com\rim\samples\server\httppushdemo" directory under the BlackBerry JDE
    installation directory.
10) In the HTTP Push Demo Server window, type a message.
11) Select the "rim" or "pap" radio button.
12) Click "Send".
13) In the BlackBerry Simulator, click "Ok" in response to the received message.

The BlackBerry Simulator's screen will display the sent message.

Note: Step 1 is necessary to ensure application-level reliability for the device side
HTTP Push Demo, since it listens on port 100.

Note: Steps 5 through 7 (retrieving a web page via the MDS Simulator) are required to
ensure application level reliability of push data delivery.  Before the MDS Simulator
can properly deliver push data with application acknowledgement, it must determine
whether application level reliability is supported by the BlackBerry Simulator.  This
is accomplished by using the BlackBerry Simulator to retrieve a web page via the MDS
Simulator.
