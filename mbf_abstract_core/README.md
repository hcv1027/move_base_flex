# Move Base Flex Abstract Core  {#mainpage}

The mbf_abstract_core package of Move Base Flex (MBF) contains the abstract interfaces for planning controlling and recovering. Derived packages of the mbf_abstract_nav should use derived interfaces of the mbf_abstract_core which then, for example, contain a method for initialization of the plugin, e.g. by handing over a pointer to the map representation of choice.

The plugins which are loaded by Move Base Flex (a derived package of the mbf_abstract_nav) have to implement derived interfaces of the interfaces which are defined in this package. The mbf_abstract_core::AbstractPlanner provides an interface for a planner plugin to plan global paths. The mbf_abstract_core::AbstractController provides an interface for a controller plugin to control and move a robot. The mbf_abstract_core::AbstractRecovery provides an interface for a recovery plugin to recover the robot in deadlocked situations.
