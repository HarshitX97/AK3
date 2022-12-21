----------------------------------------------------------------------------------
AnyKernel3 - Flashable Zip Template for Kernel Releases with Ramdisk Modifications
----------------------------------------------------------------------------------
### by osm0sis @ xda-developers ###


## // Staying Up-To-Date ##

Now that you've got a ready zip for your device, you might be wondering how to keep it up-to-date with the latest AnyKernel commits. AnyKernel2 and AnyKernel3 have been painstakingly developed to allow you to just drop in the latest update-binary and tools directory and have everything "just work" for beginners not overly git or script savvy, but the best practice way is as follows:

1. Fork my AnyKernel3 repo on GitHub

2. `git clone https://github.com/<yourname>/AnyKernel3`

3. `git remote add upstream https://github.com/osm0sis/AnyKernel3`

4. `git checkout -b <devicename>`

5. Set it up like your <devicename> zip (i.e. remove any folders you don't use like ramdisk or patch, delete README.md, and add your anykernel.sh and optionally your Image.*-dtb if you want it up there) then commit all those changes

6. `git push --set-upstream origin <devicename>`

7. `git checkout master` then repeat steps 4-6 for any other devices you support

Then you should be able to `git pull upstream master` from your master branch and either merge or cherry-pick the new AK3 commits into your device branches as needed.

___For further support and usage examples please see the AnyKernel3 XDA thread:___ _https://forum.xda-developers.com/t/dev-template-anykernel3-easily-mod-rom-ramdisk-pack-image-gz-flashable-zip.2670512/_

__Have fun!__
