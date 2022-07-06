%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%	eQEMU: extended QEMU for audit and access control
%						2022/07/06
%						yutaka_ishikawa@nii.ac.jp
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
This is a readme file for extended QEMU.

(1) Installation
$ mkdir build
$ cd build
$ ../configure --extra-cflags=-DEQEMU \
	       --target-list="aarch64-linux-user,x86_64-linux-user"
$ make -j 4
$ pushd contrib/plugins/
$ make
$ popd
$ cd ..

