^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package optris_drivers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Forthcoming
-----------
* install targets
* fixed deps
* changelogs
* updated maintainer
* removed serial number from launchfile --> accept every serial number attached
* -- minor changes so pi80 and the new 4 SDK is supported
* adapted to irDirectSDK version 4.0.0
* adaptation to interface changes of basic driver
* adaption to Version 2.0.7 of libirimager
* commeted launch parameter (default submission is raw)
* added service parameters for modifying palette conversion
* added service to switch palette
* renamed service method
* renamed topic for setting temperature range
* added object oriented camera manager
  added service for switching temperature range
  added topic for flag state
* adapted to Version 2.0.0 of libirimager
* CMake fix for kinetic
* Merge pull request `#17 <https://github.com/LCAS/optris_drivers/issues/17>`_ from tradr-project/efficient_copy
  More efficient image buffer copy
* More efficient image buffer copy
* adapted interface to libirimager driver version 1.1.0
* Merge branch 'groovy-devel' of https://github.com/ohm-ros-pkg/optris_drivers into groovy-devel
* added missing file
* - adapted to new interface (Version 1.1.0)
  - temperature range can be changed on-the-fly
* Merge pull request `#13 <https://github.com/LCAS/optris_drivers/issues/13>`_ from sebsonf/groovy-devel
  Support for geometric calibration in compliance with image_pipeline.
* check for successful image acquisition (might reduce cpu load)
* delete temporary files
* added support for geometric calibration in compliance with image_pipeline. CameraInfoManager was added, advertising /optris/raw_image and /optris/camera_info topics as well as set_camera_info service used by the camera_calibration package. A rectified image is generated and advertised under topic /optris/image_rect_color using the image_proc node.
* fix for cfg (renamed wrong file name binary.cfg -> Threshold.cfg)
* fixed bug (occured with catkin_make install)
* adapted new version of optris drivers
* removed old optris drivers, recent versions are obtainable from the vendor's homepage
* added message generation dependencies
* Merge pull request `#12 <https://github.com/LCAS/optris_drivers/issues/12>`_ from peymmo/groovy-devel
  Add new temperature msg with header/add new internal timer publisher
* remove the duplicate publishers of internal Temperatures
* add a new custom temperature msg to includes all the internal temperatures with timestamp
* Publish the time of capture as a new topic
* Merge pull request `#10 <https://github.com/LCAS/optris_drivers/issues/10>`_ from ChrisPfiOhm/groovy-devel
  Minor changes in documentation, and clean up
* -- minor bug fix in last commit
  -- added documentation
* -- clean up of unused variables
  -- added init flag to change inversion of image
* Minor change in license header
* Merged
* -- added new node for binary generation suitable for image calibration
  -- added paramete setting in image conversion node for png compression
  -- added service for binary generation to change threshold
  -- added check for subscribers to save computation time
* Merge branch 'groovy-devel' of https://github.com/ohm-ros-pkg/optris_drivers into groovy-devel
* added current version of i386 driver
* fixed old version for basic driver on ARM and amd64
* fixed e-mail adress
* added maintainer
* removed binary driver dependent files
* added dependency check
* removed config files
* added binary driver for armhf platforms
* added binary driver for amd64 architecture
* Merge /tmp/optris_drivers into fuerte-devel
  Conflicts:
  CMakeLists.txt
* added binary driver for i386 architectures
* fixed include path
* adaptation to new optris driver interface
* Merge branch 'groovy-devel' of https://github.com/ohm-ros-pkg/optris_drivers into fuerte-devel
* Added camera config
* migration to hydro
  migration to hydro
* bugfix (crash of destructor)
* bugfix (crash of destructor)
* bugfix (crash of destructor)
* bugfix (crash of destructor)
* Merge branch 'fuerte-devel' of https://github.com/ohm-ros-pkg/optris_drivers into fuerte-devel
* bugfix for multiple camera access (multi-threaded environment)
* bugfix for multiple camera access (multi-threaded environment)
* minor change
* support for new firmware (UVC and HID interface)
* support for cameras with new firmware (HID and UVC interface)
* fix for color conversion crash
* fix for crahs of conversion node
  added frame counter interface
  improved image quality for low frame rates
* fix for crahs of conversion node
  added frame counter interface
  improved image quality for low frame rates
* 32 Bit version for fuerte
* 64 Bit version for groovy
* 64 Bit version of new optris release
* Merge branch 'groovy-devel' of https://github.com/ohm-ros-pkg/optris_drivers into groovy-devel
  Conflicts:
  package.xml
* optimization (runtime, lookup table conversion)
* added mandatory e-mail tag
* minor change
* Merge branch 'groovy_dev' of https://github.com/ipa-mig/optris_drivers into groovy-devel
* minor change (formating, spelling)
* update description
* do not export libraries
* catkinizing bugfix
* catkinizing
* adjust manifest to allow install of system dependencies through rosdep;
  integrate export flags for include directory and libraries
* bug fix bispectral technology (64-Bit)
* bugfix with bispectral technology (invalid Publisher)
* minor changes (commenting)
* bugfix2: boost termination error at shutdown
* bugfix: boost termination error at shutdown event
* added options for config files
* Merge branch 'master' of https://github.com/ohm-ros-pkg/optris_drivers
* fix for camera heating problem on 64Bit machines
* fix for camera heating problem
* added support for bispectral technology on 64-Bit platforms
* added support for bispectral technology
* added commented option for compression support
* changed data transport from sensor_msgs to image_transport
  PNG compression is now possible on low bandwidth networks
* added support for 64-Bit systems
* fixes for automatic shutter flag control
  added documentation
* Merge branch 'master' of https://github.com/ohm-ros-pkg/optris_drivers
* added missing dependency
* Merge branch 'master' of https://github.com/ohm-ros-pkg/optris_drivers
* fixed default parameter
* added features:
  - box, flag, chip temperature
  - energy and temperature mode
  - force flag trigger
* Merge pull request `#1 <https://github.com/LCAS/optris_drivers/issues/1>`_ from ipa-mig/master
  added missing dependency in manifest
* add missing dependency
* added auto flag message
  fixed some minor bugs (spelling)
* added formats definition file
* added service for de-/activating auto flag control
* fixed wrong loop rate settings
* modified namespaces: rosrun and roslaunch can be used to couple nodes
* fixed namespace inconsistency (rosrun vs roslaunch)
* changed short documentation info for ros.org
* added missing file
* cleaned dispensables
* fixed delay in image transmission from camera
* Initial commit - working version on Ubuntu 12.04 LTS 32-bit
* Initial commit
* added missing dependency
* Contributors: BuildTools, Christian Pfitzner, Christopher Hrabia, Marc Hanheide, Martin Pecka, Moghadam, Peyman (CCI, Pullenvale), Sebastian Ferch, Stefan May, amndan, ipa-mig, lucid, mayst, sm, stefanmay
