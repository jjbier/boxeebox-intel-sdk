# Preparations

	git clone https://github.com/quasar1/boxeebox-intel-sdk.git -b ubuntu-12.04-lts  (this branch)
	cd boxeebox-intel-sdk
	mkdir build
	cd build

# Prerequisites on Ubuntu 12.04 LTS

	sudo apt-get install golang
	update to cmake 3.2.2:
	
	wget http://www.cmake.org/files/v3.2/cmake-3.2.2.tar.gz
	tar -zxvf cmake-3.2.2.tar.gz
	cd cmake-3.2.2
	mkdir build
	cd build
	cmake .. -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/usr
	make
	sudo make install
	sudo ldconfig	

# Building

	cmake ..
	make -j8


When the build fails, try just re-running "make" a couple of times and if the error persists, you'll probably have to tweak the CMakeLists.txt file a bit to suit your system (pull requests please) and re-run `make` a few times.


lib/modules/pvrsrvkm.ko
T SGXPostActivePowerEvent				      <
T SGXTestActivePowerEvent				      <
T graphics_pm_deinit					      <
T graphics_pm_init					      <
T graphics_pm_set_busy					      <
T graphics_pm_set_idle					      <
T graphics_pm_wait_not_suspended			      <
T icepm_device_register					      <
T icepm_device_unregister				      <
T icepm_set_drv_state					      <
T icepm_set_mode					      <
U intel_ce_pm_handler_v1				      <
U os_sema_destroy					      <
U os_sema_get						      <
U os_sema_init						      <
U os_sema_put						      <
U pal_flush_chipset_cache				      <
b graphics_pm_semaphore					      <
d graphics_pm_functions					      <
d graphics_pm_state					      <
t graphics_pm_resume					      <
t graphics_pm_suspend					      <


