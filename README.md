Linux for Rockchip

The Rockchip support changes in this repository originally came from:

https://github.com/Galland/rk3x_kernel_3.0.36

However, since it lacked the proper kernel git history (or any history, of which
some of us are rather fond), the "Inital commit" was changed into a kernel patch
which applies cleanly onto the v3.0.36 stable kernel tag.
After that, the remaining rk3x commits from Galland's tree were forcibly am'd,
so this tree's contents should match rk3x_kernel_3.0.36's, although their
histories differ.


The idea is for this branch to be around long enough only for all of the desired
changes to be forward ported to the HOL Linux kernel.  This is the reason for
rebasing on the kernel proper instead of an Android tree.  The goal is to use
the current, limited Rockchip support in the HOL kernel to get at least the
RK292x (or at least my RK292x) working with devicetree -- and to do plenty of
clean-up.

Seriously, who uses the semi-verbage "pls" in their kernel code?
