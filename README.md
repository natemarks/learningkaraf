# learningkaraf
common commands:
**Install:** This installs one or more bundles into the container. Passing -s to the install command instructs the container to attempt starting the bundle if possible. When a bundle is successfully installed, its bundle ID will be presented—this identifies the bundle in the running container.
**Uninstall:** This uninstalls a bundle via bundle ID (remove from container).**
Start:** This starts a bundle. If the bundle is in the resolved state, the container will call the bundles start method, otherwise the container will attempt to resolve the bundle then start if successful.
**Stop:** This stops a bundle via bundle ID (calls BundleActivator's stop method).
**Resolve:** This instructs the container to attempt to wire all required dependencies to the bundle.
**Refresh:** This refreshes a bundle's wiring; this causes the container to recalculate dependencies.
**Update:** This updates the bundle as per its updated location; bundle is reinstalled and rewired.
