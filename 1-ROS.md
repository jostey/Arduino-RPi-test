# 1. ROS
_ROS (Robot Operating System) provee librerías y herramientas para ayudar a los desarrolladores de software a crear aplicaciones para robots. ROS provee abstracción de hardware, controladores de dispositivos, librerías, herramientas de visualización, comunicación por mensajes, administración de paquetes y más. ROS está bajo la licencia open source, BSD._ http://wiki.ros.org/es
# Instalación
A continuación vamos a instalar ROS en la *raspi* desde la terminal.

0. **Instalamos dirmngr** (necesario para añadir repositorio):

	 `$ sudo apt-get install dirmngr`
 1. **Añadimos** el **repositorio** de ROS
  
	  `$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`
  
	  `$ sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 421C365BD9FF1F717815A3895523BAEEB01FA116`

 2. **Instalamos ROS**
  
	  `$ sudo apt-get update`
	  
	  `$ sudo apt-get install -y python-rosdep python-rosinstall-generator python-wstool python-rosinstall build-essential cmake`
	  
	  `$ sudo rosdep init`
	  
	  `$ rosdep update`
	  
	  `$ rosinstall_generator desktop_full --rosdistro melodic --deps --tar > melodic-desktop-full.rosinstall`
	  
	  `$ wstool init -j8 src melodic-desktop-full.rosinstall`
	  
	  `$ rosdep install --from-paths src --ignore-src --rosdistro melodic -y`
	  
	  `$ ./src/catkin/bin/catkin_make_isolated --install -DCMAKE_BUILD_TYPE=Release` 
	  

*(incompleto)*
