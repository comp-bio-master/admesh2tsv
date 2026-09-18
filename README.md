# admesh2tsv.bash

Converts output from [`admesh`](https://admesh.readthedocs.io/en/latest/) into a tidy TSV

[`admesh`](https://admesh.readthedocs.io/en/latest/) is a tool that extracts data from 3D scans stored as STL files

Example usage of `admesh2tsv.bash` with provided test data set `admesh.out`:

```bash
# bash admesh2tsv.bash <admesh output file>
bash admesh2tsv.bash admesh.out

# bash admesh2tsv.bash <admesh output file> > <new tidy tsv file>
bash admesh2tsv.bash admesh.out > admesh.tsv
```

* `admesh2tsv.bash` is the script that converts from `admesh` to `tsv` format

* `admesh.out` is an example file output by `admesh` run on `stl` files of limpet shells.  Note that I clipped the "bottom" off of the limpet shell `stl` files prior to running admesh so that the surface area represents the dorsal surface area of the shell (not the ventral). The original `stl` file data is not provided, just the admesh output.

---

# LimpetShellEvolution

## Extracting data from 3D scans of limpet shells to test for fisheries-induced evolution

My lab has been studying the evolution of limpets in Hawaii.  They are a local delicacy and are under intense harvesting pressure.  We are interested in the selective pressures applied by overharvesting and how it affects the evolution of phenotypes.  

We found that shell surface area is associate with human harvesting and want to use 3d scans of the limpet shells to more precisely test of effects of harvesting on phenotype. Here are some views of a 3d scan:

![alt text](https://github.com/tamucc-comp-bio-2020/classroom_repo/blob/master/lectures/Week03_files/3Dscan_limpetShell.PNG) ![alt text](https://github.com/tamucc-comp-bio-2020/classroom_repo/blob/master/lectures/Week03_files/3Dscan_limpetShell_left.PNG) ![alt text](https://github.com/tamucc-comp-bio-2020/classroom_repo/blob/master/lectures/Week03_files/3Dscan_limpetShell_right.PNG) ![alt text](https://github.com/tamucc-comp-bio-2020/classroom_repo/blob/master/lectures/Week03_files/3Dscan_limpetShell_top.PNG) ![alt text](https://github.com/tamucc-comp-bio-2020/classroom_repo/blob/master/lectures/Week03_files/3Dscan_limpetShell_bottom.PNG)

#### [Related Publication from my Research Group](https://onlinelibrary.wiley.com/doi/abs/10.1111/jbi.13845?af=R)

