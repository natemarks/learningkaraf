# learningkaraf


common commands:


**Install:** This installs one or more bundles into the container. Passing -s to the install command instructs the container to attempt starting the bundle if possible. When a bundle is successfully installed, its bundle ID will be presented—this identifies the bundle in the running container.

**Uninstall:** This uninstalls a bundle via bundle ID (remove from container).

**Start:** This starts a bundle. If the bundle is in the resolved state, the container will call the bundles start method, otherwise the container will attempt to resolve the bundle then start if successful.

**Stop:** This stops a bundle via bundle ID (calls BundleActivator's stop method).

**Resolve:** This instructs the container to attempt to wire all required dependencies to the bundle.

**Refresh:** This refreshes a bundle's wiring; this causes the container to recalculate dependencies.

**Update:** This updates the bundle as per its updated location; bundle is reinstalled and rewired.

**List:** This displays bundles/artifacts deployed into the container and their status. Passing -t 0 will display all the installed bundles instead of just those above the default list threshold of start level 50.

**Info:** This displays system information of the Karaf instance. Versions, JVM information, thread metrics, memory usage, and host system information are provided.

**Headers:** This views the headers in the bundle's manifest file. 

**Imports:** This displays imported packages. If you specify a bundle ID, the imports of that bundle are displayed.

**Exports:** This displays exported packages. If you specify a bundle ID, the exports of that bundle are displayed.

**Start-Level:** This obtains or sets the start level of the container. By convention, levels range in Karaf from 0 to 100; in which at level 0 the OSGi framework is not launched, and at level 100 all bundles may start. In the Karaf core system, bundles have run levels below 50 and user bundles generally start at level 60.

**Bundle-Level:** This obtains or sets the start level of a particular bundle. Bundles with start levels above the current run level cannot start.

**Framework:** Select OSGi framework for the container, and optionally set OSGi core debugging. By default, Apache Karaf uses Apache Felix, however it is common to switch to Equinox.

**Show-tree:** This displays bundle wiring as a tree structure. This command allows you to observe which bundles are providing services to your bundle.

**Create-dump:** This creates a directory containing diagnostic information.

**Dynamic-import:** This enables/disables dynamic import for a given bundle.

**Watch:** This watches for an updated version of a bundle; upon a new bundle becoming available it'll update to that version.

**Print-stack-traces:** This prints the full stack trace in the console when the execution of a command throws an exception.

**Restart:** This restarts the container (reboot).

**Grep, Cat, Tail, and Pipes:** The Karaf console provides several utilities that Linux users will be familiar with, including grep for regular expression matching, cat for printing file contents to screen, tail for streaming file content to the screen, and pipes (we use the | character to denote a pipe) that feed output from one command to the input of another.

**Shutdown:** This stops the Karaf instance.
