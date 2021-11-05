# XCache

Analysis Facility maintains an XCache server (managed through SLATE), with 25 x 1.5 TB NVMes and 2x25 Gbps NIC.

ServiceX uses the XCache by default.
Users can manually add the prefix `root://192.170.240.18:1094//` to their root paths, eg:

If the original path is:

    root://fax.mwt2.org:1094//pnfs/uchicago.edu/atlaslocalgroupdisk/rucio/user/mgeyik/63/c4/user.mgeyik.26617246._000006.out.root

make it:

    root://192.170.240.18:1094//root://fax.mwt2.org:1094//pnfs/uchicago.edu/atlaslocalgroupdisk/rucio/user/mgeyik/63/c4/user.mgeyik.26617246._000006.out.root

Alternatively you may use script *xcache_ls* to get the cfile containing the best paths to access all the files in their dataset.
