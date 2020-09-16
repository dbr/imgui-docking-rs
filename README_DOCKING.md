To update:
* First update the master branch. This need to be in sync with imgui-rs master branch.
* Then branch off master.
* Then clone cimgui repo docking_inter branch, make sure imgui submodule is cloned also.
* Copy from the root, cimgui.h and cimgui.cpp into imgui-sys/thirdparty
* Copy from output/* into imgui-sys/thirdparty
* Checkout imgui-sys/thirdparty/imgui to the same commit id as is in cimgui/imgui submodule
* cd into imgui-sys-bindgen
* cargo run
* cd into imgui-sys
* cargo build - Hopefully everything builds fine :)
* Commit those changes
* Now cherry pick across the changes for docking, should be no more than 4.
