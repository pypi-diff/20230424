# Comparing `tmp/mindsponge_ascend-1.0.0a0-py3-none-any.whl.zip` & `tmp/mindsponge_ascend-1.0.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,235 +1,362 @@
-Zip file size: 1482770 bytes, number of entries: 233
--rw-r--r--  2.0 unx     3409 b- defN 23-Jan-31 13:19 mindsponge/__init__.py
--rw-r--r--  2.0 unx     1102 b- defN 23-Jan-31 13:19 mindsponge/callback/__init__.py
--rw-r--r--  2.0 unx     8488 b- defN 23-Jan-31 13:19 mindsponge/callback/h5md.py
--rw-r--r--  2.0 unx     5098 b- defN 23-Jan-31 13:19 mindsponge/callback/information.py
--rw-r--r--  2.0 unx     1311 b- defN 23-Jan-31 13:19 mindsponge/cell/__init__.py
--rw-r--r--  2.0 unx     1802 b- defN 23-Jan-31 13:19 mindsponge/cell/amp.py
--rw-r--r--  2.0 unx    21428 b- defN 23-Jan-31 13:19 mindsponge/cell/basic.py
--rw-r--r--  2.0 unx    13153 b- defN 23-Jan-31 13:19 mindsponge/cell/equivariant.py
--rw-r--r--  2.0 unx     1359 b- defN 23-Jan-31 13:19 mindsponge/cell/initializer.py
--rw-r--r--  2.0 unx     1576 b- defN 23-Jan-31 13:19 mindsponge/cell/mask.py
--rw-r--r--  2.0 unx    17862 b- defN 23-Jan-31 13:19 mindsponge/cell/msa.py
--rw-r--r--  2.0 unx     6984 b- defN 23-Jan-31 13:19 mindsponge/cell/transition.py
--rw-r--r--  2.0 unx    28740 b- defN 23-Jan-31 13:19 mindsponge/cell/triangle.py
--rw-r--r--  2.0 unx     1596 b- defN 23-Jan-31 13:19 mindsponge/colvar/__init__.py
--rw-r--r--  2.0 unx     7045 b- defN 23-Jan-31 13:19 mindsponge/colvar/atoms.py
--rw-r--r--  2.0 unx     5040 b- defN 23-Jan-31 13:19 mindsponge/colvar/base.py
--rw-r--r--  2.0 unx     4979 b- defN 23-Jan-31 13:19 mindsponge/colvar/bonded.py
--rw-r--r--  2.0 unx     3995 b- defN 23-Jan-31 13:19 mindsponge/colvar/colvar.py
--rw-r--r--  2.0 unx     7262 b- defN 23-Jan-31 13:19 mindsponge/colvar/index.py
--rw-r--r--  2.0 unx     1956 b- defN 23-Jan-31 13:19 mindsponge/colvar/position.py
--rw-r--r--  2.0 unx     2400 b- defN 23-Jan-31 13:19 mindsponge/common/__init__.py
--rw-r--r--  2.0 unx     1482 b- defN 23-Jan-31 13:19 mindsponge/common/config_load.py
--rw-r--r--  2.0 unx    56524 b- defN 23-Jan-31 13:19 mindsponge/common/geometry.py
--rw-r--r--  2.0 unx     8163 b- defN 23-Jan-31 13:19 mindsponge/common/protein.py
--rw-r--r--  2.0 unx    36743 b- defN 23-Jan-31 13:19 mindsponge/common/residue_constants.py
--rw-r--r--  2.0 unx    15746 b- defN 23-Jan-31 13:19 mindsponge/common/stereo_chemical_props.txt
--rw-r--r--  2.0 unx    38732 b- defN 23-Jan-31 13:19 mindsponge/common/utils.py
--rw-r--r--  2.0 unx     1480 b- defN 23-Jan-31 13:19 mindsponge/control/__init__.py
--rw-r--r--  2.0 unx     9658 b- defN 23-Jan-31 13:19 mindsponge/control/controller.py
--rw-r--r--  2.0 unx     1122 b- defN 23-Jan-31 13:19 mindsponge/control/barostat/__init__.py
--rw-r--r--  2.0 unx     7299 b- defN 23-Jan-31 13:19 mindsponge/control/barostat/barostat.py
--rw-r--r--  2.0 unx     4807 b- defN 23-Jan-31 13:19 mindsponge/control/barostat/berendsen.py
--rw-r--r--  2.0 unx     1102 b- defN 23-Jan-31 13:19 mindsponge/control/constraint/__init__.py
--rw-r--r--  2.0 unx     5928 b- defN 23-Jan-31 13:19 mindsponge/control/constraint/constraint.py
--rw-r--r--  2.0 unx     7351 b- defN 23-Jan-31 13:19 mindsponge/control/constraint/lincs.py
--rw-r--r--  2.0 unx     1226 b- defN 23-Jan-31 13:19 mindsponge/control/integrator/__init__.py
--rw-r--r--  2.0 unx     5203 b- defN 23-Jan-31 13:19 mindsponge/control/integrator/brownian.py
--rw-r--r--  2.0 unx     9473 b- defN 23-Jan-31 13:19 mindsponge/control/integrator/integrator.py
--rw-r--r--  2.0 unx     4830 b- defN 23-Jan-31 13:19 mindsponge/control/integrator/leapfrog.py
--rw-r--r--  2.0 unx     5899 b- defN 23-Jan-31 13:19 mindsponge/control/integrator/velocityverlet.py
--rw-r--r--  2.0 unx     1177 b- defN 23-Jan-31 13:19 mindsponge/control/thermostat/__init__.py
--rw-r--r--  2.0 unx     4306 b- defN 23-Jan-31 13:19 mindsponge/control/thermostat/berendsen.py
--rw-r--r--  2.0 unx     4983 b- defN 23-Jan-31 13:19 mindsponge/control/thermostat/langevin.py
--rw-r--r--  2.0 unx     6156 b- defN 23-Jan-31 13:19 mindsponge/control/thermostat/thermostat.py
--rw-r--r--  2.0 unx     1266 b- defN 23-Jan-31 13:19 mindsponge/core/__init__.py
--rw-r--r--  2.0 unx    21327 b- defN 23-Jan-31 13:19 mindsponge/core/sponge.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jan-31 13:19 mindsponge/core/analysis/__init__.py
--rw-r--r--  2.0 unx     3478 b- defN 23-Jan-31 13:19 mindsponge/core/analysis/analyse.py
--rw-r--r--  2.0 unx     1126 b- defN 23-Jan-31 13:19 mindsponge/core/simulation/__init__.py
--rw-r--r--  2.0 unx     5335 b- defN 23-Jan-31 13:19 mindsponge/core/simulation/run.py
--rw-r--r--  2.0 unx     9185 b- defN 23-Jan-31 13:19 mindsponge/core/simulation/simulation.py
--rw-r--r--  2.0 unx     1175 b- defN 23-Jan-31 13:19 mindsponge/core/wrapper/__init__.py
--rw-r--r--  2.0 unx     2581 b- defN 23-Jan-31 13:19 mindsponge/core/wrapper/its.py
--rw-r--r--  2.0 unx     2585 b- defN 23-Jan-31 13:19 mindsponge/core/wrapper/remd.py
--rw-r--r--  2.0 unx     2814 b- defN 23-Jan-31 13:19 mindsponge/core/wrapper/summation.py
--rw-r--r--  2.0 unx     4056 b- defN 23-Jan-31 13:19 mindsponge/core/wrapper/wrapper.py
--rw-r--r--  2.0 unx     2415 b- defN 23-Jan-31 13:19 mindsponge/data/__init__.py
--rw-r--r--  2.0 unx     4851 b- defN 23-Jan-31 13:19 mindsponge/data/data.py
--rw-r--r--  2.0 unx    38541 b- defN 23-Jan-31 13:19 mindsponge/data/data_transform.py
--rw-r--r--  2.0 unx     7340 b- defN 23-Jan-31 13:19 mindsponge/data/elements.py
--rw-r--r--  2.0 unx    10266 b- defN 23-Jan-31 13:19 mindsponge/data/hyperparam.py
--rw-r--r--  2.0 unx    29655 b- defN 23-Jan-31 13:19 mindsponge/data/parameters.py
--rw-r--r--  2.0 unx     1122 b- defN 23-Jan-31 13:19 mindsponge/data/export/__init__.py
--rw-r--r--  2.0 unx    19169 b- defN 23-Jan-31 13:19 mindsponge/data/export/h5md.py
--rw-r--r--  2.0 unx     1916 b- defN 23-Jan-31 13:19 mindsponge/data/export/xyz.py
--rw-r--r--  2.0 unx     1090 b- defN 23-Jan-31 13:19 mindsponge/data/forcefield/__init__.py
--rw-r--r--  2.0 unx    67680 b- defN 23-Jan-31 13:19 mindsponge/data/forcefield/amber.ff14sb.yaml
--rw-r--r--  2.0 unx     2898 b- defN 23-Jan-31 13:19 mindsponge/data/forcefield/forcefield.py
--rw-r--r--  2.0 unx      626 b- defN 23-Jan-31 13:19 mindsponge/data/forcefield/spce.yaml
--rw-r--r--  2.0 unx      634 b- defN 23-Jan-31 13:19 mindsponge/data/forcefield/tip3p.yaml
--rw-r--r--  2.0 unx     1153 b- defN 23-Jan-31 13:19 mindsponge/data/template/__init__.py
--rw-r--r--  2.0 unx    33103 b- defN 23-Jan-31 13:19 mindsponge/data/template/protein0.yaml
--rw-r--r--  2.0 unx     4913 b- defN 23-Jan-31 13:19 mindsponge/data/template/template.py
--rw-r--r--  2.0 unx      275 b- defN 23-Jan-31 13:19 mindsponge/data/template/water.spce.yaml
--rw-r--r--  2.0 unx      233 b- defN 23-Jan-31 13:19 mindsponge/data/template/water.tip3p.yaml
--rw-r--r--  2.0 unx      214 b- defN 23-Jan-31 13:19 mindsponge/data/template/water_3p.yaml
--rw-r--r--  2.0 unx     1206 b- defN 23-Jan-31 13:19 mindsponge/function/__init__.py
--rw-r--r--  2.0 unx    34376 b- defN 23-Jan-31 13:19 mindsponge/function/functions.py
--rw-r--r--  2.0 unx    16410 b- defN 23-Jan-31 13:19 mindsponge/function/operations.py
--rw-r--r--  2.0 unx    27361 b- defN 23-Jan-31 13:19 mindsponge/function/units.py
--rw-r--r--  2.0 unx     1897 b- defN 23-Jan-31 13:19 mindsponge/metrics/__init__.py
--rw-r--r--  2.0 unx    13857 b- defN 23-Jan-31 13:19 mindsponge/metrics/metrics.py
--rw-r--r--  2.0 unx    65602 b- defN 23-Jan-31 13:19 mindsponge/metrics/structure_violations.py
--rw-r--r--  2.0 unx      777 b- defN 23-Jan-31 13:19 mindsponge/ops/__init__.py
--rw-r--r--  2.0 unx      782 b- defN 23-Jan-31 13:19 mindsponge/ops/cpu/__init__.py
--rw-r--r--  2.0 unx     3667 b- defN 23-Jan-31 13:19 mindsponge/ops/cpu/neighborlistop.py
--rw-r--r--  2.0 unx      782 b- defN 23-Jan-31 13:19 mindsponge/ops/gpu/__init__.py
--rw-r--r--  2.0 unx     3713 b- defN 23-Jan-31 13:19 mindsponge/ops/gpu/neighborlistop.py
--rw-r--r--  2.0 unx     1174 b- defN 23-Jan-31 13:19 mindsponge/optimizer/__init__.py
--rw-r--r--  2.0 unx     5486 b- defN 23-Jan-31 13:19 mindsponge/optimizer/dynamics.py
--rw-r--r--  2.0 unx     1708 b- defN 23-Jan-31 13:19 mindsponge/optimizer/steepest.py
--rw-r--r--  2.0 unx    13428 b- defN 23-Jan-31 13:19 mindsponge/optimizer/updater.py
--rw-r--r--  2.0 unx     1270 b- defN 23-Jan-31 13:19 mindsponge/partition/__init__.py
--rw-r--r--  2.0 unx     9658 b- defN 23-Jan-31 13:19 mindsponge/partition/distance.py
--rw-r--r--  2.0 unx     4510 b- defN 23-Jan-31 13:19 mindsponge/partition/fullconnect.py
--rw-r--r--  2.0 unx    20680 b- defN 23-Jan-31 13:19 mindsponge/partition/grids.py
--rw-r--r--  2.0 unx    10264 b- defN 23-Jan-31 13:19 mindsponge/partition/neighbourlist.py
--rw-r--r--  2.0 unx     1264 b- defN 23-Jan-31 13:19 mindsponge/potential/__init__.py
--rw-r--r--  2.0 unx    17764 b- defN 23-Jan-31 13:19 mindsponge/potential/forcefield.py
--rw-r--r--  2.0 unx     7584 b- defN 23-Jan-31 13:19 mindsponge/potential/potential.py
--rw-r--r--  2.0 unx     1173 b- defN 23-Jan-31 13:19 mindsponge/potential/bias/__init__.py
--rw-r--r--  2.0 unx     5040 b- defN 23-Jan-31 13:19 mindsponge/potential/bias/bias.py
--rw-r--r--  2.0 unx     2327 b- defN 23-Jan-31 13:19 mindsponge/potential/bias/oscillator.py
--rw-r--r--  2.0 unx     5315 b- defN 23-Jan-31 13:19 mindsponge/potential/bias/spherical.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/__init__.py
--rw-r--r--  2.0 unx     7748 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/angle.py
--rw-r--r--  2.0 unx     7846 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/bond.py
--rw-r--r--  2.0 unx    24365 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/coulomb.py
--rw-r--r--  2.0 unx     8547 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/dihedral.py
--rw-r--r--  2.0 unx    10491 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/energy.py
--rw-r--r--  2.0 unx     9504 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/lj.py
--rw-r--r--  2.0 unx    13593 b- defN 23-Jan-31 13:19 mindsponge/potential/energy/pairs.py
--rw-r--r--  2.0 unx     1152 b- defN 23-Jan-31 13:19 mindsponge/system/__init__.py
--rw-r--r--  2.0 unx     1279 b- defN 23-Jan-31 13:19 mindsponge/system/modeling/__init__.py
--rw-r--r--  2.0 unx     4823 b- defN 23-Jan-31 13:19 mindsponge/system/modeling/add_missing_atoms.py
--rw-r--r--  2.0 unx    32590 b- defN 23-Jan-31 13:19 mindsponge/system/modeling/hadder.py
--rw-r--r--  2.0 unx     2632 b- defN 23-Jan-31 13:19 mindsponge/system/modeling/pdb_generator.py
--rw-r--r--  2.0 unx    18163 b- defN 23-Jan-31 13:19 mindsponge/system/modeling/pdb_parser.py
--rw-r--r--  2.0 unx     1103 b- defN 23-Jan-31 13:19 mindsponge/system/molecule/__init__.py
--rw-r--r--  2.0 unx    32010 b- defN 23-Jan-31 13:19 mindsponge/system/molecule/molecule.py
--rw-r--r--  2.0 unx     5075 b- defN 23-Jan-31 13:19 mindsponge/system/molecule/protein.py
--rw-r--r--  2.0 unx     1101 b- defN 23-Jan-31 13:19 mindsponge/system/residue/__init__.py
--rw-r--r--  2.0 unx     1936 b- defN 23-Jan-31 13:19 mindsponge/system/residue/amino.py
--rw-r--r--  2.0 unx    26953 b- defN 23-Jan-31 13:19 mindsponge/system/residue/residue.py
--rw-r--r--  2.0 unx     7364 b- defN 23-Jan-31 13:19 mindsponge/toolkits/__init__.py
--rw-r--r--  2.0 unx    10372 b- defN 23-Jan-31 13:19 mindsponge/toolkits/__main__.py
--rw-r--r--  2.0 unx    26521 b- defN 23-Jan-31 13:19 mindsponge/toolkits/build.py
--rw-r--r--  2.0 unx    43825 b- defN 23-Jan-31 13:19 mindsponge/toolkits/load.py
--rw-r--r--  2.0 unx    33777 b- defN 23-Jan-31 13:19 mindsponge/toolkits/process.py
--rw-r--r--  2.0 unx     1229 b- defN 23-Jan-31 13:19 mindsponge/toolkits/analysis/__init__.py
--rw-r--r--  2.0 unx    13854 b- defN 23-Jan-31 13:19 mindsponge/toolkits/analysis/md_analysis.py
--rw-r--r--  2.0 unx    31182 b- defN 23-Jan-31 13:19 mindsponge/toolkits/assign/__init__.py
--rw-r--r--  2.0 unx    13682 b- defN 23-Jan-31 13:19 mindsponge/toolkits/assign/resp.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/__init__.py
--rw-r--r--  2.0 unx    48238 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/DNA.mol2
--rw-r--r--  2.0 unx    10962 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/OL15.frcmod
--rw-r--r--  2.0 unx    48836 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/RNA.mol2
--rw-r--r--  2.0 unx     2419 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/__init__.py
--rw-r--r--  2.0 unx     3899 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/atomic_ions.mol2
--rw-r--r--  2.0 unx     1795 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/bsc1.py
--rw-r--r--  2.0 unx    24570 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ff14SB.frcmod
--rw-r--r--  2.0 unx   128338 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ff14SB.mol2
--rw-r--r--  2.0 unx     3842 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ff14sb.py
--rw-r--r--  2.0 unx   137234 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ff19SB.frcmod
--rw-r--r--  2.0 unx   128338 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ff19SB.mol2
--rw-r--r--  2.0 unx     4049 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ff19sb.py
--rw-r--r--  2.0 unx   497800 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/gaff.dat
--rw-r--r--  2.0 unx    34098 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/gaff.py
--rw-r--r--  2.0 unx   536359 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/gaff2.dat
--rw-r--r--  2.0 unx     1523 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ions1lm_126_spce.frcmod
--rw-r--r--  2.0 unx     1523 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ions1lm_126_tip3p.frcmod
--rw-r--r--  2.0 unx     1568 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ions1lm_126_tip4pew.frcmod
--rw-r--r--  2.0 unx     4949 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ions234lm_126_spce.frcmod
--rw-r--r--  2.0 unx     4949 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ions234lm_126_tip3p.frcmod
--rw-r--r--  2.0 unx     5096 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ions234lm_126_tip4pew.frcmod
--rw-r--r--  2.0 unx      948 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ionsjc_spce.frcmod
--rw-r--r--  2.0 unx      946 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ionsjc_tip3p.frcmod
--rw-r--r--  2.0 unx      949 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ionsjc_tip4pew.frcmod
--rw-r--r--  2.0 unx    25672 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/lipid14.dat
--rw-r--r--  2.0 unx    53829 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/lipid14.mol2
--rw-r--r--  2.0 unx     2205 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/lipid14.py
--rw-r--r--  2.0 unx    36564 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/lipid17.dat
--rw-r--r--  2.0 unx   100128 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/lipid17.mol2
--rw-r--r--  2.0 unx     2424 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/lipid17.py
--rw-r--r--  2.0 unx     1987 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ol15.py
--rw-r--r--  2.0 unx     1926 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/ol3.py
--rw-r--r--  2.0 unx      551 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/opc.mol2
--rw-r--r--  2.0 unx     2755 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/opc.py
--rw-r--r--  2.0 unx    59507 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/parm10.dat
--rw-r--r--  2.0 unx    65714 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/parm19.dat
--rw-r--r--  2.0 unx     5979 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/parmbsc1.frcmod
--rw-r--r--  2.0 unx      477 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/spce.mol2
--rw-r--r--  2.0 unx     2466 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/spce.py
--rw-r--r--  2.0 unx      477 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/tip3p.mol2
--rw-r--r--  2.0 unx     2497 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/tip3p.py
--rw-r--r--  2.0 unx      551 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/tip4pew.mol2
--rw-r--r--  2.0 unx     2783 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/tip4pew.py
--rw-r--r--  2.0 unx    65808 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/GLYCAM_06j.dat
--rw-r--r--  2.0 unx     1451 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/__init__.py
--rw-r--r--  2.0 unx   226197 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/d_furanose.mol2
--rw-r--r--  2.0 unx     1972 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/d_furanose.py
--rw-r--r--  2.0 unx  1045201 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/d_pyranose.mol2
--rw-r--r--  2.0 unx     2311 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/d_pyranose.py
--rw-r--r--  2.0 unx    15635 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/glycoprotein.mol2
--rw-r--r--  2.0 unx     1749 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/glycoprotein.py
--rw-r--r--  2.0 unx   226197 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/l_furanose.mol2
--rw-r--r--  2.0 unx     1980 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/l_furanose.py
--rw-r--r--  2.0 unx  1045201 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/l_pyranose.mol2
--rw-r--r--  2.0 unx     2319 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/l_pyranose.py
--rw-r--r--  2.0 unx      822 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/amber/glycam_06j/terminal.mol2
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/__init__.py
--rw-r--r--  2.0 unx     2760 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/angle_base.py
--rw-r--r--  2.0 unx     2234 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/atom_cmap_base.py
--rw-r--r--  2.0 unx     2633 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/bond_base.py
--rw-r--r--  2.0 unx     1435 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/charge_base.py
--rw-r--r--  2.0 unx     6265 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/dihedral_base.py
--rw-r--r--  2.0 unx     3730 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/exclude_base.py
--rw-r--r--  2.0 unx     2821 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/improper_base.py
--rw-r--r--  2.0 unx     7788 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/lj_base.py
--rw-r--r--  2.0 unx      897 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/mass_base.py
--rw-r--r--  2.0 unx     3758 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/nb14_base.py
--rw-r--r--  2.0 unx     5239 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/nb14_extra_base.py
--rw-r--r--  2.0 unx     2160 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/residue_cmap_base.py
--rw-r--r--  2.0 unx     1274 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/soft_bond_base.py
--rw-r--r--  2.0 unx     1911 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/ub_angle_base.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/base/virtual_atom_base.py
--rw-r--r--  2.0 unx     1837 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/__init__.py
--rw-r--r--  2.0 unx      301 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/atomic_ions.mol2
--rw-r--r--  2.0 unx    38297 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/cmap.itp
--rw-r--r--  2.0 unx    71114 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/ffbonded.itp
--rw-r--r--  2.0 unx   134978 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/ffnonbonded.itp
--rw-r--r--  2.0 unx      768 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/forcefield.itp
--rw-r--r--  2.0 unx   126888 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/protein.mol2
--rw-r--r--  2.0 unx     3821 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/protein.py
--rw-r--r--  2.0 unx      477 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/tip3p.mol2
--rw-r--r--  2.0 unx     1271 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/tip3p.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/charmm27/tips3p.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/special/__init__.py
--rw-r--r--  2.0 unx    29126 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/special/fep.py
--rw-r--r--  2.0 unx     3848 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/special/gb.py
--rw-r--r--  2.0 unx     2316 b- defN 23-Jan-31 13:19 mindsponge/toolkits/forcefield/special/min.py
--rw-r--r--  2.0 unx    84266 b- defN 23-Jan-31 13:19 mindsponge/toolkits/helper/__init__.py
--rw-r--r--  2.0 unx     5470 b- defN 23-Jan-31 13:19 mindsponge/toolkits/helper/math.py
--rw-r--r--  2.0 unx     7015 b- defN 23-Jan-31 13:19 mindsponge/toolkits/helper/namespace.py
--rw-r--r--  2.0 unx     3516 b- defN 23-Jan-31 13:19 mindsponge/toolkits/helper/rdkit.py
--rw-r--r--  2.0 unx        9 b- defN 23-Jan-31 13:19 mindsponge/toolkits/mdrun/BIN_PATH.dat
--rw-r--r--  2.0 unx     1420 b- defN 23-Jan-31 13:19 mindsponge/toolkits/mdrun/__init__.py
--rw-r--r--  2.0 unx      183 b- defN 23-Jan-31 13:19 mindsponge/toolkits/mdrun/__main__.py
--rw-r--r--  2.0 unx    25249 b- defN 23-Jan-31 13:19 mindsponge/toolkits/tools/__init__.py
--rw-r--r--  2.0 unx      777 b- defN 23-Jan-31 13:19 mindsponge_ascend-1.0.0a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-31 13:19 mindsponge_ascend-1.0.0a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jan-31 13:19 mindsponge_ascend-1.0.0a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    22787 b- defN 23-Jan-31 13:19 mindsponge_ascend-1.0.0a0.dist-info/RECORD
-233 files, 6595092 bytes uncompressed, 1446006 bytes compressed:  78.1%
+Zip file size: 1740488 bytes, number of entries: 360
+-rw-r--r--  2.0 unx     3440 b- defN 23-Apr-04 12:21 mindsponge/__init__.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Apr-04 12:21 mindsponge/callback/__init__.py
+-rw-r--r--  2.0 unx     8488 b- defN 23-Apr-04 12:21 mindsponge/callback/h5md.py
+-rw-r--r--  2.0 unx     5098 b- defN 23-Apr-04 12:21 mindsponge/callback/information.py
+-rw-r--r--  2.0 unx     1311 b- defN 23-Apr-04 12:21 mindsponge/cell/__init__.py
+-rw-r--r--  2.0 unx     1802 b- defN 23-Apr-04 12:21 mindsponge/cell/amp.py
+-rw-r--r--  2.0 unx    21428 b- defN 23-Apr-04 12:21 mindsponge/cell/basic.py
+-rw-r--r--  2.0 unx    13131 b- defN 23-Apr-04 12:21 mindsponge/cell/equivariant.py
+-rw-r--r--  2.0 unx     1359 b- defN 23-Apr-04 12:21 mindsponge/cell/initializer.py
+-rw-r--r--  2.0 unx     1907 b- defN 23-Apr-04 12:21 mindsponge/cell/mask.py
+-rw-r--r--  2.0 unx    17731 b- defN 23-Apr-04 12:21 mindsponge/cell/msa.py
+-rw-r--r--  2.0 unx     7001 b- defN 23-Apr-04 12:21 mindsponge/cell/transition.py
+-rw-r--r--  2.0 unx    28584 b- defN 23-Apr-04 12:21 mindsponge/cell/triangle.py
+-rw-r--r--  2.0 unx     1596 b- defN 23-Apr-04 12:21 mindsponge/colvar/__init__.py
+-rw-r--r--  2.0 unx     7045 b- defN 23-Apr-04 12:21 mindsponge/colvar/atoms.py
+-rw-r--r--  2.0 unx     5040 b- defN 23-Apr-04 12:21 mindsponge/colvar/base.py
+-rw-r--r--  2.0 unx     4979 b- defN 23-Apr-04 12:21 mindsponge/colvar/bonded.py
+-rw-r--r--  2.0 unx     3995 b- defN 23-Apr-04 12:21 mindsponge/colvar/colvar.py
+-rw-r--r--  2.0 unx     7262 b- defN 23-Apr-04 12:21 mindsponge/colvar/index.py
+-rw-r--r--  2.0 unx     1956 b- defN 23-Apr-04 12:21 mindsponge/colvar/position.py
+-rw-r--r--  2.0 unx     2400 b- defN 23-Apr-04 12:21 mindsponge/common/__init__.py
+-rw-r--r--  2.0 unx     1482 b- defN 23-Apr-04 12:21 mindsponge/common/config_load.py
+-rw-r--r--  2.0 unx    57115 b- defN 23-Apr-04 12:21 mindsponge/common/geometry.py
+-rw-r--r--  2.0 unx    13663 b- defN 23-Apr-04 12:21 mindsponge/common/protein.py
+-rw-r--r--  2.0 unx    36743 b- defN 23-Apr-04 12:21 mindsponge/common/residue_constants.py
+-rw-r--r--  2.0 unx    15746 b- defN 23-Apr-04 12:21 mindsponge/common/stereo_chemical_props.txt
+-rw-r--r--  2.0 unx    38794 b- defN 23-Apr-04 12:21 mindsponge/common/utils.py
+-rw-r--r--  2.0 unx     1480 b- defN 23-Apr-04 12:21 mindsponge/control/__init__.py
+-rw-r--r--  2.0 unx     9658 b- defN 23-Apr-04 12:21 mindsponge/control/controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 23-Apr-04 12:21 mindsponge/control/barostat/__init__.py
+-rw-r--r--  2.0 unx     7299 b- defN 23-Apr-04 12:21 mindsponge/control/barostat/barostat.py
+-rw-r--r--  2.0 unx     4807 b- defN 23-Apr-04 12:21 mindsponge/control/barostat/berendsen.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Apr-04 12:21 mindsponge/control/constraint/__init__.py
+-rw-r--r--  2.0 unx     5928 b- defN 23-Apr-04 12:21 mindsponge/control/constraint/constraint.py
+-rw-r--r--  2.0 unx     7351 b- defN 23-Apr-04 12:21 mindsponge/control/constraint/lincs.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Apr-04 12:21 mindsponge/control/integrator/__init__.py
+-rw-r--r--  2.0 unx     5203 b- defN 23-Apr-04 12:21 mindsponge/control/integrator/brownian.py
+-rw-r--r--  2.0 unx     9473 b- defN 23-Apr-04 12:21 mindsponge/control/integrator/integrator.py
+-rw-r--r--  2.0 unx     4830 b- defN 23-Apr-04 12:21 mindsponge/control/integrator/leapfrog.py
+-rw-r--r--  2.0 unx     5899 b- defN 23-Apr-04 12:21 mindsponge/control/integrator/velocityverlet.py
+-rw-r--r--  2.0 unx     1177 b- defN 23-Apr-04 12:21 mindsponge/control/thermostat/__init__.py
+-rw-r--r--  2.0 unx     4306 b- defN 23-Apr-04 12:21 mindsponge/control/thermostat/berendsen.py
+-rw-r--r--  2.0 unx     4983 b- defN 23-Apr-04 12:21 mindsponge/control/thermostat/langevin.py
+-rw-r--r--  2.0 unx     6156 b- defN 23-Apr-04 12:21 mindsponge/control/thermostat/thermostat.py
+-rw-r--r--  2.0 unx     1266 b- defN 23-Apr-04 12:21 mindsponge/core/__init__.py
+-rw-r--r--  2.0 unx    21327 b- defN 23-Apr-04 12:21 mindsponge/core/sponge.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-04 12:21 mindsponge/core/analysis/__init__.py
+-rw-r--r--  2.0 unx     3478 b- defN 23-Apr-04 12:21 mindsponge/core/analysis/analyse.py
+-rw-r--r--  2.0 unx     1126 b- defN 23-Apr-04 12:21 mindsponge/core/simulation/__init__.py
+-rw-r--r--  2.0 unx     5335 b- defN 23-Apr-04 12:21 mindsponge/core/simulation/run.py
+-rw-r--r--  2.0 unx     9185 b- defN 23-Apr-04 12:21 mindsponge/core/simulation/simulation.py
+-rw-r--r--  2.0 unx     1175 b- defN 23-Apr-04 12:21 mindsponge/core/wrapper/__init__.py
+-rw-r--r--  2.0 unx     2581 b- defN 23-Apr-04 12:21 mindsponge/core/wrapper/its.py
+-rw-r--r--  2.0 unx     2585 b- defN 23-Apr-04 12:21 mindsponge/core/wrapper/remd.py
+-rw-r--r--  2.0 unx     2814 b- defN 23-Apr-04 12:21 mindsponge/core/wrapper/summation.py
+-rw-r--r--  2.0 unx     4056 b- defN 23-Apr-04 12:21 mindsponge/core/wrapper/wrapper.py
+-rw-r--r--  2.0 unx     2415 b- defN 23-Apr-04 12:21 mindsponge/data/__init__.py
+-rw-r--r--  2.0 unx     4851 b- defN 23-Apr-04 12:21 mindsponge/data/data.py
+-rw-r--r--  2.0 unx    49337 b- defN 23-Apr-04 12:21 mindsponge/data/data_transform.py
+-rw-r--r--  2.0 unx     7340 b- defN 23-Apr-04 12:21 mindsponge/data/elements.py
+-rw-r--r--  2.0 unx    10266 b- defN 23-Apr-04 12:21 mindsponge/data/hyperparam.py
+-rw-r--r--  2.0 unx    29655 b- defN 23-Apr-04 12:21 mindsponge/data/parameters.py
+-rw-r--r--  2.0 unx     1122 b- defN 23-Apr-04 12:21 mindsponge/data/export/__init__.py
+-rw-r--r--  2.0 unx    19169 b- defN 23-Apr-04 12:21 mindsponge/data/export/h5md.py
+-rw-r--r--  2.0 unx     1916 b- defN 23-Apr-04 12:21 mindsponge/data/export/xyz.py
+-rw-r--r--  2.0 unx     1090 b- defN 23-Apr-04 12:21 mindsponge/data/forcefield/__init__.py
+-rw-r--r--  2.0 unx    67680 b- defN 23-Apr-04 12:21 mindsponge/data/forcefield/amber.ff14sb.yaml
+-rw-r--r--  2.0 unx     2898 b- defN 23-Apr-04 12:21 mindsponge/data/forcefield/forcefield.py
+-rw-r--r--  2.0 unx      626 b- defN 23-Apr-04 12:21 mindsponge/data/forcefield/spce.yaml
+-rw-r--r--  2.0 unx      634 b- defN 23-Apr-04 12:21 mindsponge/data/forcefield/tip3p.yaml
+-rw-r--r--  2.0 unx     1153 b- defN 23-Apr-04 12:21 mindsponge/data/template/__init__.py
+-rw-r--r--  2.0 unx    33103 b- defN 23-Apr-04 12:21 mindsponge/data/template/protein0.yaml
+-rw-r--r--  2.0 unx     4913 b- defN 23-Apr-04 12:21 mindsponge/data/template/template.py
+-rw-r--r--  2.0 unx      275 b- defN 23-Apr-04 12:21 mindsponge/data/template/water.spce.yaml
+-rw-r--r--  2.0 unx      233 b- defN 23-Apr-04 12:21 mindsponge/data/template/water.tip3p.yaml
+-rw-r--r--  2.0 unx      214 b- defN 23-Apr-04 12:21 mindsponge/data/template/water_3p.yaml
+-rw-r--r--  2.0 unx     1206 b- defN 23-Apr-04 12:21 mindsponge/function/__init__.py
+-rw-r--r--  2.0 unx    31510 b- defN 23-Apr-04 12:21 mindsponge/function/functions.py
+-rw-r--r--  2.0 unx    16410 b- defN 23-Apr-04 12:21 mindsponge/function/operations.py
+-rw-r--r--  2.0 unx    27361 b- defN 23-Apr-04 12:21 mindsponge/function/units.py
+-rw-r--r--  2.0 unx     1897 b- defN 23-Apr-04 12:21 mindsponge/metrics/__init__.py
+-rw-r--r--  2.0 unx    13857 b- defN 23-Apr-04 12:21 mindsponge/metrics/metrics.py
+-rw-r--r--  2.0 unx    66124 b- defN 23-Apr-04 12:21 mindsponge/metrics/structure_violations.py
+-rw-r--r--  2.0 unx      777 b- defN 23-Apr-04 12:21 mindsponge/ops/__init__.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-04 12:21 mindsponge/ops/cpu/__init__.py
+-rw-r--r--  2.0 unx     3667 b- defN 23-Apr-04 12:21 mindsponge/ops/cpu/neighborlistop.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-04 12:21 mindsponge/ops/gpu/__init__.py
+-rw-r--r--  2.0 unx     3713 b- defN 23-Apr-04 12:21 mindsponge/ops/gpu/neighborlistop.py
+-rw-r--r--  2.0 unx     1174 b- defN 23-Apr-04 12:21 mindsponge/optimizer/__init__.py
+-rw-r--r--  2.0 unx     5486 b- defN 23-Apr-04 12:21 mindsponge/optimizer/dynamics.py
+-rw-r--r--  2.0 unx     1708 b- defN 23-Apr-04 12:21 mindsponge/optimizer/steepest.py
+-rw-r--r--  2.0 unx    13428 b- defN 23-Apr-04 12:21 mindsponge/optimizer/updater.py
+-rw-r--r--  2.0 unx     1270 b- defN 23-Apr-04 12:21 mindsponge/partition/__init__.py
+-rw-r--r--  2.0 unx     9658 b- defN 23-Apr-04 12:21 mindsponge/partition/distance.py
+-rw-r--r--  2.0 unx     4510 b- defN 23-Apr-04 12:21 mindsponge/partition/fullconnect.py
+-rw-r--r--  2.0 unx    20680 b- defN 23-Apr-04 12:21 mindsponge/partition/grids.py
+-rw-r--r--  2.0 unx    10264 b- defN 23-Apr-04 12:21 mindsponge/partition/neighbourlist.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-Apr-04 12:21 mindsponge/pipeline/__init__.py
+-rw-r--r--  2.0 unx     3765 b- defN 23-Apr-04 12:21 mindsponge/pipeline/pipeline.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/__init__.py
+-rw-r--r--  2.0 unx     1802 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/amp.py
+-rw-r--r--  2.0 unx    21438 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/basic.py
+-rw-r--r--  2.0 unx    13149 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/equivariant.py
+-rw-r--r--  2.0 unx     1359 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/initializer.py
+-rw-r--r--  2.0 unx     1576 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/mask.py
+-rw-r--r--  2.0 unx    17860 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/msa.py
+-rw-r--r--  2.0 unx     6985 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/transition.py
+-rw-r--r--  2.0 unx    28743 b- defN 23-Apr-04 12:21 mindsponge/pipeline/cell/triangle.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-Apr-04 12:21 mindsponge/pipeline/dataset/__init__.py
+-rw-r--r--  2.0 unx     1612 b- defN 23-Apr-04 12:21 mindsponge/pipeline/dataset/dataset.py
+-rw-r--r--  2.0 unx     1043 b- defN 23-Apr-04 12:21 mindsponge/pipeline/dataset/pdbbind/__init__.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-Apr-04 12:21 mindsponge/pipeline/dataset/pdbbind/pdbbind.py
+-rw-r--r--  2.0 unx     1005 b- defN 23-Apr-04 12:21 mindsponge/pipeline/dataset/psp/__init__.py
+-rw-r--r--  2.0 unx     5588 b- defN 23-Apr-04 12:21 mindsponge/pipeline/dataset/psp/psp.py
+-rw-r--r--  2.0 unx     1395 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/__init__.py
+-rw-r--r--  2.0 unx     3368 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/model.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/__init__.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/colabdesign.py
+-rw-r--r--  2.0 unx     1129 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/colabdesign_configuratuin.py
+-rw-r--r--  2.0 unx     4552 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/colabdesign_data.py
+-rw-r--r--  2.0 unx     4073 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/colabdesign_dataset.py
+-rw-r--r--  2.0 unx     6473 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/nn_arch.py
+-rw-r--r--  2.0 unx      987 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/module/__init__.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/module/design_wrapcell.py
+-rw-r--r--  2.0 unx    16790 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/module/loss_design.py
+-rw-r--r--  2.0 unx     2735 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/colabdesign/module/utils.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/deepdr/__init__.py
+-rw-r--r--  2.0 unx     6299 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/deepdr/deepdr.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/deepdr/deepdr_configuration.py
+-rw-r--r--  2.0 unx     2573 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/deepdr/deepdr_data.py
+-rw-r--r--  2.0 unx     6547 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/deepdr/deepdr_dataset.py
+-rw-r--r--  2.0 unx     6205 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/deepdr/mda_nn_arch.py
+-rw-r--r--  2.0 unx     5073 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/deepdr/vae_nn_arch.py
+-rw-r--r--  2.0 unx     1125 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/graphdta/__init__.py
+-rw-r--r--  2.0 unx     7260 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/graphdta/data_process.py
+-rw-r--r--  2.0 unx     5205 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/graphdta/get_train_data.py
+-rw-r--r--  2.0 unx     3537 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/graphdta/graphdta.py
+-rw-r--r--  2.0 unx      886 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/graphdta/graphdta_configuration.py
+-rw-r--r--  2.0 unx     5869 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/graphdta/graphdta_dataset.py
+-rw-r--r--  2.0 unx     3751 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/graphdta/nn_arch.py
+-rw-r--r--  2.0 unx     1222 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/__init__.py
+-rw-r--r--  2.0 unx     1663 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/build_vocab.py
+-rw-r--r--  2.0 unx    13018 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/grover.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/grover_configuration.py
+-rw-r--r--  2.0 unx     9236 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/grover_dataset.py
+-rw-r--r--  2.0 unx    21245 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/nn_arch.py
+-rw-r--r--  2.0 unx     4147 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/save_features.py
+-rw-r--r--  2.0 unx     2288 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/split_data.py
+-rw-r--r--  2.0 unx      667 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/__init__.py
+-rw-r--r--  2.0 unx      667 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/data/__init__.py
+-rw-r--r--  2.0 unx     6508 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/data/mindsporevocab.py
+-rw-r--r--  2.0 unx     7806 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/data/molfeaturegenerator.py
+-rw-r--r--  2.0 unx    15835 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/data/molgraph.py
+-rw-r--r--  2.0 unx     3739 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/data/scaler.py
+-rw-r--r--  2.0 unx     2924 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/data/task_labels.py
+-rw-r--r--  2.0 unx     5988 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/data/transforms.py
+-rw-r--r--  2.0 unx      667 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/model/__init__.py
+-rw-r--r--  2.0 unx    35970 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/model/layers.py
+-rw-r--r--  2.0 unx      667 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/model_utils/__init__.py
+-rw-r--r--  2.0 unx     1030 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/model_utils/local_adapter.py
+-rw-r--r--  2.0 unx      667 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/util/__init__.py
+-rw-r--r--  2.0 unx     2874 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/util/logger.py
+-rw-r--r--  2.0 unx     5305 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/util/nn_utils.py
+-rw-r--r--  2.0 unx     2026 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/util/scheduler.py
+-rw-r--r--  2.0 unx     9373 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/grover/src/util/utils.py
+-rw-r--r--  2.0 unx     1123 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/kgnn/__init__.py
+-rw-r--r--  2.0 unx     4174 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/kgnn/kgnn.py
+-rw-r--r--  2.0 unx     1141 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/kgnn/kgnn_configuration.py
+-rw-r--r--  2.0 unx     5304 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/kgnn/kgnn_data.py
+-rw-r--r--  2.0 unx     6576 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/kgnn/kgnn_dataset.py
+-rw-r--r--  2.0 unx     1441 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/kgnn/loss.py
+-rw-r--r--  2.0 unx    13354 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/kgnn/nn_arch.py
+-rw-r--r--  2.0 unx      901 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaassessment/__init__.py
+-rw-r--r--  2.0 unx     1888 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaassessment/megaassessment_configuration.py
+-rw-r--r--  2.0 unx     8946 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaassessment/megassessment.py
+-rw-r--r--  2.0 unx     3997 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaassessment/megassessment_dataset.py
+-rw-r--r--  2.0 unx    21147 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaassessment/nn_arch.py
+-rw-r--r--  2.0 unx      821 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaevogen/__init__.py
+-rw-r--r--  2.0 unx     3066 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaevogen/evogen.py
+-rw-r--r--  2.0 unx    31237 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaevogen/evogen_block.py
+-rw-r--r--  2.0 unx      843 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaevogen/evogen_configuration.py
+-rw-r--r--  2.0 unx    12328 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaevogen/evogen_datafunction.py
+-rw-r--r--  2.0 unx     7332 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaevogen/evogen_dataprocess.py
+-rw-r--r--  2.0 unx    13290 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megaevogen/nn_arch.py
+-rw-r--r--  2.0 unx     1126 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/__init__.py
+-rw-r--r--  2.0 unx     9832 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/megafold.py
+-rw-r--r--  2.0 unx     2394 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/megafold_configuration.py
+-rw-r--r--  2.0 unx    35015 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/megafold_data.py
+-rw-r--r--  2.0 unx    12638 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/megafold_dataset.py
+-rw-r--r--  2.0 unx     3059 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/megafold_feature.py
+-rw-r--r--  2.0 unx    18000 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/nn_arch.py
+-rw-r--r--  2.0 unx      985 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/__init__.py
+-rw-r--r--  2.0 unx     8492 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/evoformer.py
+-rw-r--r--  2.0 unx     9404 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/fold_wrapcell.py
+-rw-r--r--  2.0 unx     9932 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/head.py
+-rw-r--r--  2.0 unx    18261 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/loss_module.py
+-rw-r--r--  2.0 unx     1629 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/lr.py
+-rw-r--r--  2.0 unx    13265 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/structure.py
+-rw-r--r--  2.0 unx    13127 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/megafold/module/template_embedding.py
+-rw-r--r--  2.0 unx     1125 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/__init__.py
+-rw-r--r--  2.0 unx     5136 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/multimer.py
+-rw-r--r--  2.0 unx     1795 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/multimer_configuration.py
+-rw-r--r--  2.0 unx    13011 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/multimer_data.py
+-rw-r--r--  2.0 unx     4742 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/multimer_dataset.py
+-rw-r--r--  2.0 unx     1982 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/multimer_feature.py
+-rw-r--r--  2.0 unx    17064 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/nn_arch.py
+-rw-r--r--  2.0 unx      987 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/module/__init__.py
+-rw-r--r--  2.0 unx    14511 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/module/multimer_block.py
+-rw-r--r--  2.0 unx     6548 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/module/multimer_evoformer.py
+-rw-r--r--  2.0 unx     2542 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/module/multimer_head.py
+-rw-r--r--  2.0 unx    13361 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/module/multimer_structure.py
+-rw-r--r--  2.0 unx    12664 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/multimer/module/multimer_template_embedding.py
+-rw-r--r--  2.0 unx      889 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/pafnucy/__init__.py
+-rw-r--r--  2.0 unx     7285 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/pafnucy/nn_arch.py
+-rw-r--r--  2.0 unx     4676 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/pafnucy/pafnucy.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/pafnucy/pafnucy_configuration.py
+-rw-r--r--  2.0 unx    27942 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/pafnucy/pafnucy_data.py
+-rw-r--r--  2.0 unx     8583 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/pafnucy/pafnucy_dataset.py
+-rw-r--r--  2.0 unx     1130 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/ufold/__init__.py
+-rw-r--r--  2.0 unx     4750 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/ufold/nn_arch.py
+-rw-r--r--  2.0 unx     5466 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/ufold/ufold.py
+-rw-r--r--  2.0 unx     1145 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/ufold/ufold_configuration.py
+-rw-r--r--  2.0 unx     9739 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/ufold/ufold_data.py
+-rw-r--r--  2.0 unx     6892 b- defN 23-Apr-04 12:21 mindsponge/pipeline/models/ufold/ufold_dataset.py
+-rw-r--r--  2.0 unx     1264 b- defN 23-Apr-04 12:21 mindsponge/potential/__init__.py
+-rw-r--r--  2.0 unx    17764 b- defN 23-Apr-04 12:21 mindsponge/potential/forcefield.py
+-rw-r--r--  2.0 unx     7584 b- defN 23-Apr-04 12:21 mindsponge/potential/potential.py
+-rw-r--r--  2.0 unx     1173 b- defN 23-Apr-04 12:21 mindsponge/potential/bias/__init__.py
+-rw-r--r--  2.0 unx     5040 b- defN 23-Apr-04 12:21 mindsponge/potential/bias/bias.py
+-rw-r--r--  2.0 unx     2327 b- defN 23-Apr-04 12:21 mindsponge/potential/bias/oscillator.py
+-rw-r--r--  2.0 unx     5315 b- defN 23-Apr-04 12:21 mindsponge/potential/bias/spherical.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/__init__.py
+-rw-r--r--  2.0 unx     7748 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/angle.py
+-rw-r--r--  2.0 unx     7846 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/bond.py
+-rw-r--r--  2.0 unx    24365 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/coulomb.py
+-rw-r--r--  2.0 unx     8547 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/dihedral.py
+-rw-r--r--  2.0 unx    10491 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/energy.py
+-rw-r--r--  2.0 unx     9504 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/lj.py
+-rw-r--r--  2.0 unx    13593 b- defN 23-Apr-04 12:21 mindsponge/potential/energy/pairs.py
+-rw-r--r--  2.0 unx     1152 b- defN 23-Apr-04 12:21 mindsponge/system/__init__.py
+-rw-r--r--  2.0 unx     1279 b- defN 23-Apr-04 12:21 mindsponge/system/modeling/__init__.py
+-rw-r--r--  2.0 unx     4823 b- defN 23-Apr-04 12:21 mindsponge/system/modeling/add_missing_atoms.py
+-rw-r--r--  2.0 unx    32590 b- defN 23-Apr-04 12:21 mindsponge/system/modeling/hadder.py
+-rw-r--r--  2.0 unx     2632 b- defN 23-Apr-04 12:21 mindsponge/system/modeling/pdb_generator.py
+-rw-r--r--  2.0 unx    18163 b- defN 23-Apr-04 12:21 mindsponge/system/modeling/pdb_parser.py
+-rw-r--r--  2.0 unx     1103 b- defN 23-Apr-04 12:21 mindsponge/system/molecule/__init__.py
+-rw-r--r--  2.0 unx    32010 b- defN 23-Apr-04 12:21 mindsponge/system/molecule/molecule.py
+-rw-r--r--  2.0 unx     5075 b- defN 23-Apr-04 12:21 mindsponge/system/molecule/protein.py
+-rw-r--r--  2.0 unx     1101 b- defN 23-Apr-04 12:21 mindsponge/system/residue/__init__.py
+-rw-r--r--  2.0 unx     1936 b- defN 23-Apr-04 12:21 mindsponge/system/residue/amino.py
+-rw-r--r--  2.0 unx    26953 b- defN 23-Apr-04 12:21 mindsponge/system/residue/residue.py
+-rw-r--r--  2.0 unx     7364 b- defN 23-Apr-04 12:21 mindsponge/toolkits/__init__.py
+-rw-r--r--  2.0 unx    10372 b- defN 23-Apr-04 12:21 mindsponge/toolkits/__main__.py
+-rw-r--r--  2.0 unx    26521 b- defN 23-Apr-04 12:21 mindsponge/toolkits/build.py
+-rw-r--r--  2.0 unx    43825 b- defN 23-Apr-04 12:21 mindsponge/toolkits/load.py
+-rw-r--r--  2.0 unx    33777 b- defN 23-Apr-04 12:21 mindsponge/toolkits/process.py
+-rw-r--r--  2.0 unx     1229 b- defN 23-Apr-04 12:21 mindsponge/toolkits/analysis/__init__.py
+-rw-r--r--  2.0 unx    13854 b- defN 23-Apr-04 12:21 mindsponge/toolkits/analysis/md_analysis.py
+-rw-r--r--  2.0 unx    31182 b- defN 23-Apr-04 12:21 mindsponge/toolkits/assign/__init__.py
+-rw-r--r--  2.0 unx    13682 b- defN 23-Apr-04 12:21 mindsponge/toolkits/assign/resp.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/__init__.py
+-rw-r--r--  2.0 unx    48238 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/DNA.mol2
+-rw-r--r--  2.0 unx    10962 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/OL15.frcmod
+-rw-r--r--  2.0 unx    48836 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/RNA.mol2
+-rw-r--r--  2.0 unx     2419 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/__init__.py
+-rw-r--r--  2.0 unx     3899 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/atomic_ions.mol2
+-rw-r--r--  2.0 unx     1795 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/bsc1.py
+-rw-r--r--  2.0 unx    24570 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ff14SB.frcmod
+-rw-r--r--  2.0 unx   128338 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ff14SB.mol2
+-rw-r--r--  2.0 unx     3842 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ff14sb.py
+-rw-r--r--  2.0 unx   137234 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ff19SB.frcmod
+-rw-r--r--  2.0 unx   128338 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ff19SB.mol2
+-rw-r--r--  2.0 unx     4049 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ff19sb.py
+-rw-r--r--  2.0 unx   497800 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/gaff.dat
+-rw-r--r--  2.0 unx    34098 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/gaff.py
+-rw-r--r--  2.0 unx   536359 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/gaff2.dat
+-rw-r--r--  2.0 unx     1523 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ions1lm_126_spce.frcmod
+-rw-r--r--  2.0 unx     1523 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ions1lm_126_tip3p.frcmod
+-rw-r--r--  2.0 unx     1568 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ions1lm_126_tip4pew.frcmod
+-rw-r--r--  2.0 unx     4949 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ions234lm_126_spce.frcmod
+-rw-r--r--  2.0 unx     4949 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ions234lm_126_tip3p.frcmod
+-rw-r--r--  2.0 unx     5096 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ions234lm_126_tip4pew.frcmod
+-rw-r--r--  2.0 unx      948 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ionsjc_spce.frcmod
+-rw-r--r--  2.0 unx      946 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ionsjc_tip3p.frcmod
+-rw-r--r--  2.0 unx      949 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ionsjc_tip4pew.frcmod
+-rw-r--r--  2.0 unx    25672 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/lipid14.dat
+-rw-r--r--  2.0 unx    53829 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/lipid14.mol2
+-rw-r--r--  2.0 unx     2205 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/lipid14.py
+-rw-r--r--  2.0 unx    36564 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/lipid17.dat
+-rw-r--r--  2.0 unx   100128 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/lipid17.mol2
+-rw-r--r--  2.0 unx     2424 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/lipid17.py
+-rw-r--r--  2.0 unx     1987 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ol15.py
+-rw-r--r--  2.0 unx     1926 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/ol3.py
+-rw-r--r--  2.0 unx      551 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/opc.mol2
+-rw-r--r--  2.0 unx     2755 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/opc.py
+-rw-r--r--  2.0 unx    59507 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/parm10.dat
+-rw-r--r--  2.0 unx    65714 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/parm19.dat
+-rw-r--r--  2.0 unx     5979 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/parmbsc1.frcmod
+-rw-r--r--  2.0 unx      477 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/spce.mol2
+-rw-r--r--  2.0 unx     2466 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/spce.py
+-rw-r--r--  2.0 unx      477 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/tip3p.mol2
+-rw-r--r--  2.0 unx     2497 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/tip3p.py
+-rw-r--r--  2.0 unx      551 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/tip4pew.mol2
+-rw-r--r--  2.0 unx     2783 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/tip4pew.py
+-rw-r--r--  2.0 unx    65808 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/GLYCAM_06j.dat
+-rw-r--r--  2.0 unx     1451 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/__init__.py
+-rw-r--r--  2.0 unx   226197 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/d_furanose.mol2
+-rw-r--r--  2.0 unx     1972 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/d_furanose.py
+-rw-r--r--  2.0 unx  1045201 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/d_pyranose.mol2
+-rw-r--r--  2.0 unx     2311 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/d_pyranose.py
+-rw-r--r--  2.0 unx    15635 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/glycoprotein.mol2
+-rw-r--r--  2.0 unx     1749 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/glycoprotein.py
+-rw-r--r--  2.0 unx   226197 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/l_furanose.mol2
+-rw-r--r--  2.0 unx     1980 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/l_furanose.py
+-rw-r--r--  2.0 unx  1045201 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/l_pyranose.mol2
+-rw-r--r--  2.0 unx     2319 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/l_pyranose.py
+-rw-r--r--  2.0 unx      822 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/amber/glycam_06j/terminal.mol2
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/__init__.py
+-rw-r--r--  2.0 unx     2760 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/angle_base.py
+-rw-r--r--  2.0 unx     2234 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/atom_cmap_base.py
+-rw-r--r--  2.0 unx     2633 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/bond_base.py
+-rw-r--r--  2.0 unx     1435 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/charge_base.py
+-rw-r--r--  2.0 unx     6265 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/dihedral_base.py
+-rw-r--r--  2.0 unx     3730 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/exclude_base.py
+-rw-r--r--  2.0 unx     2821 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/improper_base.py
+-rw-r--r--  2.0 unx     7788 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/lj_base.py
+-rw-r--r--  2.0 unx      897 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/mass_base.py
+-rw-r--r--  2.0 unx     3758 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/nb14_base.py
+-rw-r--r--  2.0 unx     5239 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/nb14_extra_base.py
+-rw-r--r--  2.0 unx     2160 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/residue_cmap_base.py
+-rw-r--r--  2.0 unx     1274 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/soft_bond_base.py
+-rw-r--r--  2.0 unx     1911 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/ub_angle_base.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/base/virtual_atom_base.py
+-rw-r--r--  2.0 unx     1837 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/__init__.py
+-rw-r--r--  2.0 unx      301 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/atomic_ions.mol2
+-rw-r--r--  2.0 unx    38297 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/cmap.itp
+-rw-r--r--  2.0 unx    71114 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/ffbonded.itp
+-rw-r--r--  2.0 unx   134978 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/ffnonbonded.itp
+-rw-r--r--  2.0 unx      768 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/forcefield.itp
+-rw-r--r--  2.0 unx   126888 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/protein.mol2
+-rw-r--r--  2.0 unx     3821 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/protein.py
+-rw-r--r--  2.0 unx      477 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/tip3p.mol2
+-rw-r--r--  2.0 unx     1271 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/tip3p.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/charmm27/tips3p.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/special/__init__.py
+-rw-r--r--  2.0 unx    29126 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/special/fep.py
+-rw-r--r--  2.0 unx     3848 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/special/gb.py
+-rw-r--r--  2.0 unx     2316 b- defN 23-Apr-04 12:21 mindsponge/toolkits/forcefield/special/min.py
+-rw-r--r--  2.0 unx    84266 b- defN 23-Apr-04 12:21 mindsponge/toolkits/helper/__init__.py
+-rw-r--r--  2.0 unx     5470 b- defN 23-Apr-04 12:21 mindsponge/toolkits/helper/math.py
+-rw-r--r--  2.0 unx     7015 b- defN 23-Apr-04 12:21 mindsponge/toolkits/helper/namespace.py
+-rw-r--r--  2.0 unx     3516 b- defN 23-Apr-04 12:21 mindsponge/toolkits/helper/rdkit.py
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-04 12:21 mindsponge/toolkits/mdrun/BIN_PATH.dat
+-rw-r--r--  2.0 unx     1420 b- defN 23-Apr-04 12:21 mindsponge/toolkits/mdrun/__init__.py
+-rw-r--r--  2.0 unx      183 b- defN 23-Apr-04 12:21 mindsponge/toolkits/mdrun/__main__.py
+-rw-r--r--  2.0 unx    25249 b- defN 23-Apr-04 12:21 mindsponge/toolkits/tools/__init__.py
+-rw-r--r--  2.0 unx      778 b- defN 23-Apr-04 12:21 mindsponge_ascend-1.0.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 12:21 mindsponge_ascend-1.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-04 12:21 mindsponge_ascend-1.0.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36455 b- defN 23-Apr-04 12:21 mindsponge_ascend-1.0.0rc1.dist-info/RECORD
+360 files, 7472241 bytes uncompressed, 1681242 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -285,14 +285,395 @@
 
 Filename: mindsponge/partition/grids.py
 Comment: 
 
 Filename: mindsponge/partition/neighbourlist.py
 Comment: 
 
+Filename: mindsponge/pipeline/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/pipeline.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/amp.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/basic.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/equivariant.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/initializer.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/mask.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/msa.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/transition.py
+Comment: 
+
+Filename: mindsponge/pipeline/cell/triangle.py
+Comment: 
+
+Filename: mindsponge/pipeline/dataset/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/dataset/dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/dataset/pdbbind/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/dataset/pdbbind/pdbbind.py
+Comment: 
+
+Filename: mindsponge/pipeline/dataset/psp/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/dataset/psp/psp.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/model.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/colabdesign.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/colabdesign_configuratuin.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/colabdesign_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/colabdesign_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/module/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/module/design_wrapcell.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/module/loss_design.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/colabdesign/module/utils.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/deepdr/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/deepdr/deepdr.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/deepdr/deepdr_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/deepdr/deepdr_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/deepdr/deepdr_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/deepdr/mda_nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/deepdr/vae_nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/graphdta/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/graphdta/data_process.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/graphdta/get_train_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/graphdta/graphdta.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/graphdta/graphdta_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/graphdta/graphdta_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/graphdta/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/build_vocab.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/grover.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/grover_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/grover_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/save_features.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/split_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/data/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/data/mindsporevocab.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/data/molfeaturegenerator.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/data/molgraph.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/data/scaler.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/data/task_labels.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/data/transforms.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/model/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/model/layers.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/model_utils/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/model_utils/local_adapter.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/util/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/util/logger.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/util/nn_utils.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/util/scheduler.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/grover/src/util/utils.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/kgnn/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/kgnn/kgnn.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/kgnn/kgnn_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/kgnn/kgnn_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/kgnn/kgnn_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/kgnn/loss.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/kgnn/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaassessment/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaassessment/megaassessment_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaassessment/megassessment.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaassessment/megassessment_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaassessment/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaevogen/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaevogen/evogen.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaevogen/evogen_block.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaevogen/evogen_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaevogen/evogen_datafunction.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaevogen/evogen_dataprocess.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megaevogen/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/megafold.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/megafold_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/megafold_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/megafold_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/megafold_feature.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/evoformer.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/fold_wrapcell.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/head.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/loss_module.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/lr.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/structure.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/megafold/module/template_embedding.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/multimer.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/multimer_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/multimer_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/multimer_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/multimer_feature.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/module/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/module/multimer_block.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/module/multimer_evoformer.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/module/multimer_head.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/module/multimer_structure.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/multimer/module/multimer_template_embedding.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/pafnucy/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/pafnucy/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/pafnucy/pafnucy.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/pafnucy/pafnucy_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/pafnucy/pafnucy_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/pafnucy/pafnucy_dataset.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/ufold/__init__.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/ufold/nn_arch.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/ufold/ufold.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/ufold/ufold_configuration.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/ufold/ufold_data.py
+Comment: 
+
+Filename: mindsponge/pipeline/models/ufold/ufold_dataset.py
+Comment: 
+
 Filename: mindsponge/potential/__init__.py
 Comment: 
 
 Filename: mindsponge/potential/forcefield.py
 Comment: 
 
 Filename: mindsponge/potential/potential.py
@@ -681,20 +1062,20 @@
 
 Filename: mindsponge/toolkits/mdrun/__main__.py
 Comment: 
 
 Filename: mindsponge/toolkits/tools/__init__.py
 Comment: 
 
-Filename: mindsponge_ascend-1.0.0a0.dist-info/METADATA
+Filename: mindsponge_ascend-1.0.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: mindsponge_ascend-1.0.0a0.dist-info/WHEEL
+Filename: mindsponge_ascend-1.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: mindsponge_ascend-1.0.0a0.dist-info/top_level.txt
+Filename: mindsponge_ascend-1.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: mindsponge_ascend-1.0.0a0.dist-info/RECORD
+Filename: mindsponge_ascend-1.0.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mindsponge/__init__.py

```diff
@@ -69,7 +69,8 @@
 
 from .system import Molecule, Protein
 from .potential import PotentialCell, ForceFieldBase, ForceField
 from .optimizer import Updater, DynamicUpdater, SteepestDescent
 from .core import Sponge, SimulationCell, RunOneStepCell, AnalyseCell
 from .function.units import global_units, set_global_units
 from .function.units import set_global_length_unit, set_global_energy_unit
+from .pipeline import PipeLine
```

## mindsponge/cell/equivariant.py

```diff
@@ -31,15 +31,15 @@
     adding location information to the sequence representation.
 
     The attention consists of three parts, namely, q, k, v obtained by the sequence representation,
     q'k'v' obtained by the interaction between the sequence representation and the rigid body group,
     and b , which is th bias, obtained from the pair representation (the second inputs -- inputs_2d).
 
     .. math::
-        a_{ij} = Softmax(w_l(c_1{q_i}^Tk_j+b{ij}-c_2\sum {\left \| T_i\circ q'_i-T_j\circ k'_j \right \| ^{2 } })
+        a_{ij} = Softmax(w_l(c_1{q_i}^Tk_j+b{ij}-c_2\sum {\left \| T_i\circ q'_i-T_j\circ k'_j \right \| ^{2 } }))
 
     where i and j represent the ith and jth amino acids in the sequence, respectively,
     and T is the rotation and translation in the input.
 
     `Jumper et al. (2021) Suppl. Alg. 22 "InvariantPointAttention"
     <https://static-content.springer.com/esm/art%3A10.1038%2Fs41586-021-03819-2/MediaObjects/41586_2021_3819_MOESM1_ESM.pdf>`_.
 
@@ -68,19 +68,19 @@
         Tensor, the update of inputs_1d, shape :math:`[N_{res}, num\_channel]`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
+        >>> import mindspore as ms
         >>> from mindsponge.cell import InvariantPointAttention
         >>> from mindspore import dtype as mstype
         >>> from mindspore import Tensor
-        >>> import mindspore.context as context
-        >>> context.set_context(mode=context.GRAPH_MODE)
+        >>> ms.set_context(mode=ms.GRAPH_MODE)
         >>> model = InvariantPointAttention(num_head=12, num_scalar_qk=16, num_scalar_v=16,
         ...                                 num_point_v=8, num_point_qk=4,
         ...                                 num_channel=384, pair_dim=128)
         >>> inputs_1d = Tensor(np.ones((256, 384)), mstype.float32)
         >>> inputs_2d = Tensor(np.ones((256, 256, 128)), mstype.float32)
         >>> mask = Tensor(np.ones((256, 1)), mstype.float32)
         >>> rotation = tuple([Tensor(np.ones(256), mstype.float16) for _ in range(9)])
```

## mindsponge/cell/mask.py

```diff
@@ -14,20 +14,30 @@
 # ============================================================================
 """Mask"""
 from mindspore.ops import operations as P
 from mindspore.ops import functional as F
 import mindspore.nn as nn
 
 
+class LayerNormProcess(nn.Cell):
+    def __init__(self,):
+        super(LayerNormProcess, self).__init__()
+        self.layernorm = P.LayerNorm(begin_norm_axis=-1, begin_params_axis=-1, epsilon=1e-5)
+
+    def construct(self, msa_act, query_norm_gamma, query_norm_beta):
+        output, _, _ = self.layernorm(msa_act, query_norm_gamma, query_norm_beta)
+        return output
+
+
 class MaskedLayerNorm(nn.Cell):
     '''masked_layer_norm'''
 
     def __init__(self):
         super(MaskedLayerNorm, self).__init__()
-        self.norm = P.LayerNorm(begin_norm_axis=-1, begin_params_axis=-1, epsilon=1e-5)
+        self.norm = LayerNormProcess()
 
     def construct(self, act, gamma, beta, mask=None):
         '''construct'''
         act = act
         gamma = gamma
         beta = beta
 
@@ -35,10 +45,10 @@
         if mask is not None:
             mask = F.expand_dims(mask, -1)
             mask = mask * ones
         else:
             mask = ones
 
         act = act * mask
-        act, _, _ = self.norm(act, gamma, beta)
+        act = self.norm(act, gamma, beta)
         act = act * mask
         return act
```

## mindsponge/cell/msa.py

```diff
@@ -205,15 +205,15 @@
         >>> attn_out = model(msa_act, msa_mask, index)
         >>> print(attn_out.shape)
         (512, 256, 256)
     """
 
     def __init__(self, num_head, key_dim, gating, msa_act_dim, batch_size=None, slice_num=0):
         super(MSAColumnAttention, self).__init__()
-        self.query_norm = P.LayerNorm(begin_norm_axis=-1, begin_params_axis=-1, epsilon=1e-5)
+        self.query_norm = MaskedLayerNorm()
         self.attn_mod = Attention(num_head, key_dim, gating, msa_act_dim, msa_act_dim, msa_act_dim, batch_size)
         self.batch_size = batch_size
         self.slice_num = slice_num
         self.msa_act_dim = msa_act_dim
         self.idx = Tensor(0, mstype.int32)
         self._init_parameter()
 
@@ -226,15 +226,15 @@
             query_norm_gamma = self.query_norm_gammas
             query_norm_beta = self.query_norm_betas
         msa_act = P.Transpose()(msa_act, (1, 0, 2))
         msa_mask = P.Transpose()(msa_mask, (1, 0))
 
         input_mask = 1e9 * (msa_mask - 1.)
         input_mask = P.ExpandDims()(P.ExpandDims()(input_mask, 1), 2)
-        msa_act, _, _ = self.query_norm(msa_act, query_norm_gamma, query_norm_beta)
+        msa_act = self.query_norm(msa_act, query_norm_gamma, query_norm_beta)
         batched_inputs = (msa_act, input_mask)
         nonbatched_inputs = (index,)
         msa_act = _memory_reduce(self._compute, batched_inputs, nonbatched_inputs, self.slice_num)
         msa_act = P.Transpose()(msa_act, (1, 0, 2))
         return msa_act
 
     def _init_parameter(self):
@@ -250,15 +250,15 @@
         msa_act = self.attn_mod(msa_act, msa_act, input_mask, index)
         return msa_act
 
 
 class MSAColumnGlobalAttention(nn.Cell):
     r"""
     MSA column global attention. Transpose MSA information at sequence axis and residue axis, then use `GlobalAttention
-    <https://www.mindspore.cn/mindsponge/docs/zh-CN/r1.0.0-alpha/cell/mindsponge.cell.GlobalAttention.html>` to
+    <https://www.mindspore.cn/mindsponge/docs/zh-CN/r1.0/cell/mindsponge.cell.GlobalAttention.html>`_ to
     do Attention between input sequences without dealing with the relationship between residues in sequence.
     Comparing with MSAColumnAttention, it uses GlobalAttention to deal with longer input sequence.
 
     Reference:
         `Jumper et al. (2021) Suppl. Alg. 19 'MSAColumnGlobalAttention'
         <https://www.nature.com/articles/s41586-021-03819-2>`_.
 
@@ -294,15 +294,15 @@
         >>> print(msa_out.shape)
         (4, 256, 64)
     """
 
     def __init__(self, num_head, gating, msa_act_dim, batch_size=None, slice_num=0):
         super(MSAColumnGlobalAttention, self).__init__()
         self.attn_mod = GlobalAttention(num_head, gating, msa_act_dim, msa_act_dim, batch_size)
-        self.query_norm = P.LayerNorm(begin_norm_axis=-1, begin_params_axis=-1, epsilon=1e-5)
+        self.query_norm = MaskedLayerNorm()
         self.batch_size = batch_size
         self.slice_num = slice_num
         self.msa_act_dim = msa_act_dim
         self.idx = Tensor(0, mstype.int32)
         self._init_parameter()
 
     def construct(self, msa_act, msa_mask, index=None):
@@ -317,17 +317,17 @@
             query_norm_beta = self.query_norm_betas
             msa_act = P.Transpose()(msa_act, (1, 0, 2))
             msa_mask = P.Transpose()(msa_mask, (1, 0))
 
         input_mask = 1e9 * (msa_mask - 1.)
         input_mask = P.ExpandDims()(P.ExpandDims()(input_mask, 1), 2)
 
-        msa_act, _, _ = self.query_norm(msa_act,
-                                        query_norm_gamma,
-                                        query_norm_beta)
+        msa_act = self.query_norm(msa_act,
+                                  query_norm_gamma,
+                                  query_norm_beta)
         msa_mask = P.ExpandDims()(msa_mask, -1)
         batched_inputs = (msa_act, msa_mask)
         nonbatched_inputs = (index,)
         msa_act = _memory_reduce(self._compute, batched_inputs, nonbatched_inputs, self.slice_num)
         msa_act = P.Transpose()(msa_act, (1, 0, 2))
         return msa_act
```

## mindsponge/cell/transition.py

```diff
@@ -39,22 +39,22 @@
         input_dim(int):                    The channels of the input.
         batch_size(int):                   The batch size of parameters in Transition,
                                            used in while control flow. Default: "None".
         slice_num (int):                   The slice num used in transition layer
                                            when the memory is overflow. Default: 0.
 
     Inputs:
-        - **act** (Tensor) - The input with channels equal to input_dim, shape is (..., input_dim).
+        - **act** (Tensor) - The input with channels equal to input_dim, shape is :math:`(..., input\_dim)`.
         - **index** (Tensor) - The index of while loop, only used in case of while control
           flow. Default: "None".
-        - **mask** (Tensor) - The mask of act when to do layernorm with shape :math:`(32, input_{dim})`,
+        - **mask** (Tensor) - The mask of act when to do layernorm with shape :math:`(32, input_\dim)`,
           Default: "None".
 
     Outputs:
-        Tensor, the float tensor of the output of the layer with shape (..., input_dim).
+        Tensor, the float tensor of the output of the layer with shape :math:`(..., input\_dim)`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindsponge.cell import Transition
```

## mindsponge/cell/triangle.py

```diff
@@ -180,15 +180,15 @@
         (256, 256, 64)
     """
 
     def __init__(self, num_intermediate_channel, equation, layer_norm_dim, batch_size=None):
         super(TriangleMultiplication, self).__init__()
         self.num_intermediate_channel = num_intermediate_channel
         self.equation = equation
-        self.layer_norm = P.LayerNorm(begin_norm_axis=-1, begin_params_axis=-1, epsilon=1e-5)
+        self.layer_norm = MaskedLayerNorm()
         self.matmul = P.MatMul(transpose_b=True)
         self.sigmoid = nn.Sigmoid()
         self.batch_matmul_trans_b = P.BatchMatMul(transpose_b=True)
         equation = ["ikc,jkc->ijc", "kjc,kic->ijc"]
         if self.equation not in equation:
             print("TriangleMultiplication Not Suppl")
         if self.equation == "ikc,jkc->ijc":
@@ -246,17 +246,17 @@
             center_layer_norm_beta = self.center_layer_norm_betas
             output_projection_weight = self.output_projection_weights
             output_projection_bias = self.output_projection_biases
             gating_linear_weight = self.gating_linear_weights
             gating_linear_bias = self.gating_linear_biases
 
         mask = P.ExpandDims()(mask, -1)
-        act, _, _ = self.layer_norm(act,
-                                    layer_norm_input_gamma,
-                                    layer_norm_input_beta)
+        act = self.layer_norm(act,
+                              layer_norm_input_gamma,
+                              layer_norm_input_beta)
 
         act_shape = P.Shape()(act)
         if len(act_shape) != 2:
             act = P.Reshape()(act, (-1, act_shape[-1]))
         out_shape = act_shape[:-1] + (-1,)
         input_act = act
         left_projection = P.BiasAdd()(self.matmul(act, left_projection_weight), left_projection_bias)
@@ -282,17 +282,17 @@
                 act = P.Transpose()(act, (1, 2, 0))
             else:
                 left_proj_act_tmp = P.Transpose()(left_proj_act, (2, 1, 0))
                 right_proj_act_tmp = P.Transpose()(right_proj_act, (2, 1, 0))
                 act = self.batch_matmul_trans_b(left_proj_act_tmp, right_proj_act_tmp)
                 act = P.Transpose()(act, (2, 1, 0))
 
-        act, _, _ = self.layer_norm(act,
-                                    center_layer_norm_gamma,
-                                    center_layer_norm_beta)
+        act = self.layer_norm(act,
+                              center_layer_norm_gamma,
+                              center_layer_norm_beta)
 
         if len(act_shape) != 2:
             act = P.Reshape()(act, (-1, act_shape[-1]))
 
         act = P.BiasAdd()(self.matmul(act, output_projection_weight), output_projection_bias)
         gate_values = P.BiasAdd()(self.matmul(input_act, gating_linear_weight), gating_linear_bias)
         gate_values = self.sigmoid(gate_values)
@@ -401,29 +401,29 @@
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindsponge.cell import OuterProductMean
         >>> from mindspore import dtype as mstype
         >>> from mindspore import Tensor
-        >>> from mindspore.ops import operations as P
+        >>> from mindspore import ops
         >>> model = OuterProductMean(num_outer_channel=32, act_dim=128, num_output_channel=256)
         >>> act = Tensor(np.ones((32, 64, 128)), mstype.float32)
         >>> mask = Tensor(np.ones((32, 64)), mstype.float32)
-        >>> mask_norm = P.ExpandDims()(P.MatMul(transpose_a=True)(mask, mask), -1)
+        >>> mask_norm = ops.ExpandDims()(P.MatMul(transpose_a=True)(mask, mask), -1)
         >>> output= model(act, mask, mask_norm)
         >>> print(output.shape)
         (64, 64, 256)
     """
 
     def __init__(self, num_outer_channel, act_dim, num_output_channel, batch_size=None, slice_num=0):
         super(OuterProductMean, self).__init__()
         self.num_output_channel = num_output_channel
         self.num_outer_channel = num_outer_channel
-        self.layer_norm_input = P.LayerNorm(begin_norm_axis=-1, begin_params_axis=-1, epsilon=1e-5)
+        self.layer_norm_input = MaskedLayerNorm()
         self.matmul_trans_b = P.MatMul(transpose_b=True)
         self.matmul = P.MatMul()
         self.batch_matmul_trans_b = P.BatchMatMul(transpose_b=True)
         self.act_dim = act_dim
         self.batch_size = batch_size
         self.slice_num = slice_num
         self.idx = Tensor(0, mstype.int32)
@@ -447,15 +447,15 @@
             left_projection_weight = self.left_projection_weights
             left_projection_bias = self.left_projection_biases
             right_projection_weight = self.right_projection_weights
             right_projection_bias = self.right_projection_biases
             linear_output_weight = self.linear_output_weights
             linear_output_bias = self.o_biases
         mask = P.ExpandDims()(mask, -1)
-        act, _, _ = self.layer_norm_input(act, layer_norm_input_gamma, layer_norm_input_beta)
+        act = self.layer_norm_input(act, layer_norm_input_gamma, layer_norm_input_beta)
         act_shape = P.Shape()(act)
         if len(act_shape) != 2:
             act = P.Reshape()(act, (-1, act_shape[-1]))
         out_shape = act_shape[:-1] + (-1,)
         left_act = mask * P.Reshape()(
             P.BiasAdd()(self.matmul_trans_b(act, left_projection_weight), left_projection_bias), out_shape)
         right_act = mask * P.Reshape()(
```

## mindsponge/common/geometry.py

```diff
@@ -332,15 +332,15 @@
 
     Examples:
         >>> import mindsponge
         >>> v1 = (1, 2, 3)
         >>> v2 = (3, 4, 5)
         >>> ans = mindsponge.common.vecs_cross_vecs(v1, v2)
         >>> print(ans)
-        (2, -4, 2)
+        (-2, 4, -2)
     """
     cross_res = (v1[1] * v2[2] - v1[2] * v2[1],
                  v1[2] * v2[0] - v1[0] * v2[2],
                  v1[0] * v2[1] - v1[1] * v2[0])
     return cross_res
 
 
@@ -361,22 +361,24 @@
 
     The unit vector of :math:`\vec e_1'` is :math:`\vec e_1 = \frac{\vec e_1'}{|\vec e_1'|}`,
     which is the y axis of the local coordinate system.
 
     Finally get the unit vector of z axis :math:`\vec e_2` by calculating cross product of
     :math:`\vec e_1` and :math:`\vec e_0`.
 
+    The final rots is :math:`(e_{0x}, e_{1x}, e_{2x}, e_{0y}, e_{1y}, e_{2y}, e_{0z}, e_{1z}, e_{2z})`.
+
     Args:
         e0_unnormalized (tuple):    vectors :math:`\vec a` as x-axis of x-y plane,
                                     length is 3. Data type is constant or Tensor with same shape.
         e1_unnormalized (tuple):    vectors :math:`\vec b` forming x-y plane,
                                     length is 3. Data type is constant or Tensor with same shape.
 
     Returns:
-        tuple, rotation matrix :math:`(e_0_x, e_1_x, e_2_x, e_0_y, e_1_y, e_2_y, e_0_z, e_1_z, e_2_z)` .
+        tuple, rotation matrix :math:`(e_{0x}, e_{1x}, e_{2x}, e_{0y}, e_{1y}, e_{2y}, e_{0z}, e_{1z}, e_{2z})` .
             Data type is constant or Tensor with same shape.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import mindsponge
@@ -539,19 +541,20 @@
     local coordinate system to global coordinate system.
 
     Use `invert_rots` to calculate the invert rotations of rigid. Then use
     `rots_mul_vecs` to rotate the translations of rigid. The opposite of the
     result is the translations of invert rigid.
 
     .. math::
-        inv\_rots = r_r^T = (r_0, r_3, r_6, r_1, r_4, r_7, r_2, r_5, r_8)
-
-        inv\_trans = -r_r^T \cdot r_t^T = (- (r_0 \times t_0 + r_3 \times t_0 + r_6 \times t_0),
+        \begin{split}
+        &inv\_rots = r_r^T = (r_0, r_3, r_6, r_1, r_4, r_7, r_2, r_5, r_8) \\
+        &inv\_trans = -r_r^T \cdot r_t^T = (- (r_0 \times t_0 + r_3 \times t_0 + r_6 \times t_0),
                                            - (r_1 \times t_1 + r_4 \times t_1 + r_7 \times t_1),
-                                           - (r_2 \times t_2 + r_5 \times t_2 + r_8 \times t_2))
+                                           - (r_2 \times t_2 + r_5 \times t_2 + r_8 \times t_2)) \\
+        \end{split}
 
     Args:
         rigids (tuple): rigids, including the rots and trans changing rigids
                         from global coordinate system to local coordinate system.
 
     Returns:
         tuple(rots, trans), group inverse of rigid transformations, length is 2. Include rots
@@ -579,17 +582,17 @@
 def vecs_add(v1, v2):
     """Add two vectors 'v1' and 'v2'."""
     return (v1[0] + v2[0], v1[1] + v2[1], v1[2] + v2[2])
 
 
 def rigids_mul_vecs(rigids, v):
     r"""
-    Transform vector :math:`v` to rigid' local coordinate system.
+    Transform vector :math:`\vec v` to rigid' local coordinate system.
 
-    Multiply vector :math:`v` and the rotations of rigid together
+    Multiply vector :math:`\vec v` and the rotations of rigid together
     and add the translations of rigid. The result is the output vector.
 
     .. math::
         v = r_rv+r_t
 
     Args:
         rigids (tuple): rigid.
@@ -612,23 +615,23 @@
     return vecs_add(rots_mul_vecs(rigids[0], v), rigids[1])
 
 
 def rigids_mul_rots(x, y):
     r"""
     Numpy version of getting results rigid :math:`x` multiply rotations :math:`\vec y` .
 
-    Multiply rotations of rigid :math:`x` with rotations :math:`y`,
+    Multiply rotations of rigid :math:`x[0]` with rotations :math:`\vec y`,
     the result is rigids new rotations. Translations of rigid will not changed.
 
     .. math::
         (r, t) = (x_ry, x_t)
 
     Args:
-        x (tuple):  rigid :math:`x` . Length is 2. Include rots :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`
-                    and trans :math:`(x, y, z)` . Data type is constant or Tensor with same shape.
+        x (tuple):  rigid :math:`x` . Length is 2. Include rots :math:`x_r = (xx, xy, xz, yx, yy, yz, zx, zy, zz)`
+                    and trans :math:`x_t = (x, y, z)` . Data type is constant or Tensor with same shape.
         y (tuple):  rotations :math:`\vec y` , length is 9. Data type is constant or Tensor with same shape.
 
     Returns:
         tuple(rots, trans), length is 2, rigid whose rotations are changed.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
@@ -644,15 +647,15 @@
     rigids = (rots_mul_rots(x[0], y), x[1])
     return rigids
 
 
 def rigids_mul_rigids(a, b):
     r"""
     Change rigid :math:`b` from its local coordinate system to rigid :math:`a`
-    local coordinate system, using rigid :math:`a` rotations and translations.
+    local coordinate system, using rigid rotations and translations.
 
     Use the rotations calculated by multiplying rotations of rigid :math:`b`
     and rigid :math:`a` as new rotations of rigid :math:`b` .
 
     Multiply the translations of rigid :math:`b` with rotations of rigid :math:`a` ,
     then add translations of rigid :math:`a` . The translations got is new translations
     of rigid :math:`b`.
@@ -708,15 +711,15 @@
         \end{split}
 
     Args:
         x(tuple):   rots x, :math:`(xx1, xy1, xz1, yx1, yy1, yz1, zx1, zy1, zz1)`.
         y(tuple):   rots y, :math:`(xx2, xy2, xz2, yx2, yy2, yz2, zx2, zy2, zz2)`.
 
     Returns:
-        tuple, the result of rots x multiplying rots y. Shape is :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`.
+        tuple, the result of rots x multiplying rots y. The result is :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindsponge.common.geometry import rots_mul_rots
         >>> rtos_0 = (1, 1, 1, 1, 1, 1, 1)
@@ -736,15 +739,16 @@
     """
     Get vectors from the last axis of input tensor.
 
     Args:
         inputs(Tensor): Atom position information. Shape is :math:`(..., 3)`.
 
     Returns:
-        tuple :math:`(x, y, z)` , including the coordinate information of x, y and z.
+        tuple :math:`(x, y, z)` with three tensors,
+        including the coordinate information of x, y and z.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore as ms
@@ -761,15 +765,16 @@
 
 
 def vecs_to_tensor(v):
     """
     Converts 'v' to tensor with last dim shape 3, inverse of 'vecs_from_tensor'.
 
     Args:
-        v(tuple):   Input tuple v :math:`(x, y, z)`, including the coordinate information of x, y and z.
+        v(tuple):   Input tuple v :math:`(x, y, z)` with three tensors, including
+                    the coordinate information of x, y and z.
 
     Returns:
         tensor, concat the tensor in last dims, shape :math:`(..., 3)` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
@@ -818,17 +823,17 @@
                                             shape is :math:`[..., N_{res}, 3]` .
         point_b(float, tensor) -> (tensor): Spatial location information of atom 'CA',
                                             shape is :math:`[..., N_{res}, 3]` .
         point_c(float, tensor) -> (tensor): Spatial location information of atom 'C',
                                             shape is :math:`[..., N_{res}, 3]` .
 
     Returns:
-        - Tuple, rots :math:`[xx, xy, xz, yx, yy, yz, zx, zy, zz]` ,
+        - Tuple, rots :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)` ,
           the shape of every element is :math:`(..., N_{res})` .
-        - Tuple, trans :math:`[x, y, z]` , the shape of every element is :math:`(..., N_{res})` .
+        - Tuple, trans :math:`(x, y, z)` , the shape of every element is :math:`(..., N_{res})` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore as ms
@@ -883,15 +888,15 @@
       to obtain each component of the rotation matrix, inverse of 'rots_to_tensor'.
 
     Args:
         rots(Tensor):       Represent the rotation matrix, shape is :math:`(..., 3, 3)` .
         use_numpy(bool):    Whether to use numpy to calculate. Default: False.
 
     Returns:
-        Tuple, rots represented by vectors, shape is :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`.
+        Tuple, rots represented by vectors, rots is :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore as ms
@@ -956,16 +961,18 @@
         rotation(tensor):       Rots, shape is :math:`(N_{res}, 9)`. Default: None.
         normalize(bool):        Whether to use normalization. Default: True.
         unstack_inputs(bool):   Whether input is vector(True) of Tensor(False). Default: False.
         use_numpy(bool):        Whether to use numpy. Default: False.
 
     Returns:
         result after quat affine.
+
         - quaternion, tensor, shape is :math:`(N_{res}, 4)` .
-        - rotation, tuple, :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`, shape of every element is :math:`(N_{res},)` .
+        - rotation, tuple, :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`,
+          shape of every element is :math:`(N_{res},)` .
         - translation, tensor, shape is :math:`(N_{res}, 3)` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
@@ -1008,15 +1015,15 @@
         \end{split}
 
     Args:
         normalized_quat (tensor): normalized quaternion, shape :math:`(N_{res}, 4)`.
         use_numpy (bool): use numpy or not, Default: "False".
 
     Returns:
-        tuple, rotation :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`, every element shape :math:`(N_{res},)`.
+        tuple, rotation :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`, every element shape :math:`(N_{res}, )`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore as ms
@@ -1048,16 +1055,16 @@
     Args:
         num_residues(int):  Number of residues.
         use_numpy(bool):    Whether to use numpy. Default: False.
 
     Returns:
         result after quat affine.
         - quaternion, tensor, shape is :math:`(N_{res}, 4)` .
-        - rotation, tuple, :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`, shape of every element is :math:`(N_{res},)` .
-        - translation, tensor, shape is :math:`(N_{res}, 3)` .
+        - rotation, tuple, :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`, shape of every element is :math:`(N_{res}, )` .
+        - translation, tuple, :math:`(x, y, z)` shape of every element tensor is :math:`(N_{res}, )` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore as ms
@@ -1087,17 +1094,17 @@
     Add an extra dimension to the input `v` at the given axis.
 
     Args:
         v(Tuple):   Input vector. Length is 3, :math:`(xx, xy, xz)` .
         axis(int):  Specifies the dimension index at which to expand the shape of `v`. Only constant value is allowed.
 
     Returns:
-        Tuple, if the axis is 0, and the shape of :math:`xx` is :math:`(... , X_R)`, where X_R is any number.
-          If the axis is other value, then expand in the other direction. And return expanded
-          :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`
+        Tuple, if the axis is 0, and the shape of :math:`xx` is :math:`(..., X_R)`, where X_R is any number.
+          The expanded shape is :math:`(1, ..., X_R)`. If the axis is other value, then expand in the other
+          direction. And return expanded :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindsponge.common.geometry import vecs_expand_dims
         >>> from mindspore.common import Tensor
@@ -1120,16 +1127,16 @@
     Args:
         rots (Tuple):   The rotation matrix is :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`,
                         and xx and xy have the same shape
         axis (Int):     Specifies the dimension index at which to expand the shape of v.
                         Only constant value is allowed.
 
     Returns:
-        Tuple, rots. If the value of axis is 0, and the shape of xx is :math:`(... ,X_R)`,
-          where X_R is any number, and the expanded shape is :math:`(1,... ,X_R)`.
+        Tuple, rots. If the value of axis is 0, and the shape of xx is :math:`(..., X_R)`,
+          where X_R is any number, and the expanded shape is :math:`(1, ..., X_R)`.
           Return expanded :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindsponge.common.geometry import rots_expand_dims
@@ -1159,16 +1166,16 @@
     matrix :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)` and the translation vector :math:`(x, y, z)` translation.
 
     First, the initial coordinates are translated, and then the transpose of the rotation matrix is multiplied
     by rot_point to get the final coordinates.
 
     .. math::
         \begin{split}
-        &rot_point = transformed_point - translation \\
-        &result = rotation^t * rot_point \\
+        &rot\_point = transformed\_point - translation \\
+        &result = rotation^T * rot\_point \\
         \end{split}
 
     The specific procedures of vector subtraction, transpose and multiplication can be referred to the
     api of vecs_sub, invert_rots, rots_mul_vecs etc.
 
     Args:
         transformed_point (Tuple):  The initial coordinates of the input have shape :math:`(x, y, z)`,
@@ -1211,16 +1218,16 @@
 
 def quat_multiply_by_vec(quat, vec):
     r"""
     Multiply a quaternion by a pure-vector quaternion.
 
     .. math::
         \begin{split}
-        &temp =  QUAT_MULTIPLY_BY_VEC * quat[..., :, None, None] * vec[..., None, :, None] \\
-        &result = sum(tempc,axis=(-3, -2)) \\
+        &temp =  QUAT\_MULTIPLY\_BY\_VEC * quat[..., :, None, None] * vec[..., None, :, None] \\
+        &result = sum(temp,axis=(-3, -2)) \\
         \end{split}
 
     Args:
         quat (Tensor):  Quaternion.Tensor of shape :math:`(..., 4)`.
         vec (Tensor):   A pure-vector quaternion, :math:`(b, c, d)` not normalized quaternion.
                         Quaternion can be expressed as :math:`(1, b, c, d)`.
 
@@ -1252,22 +1259,22 @@
     Return a new QuatAffine which applies the transformation update first.
 
     The process of obtaining the updated translation vector and rotation matrix is as follows:
 
     .. math::
         \begin{split}
         &update = (xx, xy, xz, yx, yy, yz) \\
-        &vector_quaternion_update = (xx, xy, xz) \\
+        &vector\_quaternion\_update = (xx, xy, xz) \\
         &x = (yx) \\
         &y = (yy) \\
         &z = (yz) \\
-        &trans_update = (x, y, z) \\
-        &new_quaternion = quaternion + vector_quaternion_update * quaternion \\
-        &rotated_trans_update = rotation * trans_update \\
-        &new_translation = translation + rotated_trans_update \\
+        &trans\_update = (x, y, z) \\
+        &new\_quaternion = quaternion + vector\_quaternion\_update * quaternion \\
+        &rotated\_trans\_update = rotation * trans\_update \\
+        &new\_translation = translation + rotated\_trans\_update \\
         \end{split}
 
     vector_quaternion_update and quaternion are multiplied by the quat_multiply_by_vec function,
     Affine transformation is performed using the generated new_quaternion and new_translation.
     The process of affine transformation is referred to the quat_affine api.
 
     Args:
@@ -1359,28 +1366,31 @@
     translation = (P.ExpandDims()(translation[0], -1), P.ExpandDims()(translation[1], -1),
                    P.ExpandDims()(translation[2], -1),)
     return mnp.concatenate((quaternion,) + translation, axis=-1)
 
 
 def quaternion_from_tensor(tensor, normalize=False):
     r"""
-    Take the input 'tensor' to get the new 'quaternion', 'rotation', 'translation'.
+    Take the input 'tensor' :math:`[(xx, xy, xz, yx, yy, yz, zz)]` to get the new
+    'quaternion', 'rotation', 'translation'.
 
     .. math::
         \begin{split}
-        &quaternion = [(x_1, y_1, z_1, m_1)] \\
-        &translation = [(x_2, y_2, z_2)] \\
-        &result = [(x_1, y_1, z_1, m_1, x_2, y_2, z_2)] \\
+        &tensor = [(xx, xy, xz, yx, yy, yz, zz)] \\
+        &quaternion = (xx, xy, xz, yx) \\
+        &translation = (yy, yz, zz) \\
         \end{split}
 
     Affine transformation is performed using the generated quaternion and translation.
     The process of affine transformation is referred to the quat_affine api.
 
     Args:
-        tensor(Tensor):     An initial Tensor of shape is :math:`[(... 7)]`.
+        tensor(Tensor):     An initial Tensor :math:`[(xx, xy, xz, yx, yy, yz, zz)]` .
+                            :math:`[(xx, xy, xz, yx)]` is the same with `quaternion`.
+                            :math:`(yy, yz, zz)` is the same with `translation`.
         normalize(bool):    Control whether to find the norm during quat_affine. Default: False.
 
     Returns:
         - Tensor, new quaternion.Tensor of shape :math:`(..., 4)` .
         - Tuple, new rotation, :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`,
           and xx and xy are Tensor and have the same shape.
         - Tuple, translation vector :math:`[(x, y, z)]`, where x, y and z are Tensor and have the same shape.
@@ -1413,27 +1423,27 @@
 
 def apply_to_point(rotation, translation, point, extra_dims=0):
     r"""
     Rotate and translate the input coordinates.
 
     .. math::
         \begin{split}
-        &rot_point = rotation * point \\
+        &rot_point = rotation \cdot point \\
         &result = rot_point + translation \\
         \end{split}
 
     For specific multiplication and addition procedures, refer to the rots_mul_vecs and vecs_add apis.
 
     Args:
         rotation(Tuple):    The rotation matrix :math:`(xx, xy, xz, yx, yy, yz, zx, zy, zz)`,
-                            and xx and xy are Tensor and have the same shape.
+                            and :math:`xx, xy` are Tensor and have the same shape.
         translation(Tuple): Translation vector :math:`[(x, y, z)]`,
-                            where x, y and z are Tensor and have the same shape.
+                            where :math:`x, y, z` are Tensor and have the same shape.
         point(Tensor):      Initial coordinate values :math:`[(x, y, z)]`,
-                            where x, y and z are Tensor and have the same shape.
+                            where :math:`x, y, z` are Tensor and have the same shape.
         extra_dims(int):    Control whether to expand dims. default:0.
 
     Returns:
         Tuple, the result of the coordinate transformation. Length is 3.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
```

## mindsponge/common/protein.py

```diff
@@ -21,14 +21,17 @@
 import numpy as np
 
 from . import residue_constants
 
 FeatureDict = Mapping[str, np.ndarray]
 ModelOutput = Mapping[str, Any]  # Is a nested dict.
 
+PDB_CHAIN_IDS = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789'
+PDB_MAX_CHAINS = len(PDB_CHAIN_IDS)  # := 62.
+
 
 @dataclasses.dataclass(frozen=True)
 class Protein:
     """Protein structure representation."""
 
     # Cartesian coordinates of atoms in angstroms. The atom types correspond to
     # residue_constants.atom_types, i.e. the first three are N, CA, CB.
@@ -223,7 +226,154 @@
 
     return Protein(
         aatype=aatype,
         atom_positions=final_atom_positions,
         atom_mask=final_atom_mask,
         residue_index=residue_index + 1,
         b_factors=b_factors)
+
+
+@dataclasses.dataclass(frozen=True)
+class ProteinV2:
+    """ProteinV2 structure representation."""
+
+    # Cartesian coordinates of atoms in angstroms. The atom types correspond to
+    # residue_constants.atom_types, i.e. the first three are N, CA, CB.
+    atom_positions: np.ndarray  # [num_res, num_atom_type, 3]
+
+    # Amino-acid type for each residue represented as an integer between 0 and
+    # 20, where 20 is 'X'.
+    aatype: np.ndarray  # [num_res]
+
+    # Binary float mask to indicate presence of a particular atom. 1.0 if an atom
+    # is present and 0.0 if not. This should be used for loss masking.
+    atom_mask: np.ndarray  # [num_res, num_atom_type]
+
+    # Residue index as used in PDB. It is not necessarily continuous or 0-indexed.
+    residue_index: np.ndarray  # [num_res]
+
+    # 0-indexed number corresponding to the chain in the protein that this residue
+    # belongs to.
+    chain_index: np.ndarray  # [num_res]
+
+    # B-factors, or temperature factors, of each residue (in sq. angstroms units),
+    # representing the displacement of the residue from its ground truth mean
+    # value.
+    b_factors: np.ndarray  # [num_res, num_atom_type]
+
+
+def to_pdb_v2(prot: ProteinV2) -> str:
+    """Converts a `Protein` instance to a PDB string.
+
+    Args:
+      prot: The protein to convert to PDB.
+
+    Returns:
+      PDB string.
+    """
+    restypes = residue_constants.restypes + ['X']
+    res_1to3 = lambda r: residue_constants.restype_1to3.get(restypes[r], 'UNK')
+    atom_types = residue_constants.atom_types
+
+    pdb_lines = []
+
+    atom_mask = prot.atom_mask
+    aatype = prot.aatype
+    atom_positions = prot.atom_positions
+    residue_index = prot.residue_index.astype(np.int32)
+    chain_index = prot.chain_index.astype(np.int32)
+    b_factors = prot.b_factors
+
+    if np.any(aatype > residue_constants.restype_num):
+        raise ValueError('Invalid aatypes.')
+
+    chain_ids = {}
+    for i in np.unique(chain_index):  # np.unique gives sorted output.
+        if i >= PDB_MAX_CHAINS:
+            raise ValueError(
+                f'The PDB format supports at most {PDB_MAX_CHAINS} chains.')
+        chain_ids[i] = PDB_CHAIN_IDS[i]
+
+    pdb_lines.append('MODEL     1')
+    atom_index = 1
+    last_chain_index = chain_index[0]
+    # Add all atom sites.
+    for i in range(aatype.shape[0]):
+        if last_chain_index != chain_index[i]:
+            chain_end = 'TER'
+            chain_termination_line = (
+                f'{chain_end:<6}{atom_index:>5}      {res_1to3(aatype[i - 1]):>3} '
+                f'{chain_ids[chain_index[i - 1]]:>1}{residue_index[i - 1]:>4}')
+            pdb_lines.append(chain_termination_line)
+            last_chain_index = chain_index[i]
+            atom_index += 1  # Atom index increases at the TER symbol.
+
+        res_name_3 = res_1to3(aatype[i])
+        for atom_name, pos, mask, b_factor in zip(
+                atom_types, atom_positions[i], atom_mask[i], b_factors[i]):
+            if mask < 0.5:
+                continue
+
+            record_type = 'ATOM'
+            name = atom_name if len(atom_name) == 4 else f' {atom_name}'
+            alt_loc = ''
+            insertion_code = ''
+            occupancy = 1.00
+            element = atom_name[0]  # Protein supports only C, N, O, S, this works.
+            charge = ''
+            # PDB is a columnar format, every space matters here!
+            atom_line = (f'{record_type:<6}{atom_index:>5} {name:<4}{alt_loc:>1}'
+                         f'{res_name_3:>3} {chain_ids[chain_index[i]]:>1}'
+                         f'{residue_index[i]:>4}{insertion_code:>1}   '
+                         f'{pos[0]:>8.3f}{pos[1]:>8.3f}{pos[2]:>8.3f}'
+                         f'{occupancy:>6.2f}{b_factor:>6.2f}          '
+                         f'{element:>2}{charge:>2}')
+            pdb_lines.append(atom_line)
+            atom_index += 1
+
+    # Close the chain.
+    chain_end = 'TER'
+    chain_termination_line = (
+        f'{chain_end:<6}{atom_index:>5}      {res_1to3(aatype[-1]):>3} '
+        f'{chain_ids[chain_index[-1]]:>1}{residue_index[-1]:>4}')
+    pdb_lines.append(chain_termination_line)
+    pdb_lines.append('ENDMDL')
+
+    pdb_lines.append('END')
+    pdb_lines.append('')
+    return '\n'.join(pdb_lines)
+
+
+def from_prediction_v2(final_atom_positions,
+                       final_atom_mask,
+                       aatype,
+                       residue_index,
+                       b_factors=None,
+                       asym_id=None,
+                       remove_leading_feature_dimension=True) -> ProteinV2:
+    """Assembles a protein from a prediction.
+
+    Args:
+        final_atom_positions: atom positions
+        final_atom_mask: atom mask
+        aatype: amino acid type
+        residue_index: idx of the residue
+    Returns:
+        A protein instance.
+    """
+    def _maybe_remove_leading_dim(arr: np.ndarray) -> np.ndarray:
+        return arr[0] if remove_leading_feature_dimension else arr
+
+    if asym_id is not None:
+        chain_index = _maybe_remove_leading_dim(asym_id)
+    else:
+        chain_index = np.zeros_like(aatype)
+    if b_factors is None:
+        b_factors = np.zeros_like(final_atom_mask)
+
+    return ProteinV2(
+        aatype=aatype,
+        atom_positions=final_atom_positions,
+        atom_mask=final_atom_mask,
+        residue_index=residue_index + 1,
+        chain_index=chain_index,
+        b_factors=b_factors)
```

## mindsponge/common/utils.py

```diff
@@ -387,21 +387,21 @@
       `common.residue_constants.atom_types`. So coordinates of atoms in protein can be encoded
       as a Tensor with shape :math:`(N_{res}, 37, 3)`.
     - Densely encoding. 20 amino acids contain a total of 14 atom types as shown in
       `common.residue_constants.restype_name_to_atom14_names`. So coordinates of atoms in protein can be encoded
       as a Tensor with shape :math:`(N_{res}, 14, 3)`.
 
     Args:
-        aatype(numpy.array):                Protein sequence encoding. the encoding method refers to
-                                            `common.residue_constants.restype_order`. The value ranges from 0 to 20.
+        aatype(numpy.ndarray):              Protein sequence encoding. the encoding method refers to
+                                            `common.residue_constants.restype_order`. Value range is :math:`[0,20]`.
                                             20 means the amino acid is unknown (`UNK`).
-        all_atom_mask(numpy.array):         Mask of coordinates of all atoms in proteins. Shape is
+        all_atom_mask(numpy.ndarray):       Mask of coordinates of all atoms in proteins. Shape is
                                             :math:`(N_{res}, 37)`. If the corresponding position is 0, the amino acid
                                             does not contain the atom.
-        all_atom_positions(numpy.array):    Coordinates of all atoms in protein. Shape is :math:`(N_{res}, 37, 3)` .
+        all_atom_positions(numpy.ndarray):  Coordinates of all atoms in protein. Shape is :math:`(N_{res}, 37, 3)` .
 
     Returns:
         - numpy.array. Densely encoding, mask of all atoms in protein, including unknown amino acid atoms.
           Shape is :math:`(N_{res}, 14)`.
         - numpy.array. Densely encoding, mask of all atoms in protein, excluding unknown amino acid atoms.
           Shape is :math:`(N_{res}, 14)`.
         - numpy.array. Densely encoding, coordinates of all atoms in protein. Shape is :math:`(N_{res}, 14, 3)`.
@@ -570,15 +570,16 @@
     Args:
         pdb_path(str): the path of the input pdb.
 
     Returns:
         features(dict), the information of pdb, including these keys
 
         - aatype, numpy.array. Protein sequence encoding. Encoding method refers to
-          `common.residue_constants_restype_order`, [0:20]. 20 means the amino acid is `UNK`. Shape :math:`(N_{res})` .
+          `common.residue_constants_restype_order`, :math:`[0,20]` . 20 means the amino acid is `UNK`.
+          Shape :math:`(N_{res}, )` .
         - all_atom_positions, numpy.array. Coordinates of all residues in pdb. Shape :math:`(N_{res}, 37)` .
         - all_atom_mask, numpy.array. Mask of atoms in pdb. Shape :math:`(N_{res}, 37)` .
           0 means the atom inexistence.
         - atom14_atom_exists, numpy.array. Densely encoding, mask of all atoms in protein.
           The position with atoms is 1 and the position without atoms is 0. Shape is :math:`(N_{res}, 14)`.
         - atom14_gt_exists, numpy.array. Densely encoding, mask of all atoms in protein.
           Keep the same as `atom14_atom_exist`. Shape is :math:`(N_{res}, 14)`.
@@ -595,14 +596,15 @@
         - atom14_alt_gt_exists, numpy.array. Densely encoding, mask of all atoms in chiral proteins.
           Shape is :math:`(N_{res}, 14)` .
         - atom14_atom_is_ambiguous, numpy.array. Because of the local symmetry of some amino acid structures,
           the symmetric atomic codes can be transposed. Specific atoms can be found in
           `common.residue_atom_renaming_swaps`. This feature records the uncertain atom encoding positions.
           Shape is :math:`(N_{res}, 14)` .
         - residue_index, numpy.array. Residue index information of protein sequence, ranging from 1 to :math:`N_{res}` .
+          Shape is :math:`(N_{res}, )` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindsponge.common import get_pdb_info
         >>> pdb_path = "YOUR PDB PATH"
```

## mindsponge/data/data_transform.py

```diff
@@ -1,908 +1,1139 @@
-# Copyright 2021 The AIMM Group at Shenzhen Bay Laboratory & Peking University & Huawei Technologies Co., Ltd
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""data transform MSA TEMPLATE"""
-import numpy as np
-import mindsponge.common.geometry as geometry
-from mindsponge.common.residue_constants import chi_angles_mask, chi_pi_periodic, restype_1to3, chi_angles_atoms, \
-    atom_order, residue_atom_renaming_swaps, restype_3to1, MAP_HHBLITS_AATYPE_TO_OUR_AATYPE, restype_order, \
-    restypes, restype_name_to_atom14_names, atom_types, residue_atoms, STANDARD_ATOM_MASK, restypes_with_x_and_gap, \
-    MSA_PAD_VALUES
-
-MS_MIN32 = -2147483648
-MS_MAX32 = 2147483647
-
-
-def one_hot(depth, indices):
-    """one hot compute"""
-    res = np.eye(depth)[indices.reshape(-1)]
-    return res.reshape(list(indices.shape) + [depth])
-
-
-def correct_msa_restypes(msa, deletion_matrix=None, is_evogen=False):
-    """Correct MSA restype to have the same order as residue_constants."""
-    new_order_list = MAP_HHBLITS_AATYPE_TO_OUR_AATYPE
-    new_order = np.array(new_order_list, dtype=msa.dtype)
-    msa = new_order[msa]
-    if is_evogen:
-        msa_input = np.concatenate((msa, deletion_matrix), axis=-1).astype(np.int32)
-        result = msa, msa_input
-    else:
-        result = msa
-    return result
-
-
-def randomly_replace_msa_with_unknown(msa, aatype, replace_proportion):
-    """Replace a proportion of the MSA with 'X'."""
-    msa_mask = np.random.uniform(size=msa.shape, low=0, high=1) < replace_proportion
-    x_idx = 20
-    gap_idx = 21
-    msa_mask = np.logical_and(msa_mask, msa != gap_idx)
-    msa = np.where(msa_mask, np.ones_like(msa) * x_idx, msa)
-    aatype_mask = np.random.uniform(size=aatype.shape, low=0, high=1) < replace_proportion
-    aatype = np.where(aatype_mask, np.ones_like(aatype) * x_idx, aatype)
-    return msa, aatype
-
-
-def fix_templates_aatype(template_aatype):
-    """Fixes aatype encoding of templates."""
-    # Map one-hot to indices.
-    template_aatype = np.argmax(template_aatype, axis=-1).astype(np.int32)
-    # Map hhsearch-aatype to our aatype.
-    new_order_list = MAP_HHBLITS_AATYPE_TO_OUR_AATYPE
-    new_order = np.array(new_order_list, np.int32)
-    template_aatype = new_order[template_aatype]
-    return template_aatype
-
-
-def pseudo_beta_fn(aatype, all_atom_positions, all_atom_masks):
-    """compute pseudo beta features from atom positions"""
-    is_gly = np.equal(aatype, restype_order['G'])
-    ca_idx = atom_order['CA']
-    cb_idx = atom_order['CB']
-    pseudo_beta = np.where(
-        np.tile(is_gly[..., None].astype("int32"), [1] * len(is_gly.shape) + [3]).astype("bool"),
-        all_atom_positions[..., ca_idx, :],
-        all_atom_positions[..., cb_idx, :])
-    if all_atom_masks is not None:
-        pseudo_beta_mask = np.where(is_gly, all_atom_masks[..., ca_idx], all_atom_masks[..., cb_idx])
-        pseudo_beta_mask = pseudo_beta_mask.astype(np.float32)
-        return pseudo_beta, pseudo_beta_mask
-    return pseudo_beta
-
-
-def make_atom14_masks(aatype):
-    """create atom 14 position features from aatype"""
-    rt_atom14_to_atom37 = []
-    rt_atom37_to_atom14 = []
-    rt_atom14_mask = []
-
-    for restype in restypes:
-        atom_names = restype_name_to_atom14_names.get(restype_1to3.get(restype))
-
-        rt_atom14_to_atom37.append([(atom_order[name] if name else 0) for name in atom_names])
-
-        atom_name_to_idx14 = {name: i for i, name in enumerate(atom_names)}
-        rt_atom37_to_atom14.append([(atom_name_to_idx14[name] if name in atom_name_to_idx14 else 0)
-                                    for name in atom_types])
-
-        rt_atom14_mask.append([(1. if name else 0.) for name in atom_names])
-
-    # Add dummy mapping for restype 'UNK'
-    rt_atom14_to_atom37.append([0] * 14)
-    rt_atom37_to_atom14.append([0] * 37)
-    rt_atom14_mask.append([0.] * 14)
-
-    rt_atom14_to_atom37 = np.array(rt_atom14_to_atom37, np.int32)
-    rt_atom37_to_atom14 = np.array(rt_atom37_to_atom14, np.int32)
-    rt_atom14_mask = np.array(rt_atom14_mask, np.float32)
-
-    ri_atom14_to_atom37 = rt_atom14_to_atom37[aatype]
-    ri_atom14_mask = rt_atom14_mask[aatype]
-
-    atom14_atom_exists = ri_atom14_mask
-    ri_atom14_to_atom37 = ri_atom14_to_atom37
-
-    # create the gather indices for mapping back
-    ri_atom37_to_atom14 = rt_atom37_to_atom14[aatype]
-    ri_atom37_to_atom14 = ri_atom37_to_atom14
-
-    # create the corresponding mask
-    restype_atom37_mask = np.zeros([21, 37], np.float32)
-    for restype, restype_letter in enumerate(restypes):
-        restype_name = restype_1to3.get(restype_letter)
-        atom_names = residue_atoms.get(restype_name)
-        for atom_name in atom_names:
-            atom_type = atom_order[atom_name]
-            restype_atom37_mask[restype, atom_type] = 1
-
-    atom37_atom_exists = restype_atom37_mask[aatype]
-    res = [atom14_atom_exists, ri_atom14_to_atom37, ri_atom37_to_atom14, atom37_atom_exists]
-    return res
-
-
-def block_delete_msa_indices(msa, msa_fraction_per_block, randomize_num_blocks, num_blocks):
-    """Sample MSA by deleting contiguous blocks.
-
-    Jumper et al. (2021) Suppl. Alg. 1 "MSABlockDeletion"
-
-    Arguments:
-    protein: batch dict containing the msa
-    config: ConfigDict with parameters
-
-    Returns:
-    updated protein
-    """
-
-    num_seq = msa.shape[0]
-    block_num_seq = np.floor(num_seq * msa_fraction_per_block).astype(np.int32)
-
-    if randomize_num_blocks:
-        nb = int(np.random.uniform(0, num_blocks + 1))
-    else:
-        nb = num_blocks
-    del_block_starts = np.random.uniform(0, num_seq, nb).astype(np.int32)
-    del_blocks = del_block_starts[:, None] + np.array([_ for _ in range(block_num_seq)]).astype(np.int32)
-    del_blocks = np.clip(del_blocks, 0, num_seq - 1)
-    del_indices = np.unique(np.sort(np.reshape(del_blocks, (-1,))))
-
-    # Make sure we keep the original sequence
-    keep_indices = np.setdiff1d(np.array([_ for _ in range(1, num_seq)]),
-                                del_indices)
-    keep_indices = np.concatenate([[0], keep_indices], axis=0)
-    keep_indices = [int(x) for x in keep_indices]
-    return keep_indices
-
-
-def sample_msa(msa, max_seq):
-    """Sample MSA randomly, remaining sequences are stored as `extra_*`."""
-    num_seq = msa.shape[0]
-
-    shuffled = list(range(1, num_seq))
-    np.random.shuffle(shuffled)
-    shuffled.insert(0, 0)
-    index_order = np.array(shuffled, np.int32)
-    num_sel = min(max_seq, num_seq)
-
-    sel_seq = index_order[:num_sel]
-    not_sel_seq = index_order[num_sel:]
-    is_sel = num_seq - num_sel
-    return is_sel, not_sel_seq, sel_seq
-
-
-def shape_list(x):
-    """get the list of dimensions of an array"""
-    x = np.array(x)
-    if x.ndim is None:
-        return x.shape
-
-    static = x.shape
-    ret = []
-    for _, dimension in enumerate(static):
-        ret.append(dimension)
-    return ret
-
-
-def shaped_categorical(probability):
-    """get categorical shape"""
-    ds = shape_list(probability)
-    num_classes = ds[-1]
-    flat_probs = np.reshape(probability, (-1, num_classes))
-    numbers = list(range(num_classes))
-    res = []
-    for flat_prob in flat_probs:
-        res.append(np.random.choice(numbers, p=flat_prob))
-    return np.reshape(np.array(res, np.int32), ds[:-1])
-
-
-def make_masked_msa(msa, hhblits_profile, uniform_prob, profile_prob, same_prob, replace_fraction, residue_index=None,
-                    msa_mask=None, is_evogen=False):
-    """create masked msa for BERT on raw MSA features"""
-
-    random_aatype = np.array([0.05] * 20 + [0., 0.], dtype=np.float32)
-
-    probability = uniform_prob * random_aatype + profile_prob * hhblits_profile + same_prob * one_hot(22, msa)
-
-    pad_shapes = [[0, 0] for _ in range(len(probability.shape))]
-    pad_shapes[-1][1] = 1
-    mask_prob = 1. - profile_prob - same_prob - uniform_prob
-
-    probability = np.pad(probability, pad_shapes, constant_values=(mask_prob,))
-
-    masked_aatype = np.random.uniform(size=msa.shape, low=0, high=1) < replace_fraction
-
-    bert_msa = shaped_categorical(probability)
-    bert_msa = np.where(masked_aatype, bert_msa, msa)
-
-    bert_mask = masked_aatype.astype(np.int32)
-    true_msa = msa
-    msa = bert_msa
-    if is_evogen:
-        additional_input = np.concatenate((bert_msa[0][:, None], np.asarray(residue_index)[:, None],
-                                           msa_mask[0][:, None],
-                                           bert_mask[0][:, None]),
-                                          axis=-1).astype(np.int32)
-        make_masked_msa_result = bert_mask, true_msa, msa, additional_input
-
-    else:
-        make_masked_msa_result = bert_mask, true_msa, msa
-    return make_masked_msa_result
-
-
-def nearest_neighbor_clusters(msa_mask, msa, extra_msa_mask, extra_msa, gap_agreement_weight=0.):
-    """Assign each extra MSA sequence to its nearest neighbor in sampled MSA."""
-
-    # Determine how much weight we assign to each agreement.  In theory, we could
-    # use a full blosum matrix here, but right now let's just down-weight gap
-    # agreement because it could be spurious.
-    # Never put weight on agreeing on BERT mask
-    weights = np.concatenate([np.ones(21), gap_agreement_weight * np.ones(1), np.zeros(1)], 0)
-
-    # Make agreement score as weighted Hamming distance
-    sample_one_hot = msa_mask[:, :, None] * one_hot(23, msa)
-    num_seq, num_res, _ = sample_one_hot.shape
-
-    array_extra_msa_mask = extra_msa_mask
-    if array_extra_msa_mask.any():
-        extra_one_hot = extra_msa_mask[:, :, None] * one_hot(23, extra_msa)
-        extra_num_seq, _, _ = extra_one_hot.shape
-
-        agreement = np.matmul(
-            np.reshape(extra_one_hot, [extra_num_seq, num_res * 23]),
-            np.reshape(sample_one_hot * weights, [num_seq, num_res * 23]).T)
-        # Assign each sequence in the extra sequences to the closest MSA sample
-        extra_cluster_assignment = np.argmax(agreement, axis=1)
-    else:
-        extra_cluster_assignment = np.array([])
-    return extra_cluster_assignment
-
-
-def summarize_clusters(msa, msa_mask, extra_cluster_assignment, extra_msa_mask, extra_msa, extra_deletion_matrix,
-                       deletion_matrix):
-    """Produce profile and deletion_matrix_mean within each cluster."""
-    num_seq = msa.shape[0]
-
-    def csum(x):
-        result = []
-        for i in range(num_seq):
-            result.append(np.sum(x[np.where(extra_cluster_assignment == i)], axis=0))
-        return np.array(result)
-
-    mask = extra_msa_mask
-    mask_counts = 1e-6 + msa_mask + csum(mask)  # Include center
-
-    msa_sum = csum(mask[:, :, None] * one_hot(23, extra_msa))
-    msa_sum += one_hot(23, msa)  # Original sequence
-    cluster_profile = msa_sum / mask_counts[:, :, None]
-
-    del msa_sum
-
-    del_sum = csum(mask * extra_deletion_matrix)
-    del_sum += deletion_matrix  # Original sequence
-    cluster_deletion_mean = del_sum / mask_counts
-    del del_sum
-
-    return cluster_profile, cluster_deletion_mean
-
-
-def crop_extra_msa(extra_msa, max_extra_msa):
-    """MSA features are cropped so only `max_extra_msa` sequences are kept."""
-    if extra_msa.any():
-        num_seq = extra_msa.shape[0]
-        num_sel = np.minimum(max_extra_msa, num_seq)
-        shuffled = list(range(num_seq))
-        np.random.shuffle(shuffled)
-        select_indices = shuffled[:num_sel]
-        return select_indices
-    return None
-
-
-def make_msa_feat(between_segment_residues, aatype, msa, deletion_matrix, cluster_deletion_mean, cluster_profile,
-                  extra_deletion_matrix):
-    """Create and concatenate MSA features."""
-    # Whether there is a domain break. Always zero for chains, but keeping
-    # for compatibility with domain datasets.
-    has_break = np.clip(between_segment_residues.astype(np.float32), np.array(0), np.array(1))
-    aatype_1hot = one_hot(21, aatype)
-
-    target_feat = [np.expand_dims(has_break, axis=-1), aatype_1hot]
-
-    msa_1hot = one_hot(23, msa)
-    has_deletion = np.clip(deletion_matrix, np.array(0), np.array(1))
-    deletion_value = np.arctan(deletion_matrix / 3.) * (2. / np.pi)
-
-    msa_feat = [msa_1hot, np.expand_dims(has_deletion, axis=-1), np.expand_dims(deletion_value, axis=-1)]
-
-    if cluster_profile is not None:
-        deletion_mean_value = (np.arctan(cluster_deletion_mean / 3.) * (2. / np.pi))
-        msa_feat.extend([cluster_profile, np.expand_dims(deletion_mean_value, axis=-1)])
-    extra_has_deletion = None
-    extra_deletion_value = None
-    if extra_deletion_matrix is not None:
-        extra_has_deletion = np.clip(extra_deletion_matrix, np.array(0), np.array(1))
-        extra_deletion_value = np.arctan(extra_deletion_matrix / 3.) * (2. / np.pi)
-
-    msa_feat = np.concatenate(msa_feat, axis=-1)
-    target_feat = np.concatenate(target_feat, axis=-1)
-    res = [extra_has_deletion, extra_deletion_value, msa_feat, target_feat]
-    return res
-
-
-def make_random_seed(size, seed_maker_t, low=MS_MIN32, high=MS_MAX32, random_recycle=False):
-    if random_recycle:
-        r = np.random.RandomState(seed_maker_t)
-        return r.uniform(size=size, low=low, high=high)
-    np.random.seed(seed_maker_t)
-    return np.random.uniform(size=size, low=low, high=high)
-
-
-def random_crop_to_size(seq_length, template_mask, crop_size, max_templates,
-                        subsample_templates=False, seed=0, random_recycle=False):
-    """Crop randomly to `crop_size`, or keep as is if shorter than that."""
-    seq_length = seq_length
-    seq_length_int = int(seq_length)
-    if template_mask is not None:
-        num_templates = np.array(template_mask.shape[0], np.int32)
-    else:
-        num_templates = np.array(0, np.int32)
-    num_res_crop_size = np.minimum(seq_length, crop_size)
-    num_res_crop_size_int = int(num_res_crop_size)
-
-    # Ensures that the cropping of residues and templates happens in the same way
-    # across ensembling iterations.
-    # Do not use for randomness that should vary in ensembling.
-
-    if subsample_templates:
-        templates_crop_start = int(make_random_seed(size=(), seed_maker_t=seed, low=0, high=num_templates + 1,
-                                                    random_recycle=random_recycle))
-    else:
-        templates_crop_start = 0
-
-    num_templates_crop_size = np.minimum(num_templates - templates_crop_start, max_templates)
-    num_templates_crop_size_int = int(num_templates_crop_size)
-
-    num_res_crop_start = int(make_random_seed(size=(), seed_maker_t=seed, low=0,
-                                              high=seq_length_int - num_res_crop_size_int + 1,
-                                              random_recycle=random_recycle))
-
-    templates_select_indices = np.argsort(make_random_seed(size=[num_templates], seed_maker_t=seed,
-                                                           random_recycle=random_recycle))
-    res = [num_res_crop_size, num_templates_crop_size_int, num_res_crop_start, num_res_crop_size_int, \
-           templates_crop_start, templates_select_indices]
-    return res
-
-
-def atom37_to_torsion_angles(
-        aatype: np.ndarray,
-        all_atom_pos: np.ndarray,
-        all_atom_mask: np.ndarray,
-        alt_torsions=False,
-):
-    r"""
-    This function calculates the seven torsion angles of each residue and encodes them in sine and cosine.
-    The order of the seven torsion angles is [pre_omega, phi, psi, chi_1, chi_2, chi_3, chi_4]
-    Here, pre_omega represents the twist angle between a given amino acid and the previous amino acid.
-    The phi represents twist angle between `C-CA-N-(C+1)`, psi represents twist angle between `(N-1)-C-CA-N`.
-
-    Args:
-        aatype (numpy.array):           Amino acid type with shape :math:`(batch\_size, N_{res})`.
-        all_atom_pos (numpy.array):     Atom37 representation of all atomic coordinates with
-                                        shape :math:`(batch\_size, N_{res}, 37, 3)`.
-        all_atom_mask (numpy.array):    Atom37 representation of the mask on all atomic coordinates with
-                                        shape :math:`(batch\_size, N_{res})`.
-        alt_torsions (bool):            Indicates whether to set the sign angle of shielding torsion to zero.
-                                        Default: False.
-
-    Returns:
-        Dict containing
-
-        - torsion_angles_sin_cos (numpy.array), with shape :math:`(batch\_size, N_{res}, 37, 3)` where
-          the final 2 dimensions denote sin and cos respectively.
-        - alt_torsion_angles_sin_cos (numpy.array), same as 'torsion_angles_sin_cos', but with the angle shifted
-          by pi for all chi angles affected by the naming ambiguities.
-        - torsion_angles_mask (numpy.array), Mask for which chi angles are present.
-
-    Supported Platforms:
-        ``Ascend`` ``GPU`` ``CPU``
-
-    Examples:
-        >>> import numpy as np
-        >>> from mindsponge.data.data_transform import atom37_to_torsion_angles
-        >>> n_res = 16
-        >>> bs = 1
-        >>> aatype = np.random.randn(bs, n_res).astype(np.int32)
-        >>> all_atom_pos = np.random.randn(bs, n_res, 37, 3).astype(np.float32)
-        >>> all_atom_mask = np.random.randn(bs, n_res, 37).astype(np.float32)
-        >>> angle_label_feature = atom37_to_torsion_angles(aatype, all_atom_pos, all_atom_mask)
-        >>> print(angle_label_feature.keys())
-        dict_keys(['torsion_angles_sin_cos', 'alt_torsion_angles_sin_cos', 'torsion_angles_mask'])
-    """
-
-    true_aatype = np.minimum(aatype, 20)
-
-    # get the number residue
-    num_batch, num_res = true_aatype.shape
-
-    paddings = np.zeros([num_batch, 1, 37, 3], np.float32)
-    padding_atom_pos = np.concatenate([paddings, all_atom_pos[:, :-1, :, :]], axis=1)
-
-    paddings = np.zeros([num_batch, 1, 37], np.float32)
-    padding_atom_mask = np.concatenate([paddings, all_atom_mask[:, :-1, :]], axis=1)
-
-    # compute padding atom position for omega, phi and psi
-    omega_atom_pos_padding = np.concatenate(
-        [padding_atom_pos[..., 1:3, :],
-         all_atom_pos[..., 0:2, :]
-         ], axis=-2)
-    phi_atom_pos_padding = np.concatenate(
-        [padding_atom_pos[..., 2:3, :],
-         all_atom_pos[..., 0:3, :]
-         ], axis=-2)
-    psi_atom_pos_padding = np.concatenate(
-        [all_atom_pos[..., 0:3, :],
-         all_atom_pos[..., 4:5, :]
-         ], axis=-2)
-
-    # compute padding atom position mask for omega, phi and psi
-    omega_mask_padding = (np.prod(padding_atom_mask[..., 1:3], axis=-1) *
-                          np.prod(all_atom_mask[..., 0:2], axis=-1))
-    phi_mask_padding = (padding_atom_mask[..., 2] * np.prod(all_atom_mask[..., 0:3], axis=-1))
-    psi_mask_padding = (np.prod(all_atom_mask[..., 0:3], axis=-1) * all_atom_mask[..., 4])
-
-    chi_atom_pos_indices = get_chi_atom_pos_indices()
-    atom_pos_indices = np_gather_ops(chi_atom_pos_indices, true_aatype, 0, 0)
-    chi_atom_pos = np_gather_ops(all_atom_pos, atom_pos_indices, -2, 2)
-
-    angles_mask = list(chi_angles_mask)
-    angles_mask.append([0.0, 0.0, 0.0, 0.0])
-    angles_mask = np.array(angles_mask)
-
-    chis_mask = np_gather_ops(angles_mask, true_aatype, 0, 0)
-
-    chi_angle_atoms_mask = np_gather_ops(all_atom_mask, atom_pos_indices, -1, 2)
-
-    chi_angle_atoms_mask = np.prod(chi_angle_atoms_mask, axis=-1)
-    chis_mask = chis_mask * chi_angle_atoms_mask.astype(np.float32)
-
-    torsions_atom_pos_padding = np.concatenate(
-        [omega_atom_pos_padding[:, :, None, :, :],
-         phi_atom_pos_padding[:, :, None, :, :],
-         psi_atom_pos_padding[:, :, None, :, :],
-         chi_atom_pos
-         ], axis=2)
-
-    torsion_angles_mask_padding = np.concatenate(
-        [omega_mask_padding[:, :, None],
-         phi_mask_padding[:, :, None],
-         psi_mask_padding[:, :, None],
-         chis_mask
-         ], axis=2)
-
-    torsion_frames = geometry.rigids_from_3_points(
-        point_on_neg_x_axis=geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 1, :]),
-        origin=geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 2, :]),
-        point_on_xy_plane=geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 0, :]))
-    inv_torsion_frames = geometry.invert_rigids(torsion_frames)
-    vecs = geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 3, :])
-    forth_atom_rel_pos = geometry.rigids_mul_vecs(inv_torsion_frames, vecs)
-
-    torsion_angles_sin_cos = np.stack(
-        [forth_atom_rel_pos[2], forth_atom_rel_pos[1]], axis=-1)
-    torsion_angles_sin_cos /= np.sqrt(
-        np.sum(np.square(torsion_angles_sin_cos), axis=-1, keepdims=True)
-        + 1e-8)
-
-    torsion_angles_sin_cos *= np.array(
-        [1., 1., -1., 1., 1., 1., 1.])[None, None, :, None]
-
-    chi_is_ambiguous = np_gather_ops(
-        np.array(chi_pi_periodic), true_aatype)
-    mirror_torsion_angles = np.concatenate(
-        [np.ones([num_batch, num_res, 3]),
-         1.0 - 2.0 * chi_is_ambiguous], axis=-1)
-    alt_torsion_angles_sin_cos = (torsion_angles_sin_cos * mirror_torsion_angles[:, :, :, None])
-
-    if alt_torsions:
-        fix_torsions = np.stack([np.ones(torsion_angles_sin_cos.shape[:-1]),
-                                 np.zeros(torsion_angles_sin_cos.shape[:-1])], axis=-1)
-        torsion_angles_sin_cos = torsion_angles_sin_cos * torsion_angles_mask_padding[
-            ..., None] + fix_torsions * (1 - torsion_angles_mask_padding[..., None])
-        alt_torsion_angles_sin_cos = alt_torsion_angles_sin_cos * torsion_angles_mask_padding[
-            ..., None] + fix_torsions * (1 - torsion_angles_mask_padding[..., None])
-
-    return {
-        'torsion_angles_sin_cos': torsion_angles_sin_cos[0],  # (N, 7, 2)
-        'alt_torsion_angles_sin_cos': alt_torsion_angles_sin_cos[0],  # (N, 7, 2)
-        'torsion_angles_mask': torsion_angles_mask_padding[0]  # (N, 7)
-    }
-
-
-def atom37_to_frames(
-        aatype,
-        all_atom_positions,
-        all_atom_mask,
-        is_affine=False
-):
-    r"""
-    Computes the torsion angle of up to 8 rigid groups for each residue, shape is :math:`[N_{res}, 8, 12]`,
-    where 8 is indicates that each residue can be divided into up to 8 rigid groups according to the dependence of
-    the atom on the torsion angle, there are 1 backbone frame and 7 side-chain frames.
-    For the meaning of 12 ,the first 9 elements are the 9 components of rotation matrix, the last
-    3 elements are the 3 component of translation matrix.
-
-
-    Args:
-        aatype(numpy.array):                Amino acid sequence, :math:`[N_{res}]` .
-        all_atom_positions(numpy.array):    The coordinates of all atoms, presented as atom37, :math:`[N_{res}, 37,3]`.
-        all_atom_mask(numpy.array):         Mask of all atomic coordinates, :math:`[N_{res},37]`.
-        is_affine(bool):                    Whether to perform affine, the default value is False.
-
-    Returns:
-        Dictionary, the specific content is as follows.
-
-        - **rigidgroups_gt_frames** (numpy.array) - The torsion angle of the 8 rigid body groups for each residue,
-          :math:`[N_{res}, 8, 12]`.
-        - **rigidgroups_gt_exists** (numpy.array) - The mask of rigidgroups_gt_frames denoting whether the rigid body
-          group exists according to the experiment, :math:`[N_{res}, 8]`.
-        - **rigidgroups_group_exists** (numpy.array) - Mask denoting whether given group is in principle present
-          for given amino acid type, :math:`[N_{res}, 8]` .
-        - **rigidgroups_group_is_ambiguous** (numpy.array) - Indicates that the position is chiral symmetry,
-          :math:`[N_{res}, 8]` .
-        - **rigidgroups_alt_gt_frames** (numpy.array) - 8 Frames with alternative atom renaming
-          corresponding to 'all_atom_positions' represented as flat
-          12 dimensional array :math:`[N_{res}, 8, 12]` .
-        - **backbone_affine_tensor** (numpy.array) - The translation and rotation of the local coordinates of each
-          amino acid relative to the global coordinates, :math:`[N_{res}, 7]` , for the last dimension, the first 4
-          elements are the affine tensor which contains the rotation information, the last 3 elements are the
-          translations in space.
-
-    Supported Platforms:
-        ``Ascend`` ``GPU`` ``CPU``
-
-    Examples:
-        >>> import numpy as np
-        >>> from mindsponge.data import atom37_to_frames
-        >>> from mindspore import dtype as mstype
-        >>> from mindspore import Tensor
-        >>> aatype = np.ones(193,dtype=np.int32)
-        >>> all_atom_positions = np.ones((193,37,3),dtype=np.float32)
-        >>> all_atom_mask = np.ones((193,37),dtype=np.int32)
-        >>> result = atom37_to_frames(aatype,all_atom_positions,all_atom_mask)
-        >>> for key in result.keys():
-        >>>     print(key,result[key].shape)
-        rigidgroups_gt_frames (193, 8, 12)
-        rigidgroups_gt_exists (193, 8)
-        rigidgroups_group_exists (193, 8)
-        rigidgroups_group_is_ambiguous (193, 8)
-        rigidgroups_alt_gt_frames (193, 8, 12)
-    """
-    aatype_shape = aatype.shape
-
-    flat_aatype = np.reshape(aatype, [-1])
-    all_atom_positions = np.reshape(all_atom_positions, [-1, 37, 3])
-    all_atom_mask = np.reshape(all_atom_mask, [-1, 37])
-
-    rigid_group_names_res = np.full([21, 8, 3], '', dtype=object)
-
-    # group 0: backbone frame
-    rigid_group_names_res[:, 0, :] = ['C', 'CA', 'N']
-
-    # group 3: 'psi'
-    rigid_group_names_res[:, 3, :] = ['CA', 'C', 'O']
-
-    # group 4,5,6,7: 'chi1,2,3,4'
-    for restype, letter in enumerate(restypes):
-        restype_name = restype_1to3[letter]
-        for chi_idx in range(4):
-            if chi_angles_mask[restype][chi_idx]:
-                atom_names = chi_angles_atoms[restype_name][chi_idx]
-                rigid_group_names_res[restype, chi_idx + 4, :] = atom_names[1:]
-
-    # create rigid group mask
-    rigid_group_mask_res = np.zeros([21, 8], dtype=np.float32)
-    rigid_group_mask_res[:, 0] = 1
-    rigid_group_mask_res[:, 3] = 1
-    rigid_group_mask_res[:20, 4:] = chi_angles_mask
-
-    lookup_table = atom_order.copy()
-    lookup_table[''] = 0
-    rigid_group_atom37_idx_restype = np.vectorize(lambda x: lookup_table[x])(
-        rigid_group_names_res)
-
-    rigid_group_atom37_idx_residx = np_gather_ops(
-        rigid_group_atom37_idx_restype, flat_aatype)
-
-    base_atom_pos = np_gather_ops(
-        all_atom_positions,
-        rigid_group_atom37_idx_residx,
-        batch_dims=1)
-
-    gt_frames = geometry.rigids_from_3_points(
-        point_on_neg_x_axis=geometry.vecs_from_tensor(base_atom_pos[:, :, 0, :]),
-        origin=geometry.vecs_from_tensor(base_atom_pos[:, :, 1, :]),
-        point_on_xy_plane=geometry.vecs_from_tensor(base_atom_pos[:, :, 2, :]))
-
-    # get the group mask
-    group_masks = np_gather_ops(rigid_group_mask_res, flat_aatype)
-
-    # get the atom mask
-    gt_atoms_exists = np_gather_ops(
-        all_atom_mask.astype(np.float32),
-        rigid_group_atom37_idx_residx,
-        batch_dims=1)
-    gt_masks = np.min(gt_atoms_exists, axis=-1) * group_masks
-
-    rotations = np.tile(np.eye(3, dtype=np.float32), [8, 1, 1])
-    rotations[0, 0, 0] = -1
-    rotations[0, 2, 2] = -1
-    gt_frames = geometry.rigids_mul_rots(gt_frames, geometry.rots_from_tensor(rotations, use_numpy=True))
-
-    rigid_group_is_ambiguous_res = np.zeros([21, 8], dtype=np.float32)
-    rigid_group_rotations_res = np.tile(np.eye(3, dtype=np.float32), [21, 8, 1, 1])
-
-    for restype_name, _ in residue_atom_renaming_swaps.items():
-        restype = restype_order[restype_3to1[restype_name]]
-        chi_idx = int(sum(chi_angles_mask[restype]) - 1)
-        rigid_group_is_ambiguous_res[restype, chi_idx + 4] = 1
-        rigid_group_rotations_res[restype, chi_idx + 4, 1, 1] = -1
-        rigid_group_rotations_res[restype, chi_idx + 4, 2, 2] = -1
-
-    # Gather the ambiguity information for each residue.
-    rigid_group_is_ambiguous_res_index = np_gather_ops(
-        rigid_group_is_ambiguous_res, flat_aatype)
-    rigid_group_ambiguity_rotation_res_index = np_gather_ops(
-        rigid_group_rotations_res, flat_aatype)
-
-    # Create the alternative ground truth frames.
-    alt_gt_frames = geometry.rigids_mul_rots(
-        gt_frames, geometry.rots_from_tensor(rigid_group_ambiguity_rotation_res_index, use_numpy=True))
-
-    gt_frames_flat12 = np.stack(list(gt_frames[0]) + list(gt_frames[1]), axis=-1)
-    alt_gt_frames_flat12 = np.stack(list(alt_gt_frames[0]) + list(alt_gt_frames[1]), axis=-1)
-    # reshape back to original residue layout
-    gt_frames_flat12 = np.reshape(gt_frames_flat12, aatype_shape + (8, 12))
-    gt_masks = np.reshape(gt_masks, aatype_shape + (8,))
-    group_masks = np.reshape(group_masks, aatype_shape + (8,))
-    gt_frames_flat12 = np.reshape(gt_frames_flat12, aatype_shape + (8, 12))
-    rigid_group_is_ambiguous_res_index = np.reshape(rigid_group_is_ambiguous_res_index, aatype_shape + (8,))
-    alt_gt_frames_flat12 = np.reshape(alt_gt_frames_flat12,
-                                      aatype_shape + (8, 12,))
-    if not is_affine:
-        return {
-            'rigidgroups_gt_frames': gt_frames_flat12,  # shape (..., 8, 12)
-            'rigidgroups_gt_exists': gt_masks,  # shape (..., 8)
-            'rigidgroups_group_exists': group_masks,  # shape (..., 8)
-            'rigidgroups_group_is_ambiguous':
-                rigid_group_is_ambiguous_res_index,  # shape (..., 8)
-            'rigidgroups_alt_gt_frames': alt_gt_frames_flat12,  # shape (..., 8, 12)
-        }
-
-    rotation = [[gt_frames[0][0], gt_frames[0][1], gt_frames[0][2]],
-                [gt_frames[0][3], gt_frames[0][4], gt_frames[0][5]],
-                [gt_frames[0][6], gt_frames[0][7], gt_frames[0][8]]]
-    translation = [gt_frames[1][0], gt_frames[1][1], gt_frames[1][2]]
-    backbone_affine_tensor = to_tensor(rotation, translation)[:, 0, :]
-    return {
-        'rigidgroups_gt_frames': gt_frames_flat12,  # shape (..., 8, 12)
-        'rigidgroups_gt_exists': gt_masks,  # shape (..., 8)
-        'rigidgroups_group_exists': group_masks,  # shape (..., 8)
-        'rigidgroups_group_is_ambiguous': rigid_group_is_ambiguous_res_index,  # shape (..., 8)
-        'rigidgroups_alt_gt_frames': alt_gt_frames_flat12,  # shape (..., 8, 12)
-        'backbone_affine_tensor': backbone_affine_tensor,  # shape (..., 7)
-    }
-
-
-def get_chi_atom_pos_indices():
-    """get the atom indices for computing chi angles for all residue types"""
-    chi_atom_pos_indices = []
-    for residue_name in restypes:
-        residue_name = restype_1to3[residue_name]
-        residue_chi_angles = chi_angles_atoms[residue_name]
-        atom_pos_indices = []
-        for chi_angle in residue_chi_angles:
-            atom_pos_indices.append([atom_order[atom] for atom in chi_angle])
-        for _ in range(4 - len(atom_pos_indices)):
-            atom_pos_indices.append([0, 0, 0, 0])  # For chi angles not defined on the AA.
-        chi_atom_pos_indices.append(atom_pos_indices)
-
-    chi_atom_pos_indices.append([[0, 0, 0, 0]] * 4)  # For UNKNOWN residue.
-
-    return np.array(chi_atom_pos_indices)
-
-
-def gather(params, indices, axis=0):
-    """gather operation"""
-    func = lambda p, i: np.take(p, i, axis=axis)
-    return func(params, indices)
-
-
-def np_gather_ops(params, indices, axis=0, batch_dims=0):
-    """np gather operation"""
-    if batch_dims == 0:
-        return gather(params, indices)
-    result = []
-    if batch_dims == 1:
-        for p, i in zip(params, indices):
-            axis = axis - batch_dims if axis - batch_dims > 0 else 0
-            r = gather(p, i, axis=axis)
-            result.append(r)
-        return np.stack(result)
-    for p, i in zip(params[0], indices[0]):
-        r = gather(p, i, axis=axis)
-        result.append(r)
-    res = np.stack(result)
-    return res.reshape((1,) + res.shape)
-
-
-def rot_to_quat(rot, unstack_inputs=False):
-    """transfer the rotation matrix to quaternion matrix"""
-    if unstack_inputs:
-        rot = [np.moveaxis(x, -1, 0) for x in np.moveaxis(rot, -2, 0)]
-    [[xx, xy, xz], [yx, yy, yz], [zx, zy, zz]] = rot
-
-    k = [[xx + yy + zz, zy - yz, xz - zx, yx - xy],
-         [zy - yz, xx - yy - zz, xy + yx, xz + zx],
-         [xz - zx, xy + yx, yy - xx - zz, yz + zy],
-         [yx - xy, xz + zx, yz + zy, zz - xx - yy]]
-
-    k = (1. / 3.) * np.stack([np.stack(x, axis=-1) for x in k],
-                             axis=-2)
-
-    # compute eigenvalues
-    _, qs = np.linalg.eigh(k)
-    return qs[..., -1]
-
-
-def to_tensor(rotation, translation):
-    """get affine based on rotation and translation"""
-    quaternion = rot_to_quat(rotation)
-    return np.concatenate(
-        [quaternion] +
-        [np.expand_dims(x, axis=-1) for x in translation],
-        axis=-1)
-
-
-def convert_monomer_features(chain_id, aatype, template_aatype):
-    """Reshapes and modifies monomer features for multimer models."""
-
-    auth_chain_id = np.asarray(chain_id, dtype=np.object_)
-    new_order_list = MAP_HHBLITS_AATYPE_TO_OUR_AATYPE
-    monomer_aatype = np.argmax(aatype, axis=-1).astype(np.int32)
-    monomer_template_aatype = np.argmax(template_aatype, axis=-1).astype(np.int32)
-    monomer_template_aatype = np.take(new_order_list, monomer_template_aatype.astype(np.int32), axis=0)
-
-    return auth_chain_id, monomer_aatype, monomer_template_aatype
-
-
-def convert_unnecessary_leading_dim_feats(sequence, domain_name, num_alignments, seq_length):
-    """get first dimension data of unnecessary features."""
-
-    monomer_sequence = np.asarray(sequence[0], dtype=sequence.dtype)
-    monomer_domain_name = np.asarray(domain_name[0], dtype=domain_name.dtype)
-    monomer_num_alignments = np.asarray(num_alignments[0], dtype=num_alignments.dtype)
-    monomer_seq_length = np.asarray(seq_length[0], dtype=seq_length.dtype)
-
-    converted_feature = (monomer_sequence, monomer_domain_name, monomer_num_alignments, monomer_seq_length)
-    return converted_feature
-
-
-def process_unmerged_features(deletion_matrix_int, deletion_matrix_int_all_seq, aatype, entity_id, num_chains):
-    """Postprocessing stage for per-chain features before merging."""
-    # Convert deletion matrices to float.
-    deletion_matrix = np.asarray(deletion_matrix_int, dtype=np.float32)
-    deletion_matrix_all_seq = np.asarray(deletion_matrix_int_all_seq, dtype=np.float32)
-
-    all_atom_mask = STANDARD_ATOM_MASK[aatype]
-    all_atom_mask = all_atom_mask
-    all_atom_positions = np.zeros(list(all_atom_mask.shape) + [3])
-    deletion_mean = np.mean(deletion_matrix, axis=0)
-
-    # Add assembly_num_chains.
-    assembly_num_chains = np.asarray(num_chains)
-    entity_mask = (entity_id != 0).astype(np.int32)
-    post_feature = (deletion_matrix, deletion_matrix_all_seq, deletion_mean, all_atom_mask, all_atom_positions,
-                    assembly_num_chains, entity_mask)
-
-    return post_feature
-
-
-def get_crop_size(num_alignments_all_seq, msa_all_seq, msa_crop_size, msa_size):
-    """get maximum msa crop size
-
-    Args:
-        num_alignments_all_seq: num_alignments for all sequence, which record the total number of msa
-        msa_all_seq: un-paired sequences for all msa.
-        msa_crop_size: The total number of sequences to crop from the MSA.
-        msa_size: number of msa
-
-    Returns:
-        msa_crop_size: msa sized to be cropped
-        msa_crop_size_all_seq: msa_crop_size for features with "_all_seq"
-
-    """
-
-    msa_size_all_seq = num_alignments_all_seq
-    msa_crop_size_all_seq = np.minimum(msa_size_all_seq, msa_crop_size // 2)
-
-    # We reduce the number of un-paired sequences, by the number of times a
-    # sequence from this chain's MSA is included in the paired MSA.  This keeps
-    # the MSA size for each chain roughly constant.
-    msa_all_seq = msa_all_seq[:msa_crop_size_all_seq, :]
-    num_non_gapped_pairs = np.sum(np.any(msa_all_seq != restypes_with_x_and_gap.index('-'), axis=1))
-    num_non_gapped_pairs = np.minimum(num_non_gapped_pairs, msa_crop_size_all_seq)
-
-    # Restrict the unpaired crop size so that paired+unpaired sequences do not
-    # exceed msa_seqs_per_chain for each chain.
-    max_msa_crop_size = np.maximum(msa_crop_size - num_non_gapped_pairs, 0)
-    msa_crop_size = np.minimum(msa_size, max_msa_crop_size)
-    return msa_crop_size, msa_crop_size_all_seq
-
-
-def make_seq_mask(entity_id):
-    """seq mask info, True for entity_id > 0, False for entity_id <= 0."""
-
-    seq_mask = (entity_id > 0).astype(np.float32)
-    return seq_mask
-
-
-def make_msa_mask(msa, entity_id):
-    """Mask features are all ones, but will later be zero-padded."""
-
-    msa_mask = np.ones_like(msa, dtype=np.float32)
-
-    seq_mask = (entity_id > 0).astype(np.float32)
-    msa_mask *= seq_mask[None]
-
-    return msa_mask
-
-
-def add_padding(feature_name, feature):
-    """get padding data with specified shapes of feature"""
-
-    num_res = feature.shape[1]
-    padding = MSA_PAD_VALUES.get(feature_name) * np.ones([1, num_res], feature.dtype)
-    return padding
-
-
-def generate_random_sample(cfg, model_config):
-    '''generate_random_sample'''
-    np.random.seed(0)
-    num_noise = model_config.model.latent.num_noise
-    latent_dim = model_config.model.latent.latent_dim
-
-    context_true_prob = np.absolute(model_config.train.context_true_prob)
-    keep_prob = np.absolute(model_config.train.keep_prob)
-
-    available_msa = int(model_config.train.available_msa_fraction * model_config.train.max_msa_clusters)
-    available_msa = min(available_msa, model_config.train.max_msa_clusters)
-
-    evogen_random_data = np.random.normal(
-        size=(num_noise, model_config.train.max_msa_clusters, cfg.eval.crop_size, latent_dim)).astype(np.float32)
-
-    # (Nseq,):
-    context_mask = np.zeros((model_config.train.max_msa_clusters,), np.int32)
-    z1 = np.random.random(model_config.train.max_msa_clusters)
-    context_mask = np.asarray([1 if x < context_true_prob else 0 for x in z1], np.int32)
-    context_mask[available_msa:] *= 0
-
-    # (Nseq,):
-    target_mask = np.zeros((model_config.train.max_msa_clusters,), np.int32)
-    z2 = np.random.random(model_config.train.max_msa_clusters)
-    target_mask = np.asarray([1 if x < keep_prob else 0 for x in z2], np.int32)
-
-    context_mask[0] = 1
-    target_mask[0] = 1
-
-    evogen_context_mask = np.stack((context_mask, target_mask), -1)
-    return evogen_random_data, evogen_context_mask
+# Copyright 2021 The AIMM Group at Shenzhen Bay Laboratory & Peking University & Huawei Technologies Co., Ltd
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""data transform MSA TEMPLATE"""
+import numpy as np
+from scipy.special import softmax
+import mindsponge.common.geometry as geometry
+from mindsponge.common.residue_constants import chi_angles_mask, chi_pi_periodic, restype_1to3, chi_angles_atoms, \
+    atom_order, residue_atom_renaming_swaps, restype_3to1, MAP_HHBLITS_AATYPE_TO_OUR_AATYPE, restype_order, \
+    restypes, restype_name_to_atom14_names, atom_types, residue_atoms, STANDARD_ATOM_MASK, restypes_with_x_and_gap, \
+    MSA_PAD_VALUES
+
+MS_MIN32 = -2147483648
+MS_MAX32 = 2147483647
+
+
+def one_hot(depth, indices):
+    """one hot compute"""
+    res = np.eye(depth)[indices.reshape(-1)]
+    return res.reshape(list(indices.shape) + [depth])
+
+
+def correct_msa_restypes(msa, deletion_matrix=None, is_evogen=False):
+    """Correct MSA restype to have the same order as residue_constants."""
+    new_order_list = MAP_HHBLITS_AATYPE_TO_OUR_AATYPE
+    new_order = np.array(new_order_list, dtype=msa.dtype)
+    msa = new_order[msa]
+    if is_evogen:
+        msa_input = np.concatenate((msa, deletion_matrix), axis=-1).astype(np.int32)
+        result = msa, msa_input
+    else:
+        result = msa
+    return result
+
+
+def randomly_replace_msa_with_unknown(msa, aatype, replace_proportion):
+    """Replace a proportion of the MSA with 'X'."""
+    msa_mask = np.random.uniform(size=msa.shape, low=0, high=1) < replace_proportion
+    x_idx = 20
+    gap_idx = 21
+    msa_mask = np.logical_and(msa_mask, msa != gap_idx)
+    msa = np.where(msa_mask, np.ones_like(msa) * x_idx, msa)
+    aatype_mask = np.random.uniform(size=aatype.shape, low=0, high=1) < replace_proportion
+    aatype = np.where(aatype_mask, np.ones_like(aatype) * x_idx, aatype)
+    return msa, aatype
+
+
+def fix_templates_aatype(template_aatype):
+    """Fixes aatype encoding of templates."""
+    # Map one-hot to indices.
+    template_aatype = np.argmax(template_aatype, axis=-1).astype(np.int32)
+    # Map hhsearch-aatype to our aatype.
+    new_order_list = MAP_HHBLITS_AATYPE_TO_OUR_AATYPE
+    new_order = np.array(new_order_list, np.int32)
+    template_aatype = new_order[template_aatype]
+    return template_aatype
+
+
+def pseudo_beta_fn(aatype, all_atom_positions, all_atom_masks):
+    """compute pseudo beta features from atom positions"""
+    is_gly = np.equal(aatype, restype_order['G'])
+    ca_idx = atom_order['CA']
+    cb_idx = atom_order['CB']
+    pseudo_beta = np.where(
+        np.tile(is_gly[..., None].astype("int32"), [1] * len(is_gly.shape) + [3]).astype("bool"),
+        all_atom_positions[..., ca_idx, :],
+        all_atom_positions[..., cb_idx, :])
+    if all_atom_masks is not None:
+        pseudo_beta_mask = np.where(is_gly, all_atom_masks[..., ca_idx], all_atom_masks[..., cb_idx])
+        pseudo_beta_mask = pseudo_beta_mask.astype(np.float32)
+        return pseudo_beta, pseudo_beta_mask
+    return pseudo_beta
+
+
+def make_atom14_masks(aatype):
+    """create atom 14 position features from aatype"""
+    rt_atom14_to_atom37 = []
+    rt_atom37_to_atom14 = []
+    rt_atom14_mask = []
+
+    for restype in restypes:
+        atom_names = restype_name_to_atom14_names.get(restype_1to3.get(restype))
+
+        rt_atom14_to_atom37.append([(atom_order[name] if name else 0) for name in atom_names])
+
+        atom_name_to_idx14 = {name: i for i, name in enumerate(atom_names)}
+        rt_atom37_to_atom14.append([(atom_name_to_idx14[name] if name in atom_name_to_idx14 else 0)
+                                    for name in atom_types])
+
+        rt_atom14_mask.append([(1. if name else 0.) for name in atom_names])
+
+    # Add dummy mapping for restype 'UNK'
+    rt_atom14_to_atom37.append([0] * 14)
+    rt_atom37_to_atom14.append([0] * 37)
+    rt_atom14_mask.append([0.] * 14)
+
+    rt_atom14_to_atom37 = np.array(rt_atom14_to_atom37, np.int32)
+    rt_atom37_to_atom14 = np.array(rt_atom37_to_atom14, np.int32)
+    rt_atom14_mask = np.array(rt_atom14_mask, np.float32)
+
+    ri_atom14_to_atom37 = rt_atom14_to_atom37[aatype]
+    ri_atom14_mask = rt_atom14_mask[aatype]
+
+    atom14_atom_exists = ri_atom14_mask
+    ri_atom14_to_atom37 = ri_atom14_to_atom37
+
+    # create the gather indices for mapping back
+    ri_atom37_to_atom14 = rt_atom37_to_atom14[aatype]
+    ri_atom37_to_atom14 = ri_atom37_to_atom14
+
+    # create the corresponding mask
+    restype_atom37_mask = np.zeros([21, 37], np.float32)
+    for restype, restype_letter in enumerate(restypes):
+        restype_name = restype_1to3.get(restype_letter)
+        atom_names = residue_atoms.get(restype_name)
+        for atom_name in atom_names:
+            atom_type = atom_order[atom_name]
+            restype_atom37_mask[restype, atom_type] = 1
+
+    atom37_atom_exists = restype_atom37_mask[aatype]
+    res = [atom14_atom_exists, ri_atom14_to_atom37, ri_atom37_to_atom14, atom37_atom_exists]
+    return res
+
+
+def block_delete_msa_indices(msa, msa_fraction_per_block, randomize_num_blocks, num_blocks):
+    """Sample MSA by deleting contiguous blocks.
+
+    Jumper et al. (2021) Suppl. Alg. 1 "MSABlockDeletion"
+
+    Arguments:
+    protein: batch dict containing the msa
+    config: ConfigDict with parameters
+
+    Returns:
+    updated protein
+    """
+
+    num_seq = msa.shape[0]
+    block_num_seq = np.floor(num_seq * msa_fraction_per_block).astype(np.int32)
+
+    if randomize_num_blocks:
+        nb = int(np.random.uniform(0, num_blocks + 1))
+    else:
+        nb = num_blocks
+    del_block_starts = np.random.uniform(0, num_seq, nb).astype(np.int32)
+    del_blocks = del_block_starts[:, None] + np.array([_ for _ in range(block_num_seq)]).astype(np.int32)
+    del_blocks = np.clip(del_blocks, 0, num_seq - 1)
+    del_indices = np.unique(np.sort(np.reshape(del_blocks, (-1,))))
+
+    # Make sure we keep the original sequence
+    keep_indices = np.setdiff1d(np.array([_ for _ in range(1, num_seq)]),
+                                del_indices)
+    keep_indices = np.concatenate([[0], keep_indices], axis=0)
+    keep_indices = [int(x) for x in keep_indices]
+    return keep_indices
+
+
+def sample_msa(msa, max_seq):
+    """Sample MSA randomly, remaining sequences are stored as `extra_*`."""
+    num_seq = msa.shape[0]
+
+    shuffled = list(range(1, num_seq))
+    np.random.shuffle(shuffled)
+    shuffled.insert(0, 0)
+    index_order = np.array(shuffled, np.int32)
+    num_sel = min(max_seq, num_seq)
+
+    sel_seq = index_order[:num_sel]
+    not_sel_seq = index_order[num_sel:]
+    is_sel = num_seq - num_sel
+    return is_sel, not_sel_seq, sel_seq
+
+
+def gumbel_noise(shape):
+    """Generate Gumbel Noise of given Shape."""
+    epsilon = 1e-6
+    uniform_noise = np.random.uniform(0, 1, shape)
+    gumbel = -np.log(-np.log(uniform_noise + epsilon) + epsilon)
+    return gumbel
+
+
+def gumbel_argsort_sample_idx(logits):
+    """Samples with replacement from a distribution given by 'logits'."""
+    z = gumbel_noise(logits.shape)
+    return np.argsort(logits + z, axis=-1)[..., ::-1]
+
+
+def gumbel_permutation(msa_mask, msa_chains=None):
+    """gumbel permutation."""
+    has_msa = np.sum(msa_mask, axis=-1) > 0
+    # default logits is zero
+    logits = np.zeros_like(has_msa, dtype=np.float32)
+    logits[~has_msa] = -1e6
+    # one sample only
+    assert len(logits.shape) == 1
+    # skip first row
+    logits = logits[1:]
+    has_msa = has_msa[1:]
+    if logits.shape[0] == 0:
+        return np.array([0])
+    if msa_chains is not None:
+        # skip first row
+        msa_chains = msa_chains[1:].reshape(-1)
+        msa_chains[~has_msa] = 0
+        keys, _ = np.unique(msa_chains, return_counts=True)
+        num_has_msa = np.array(has_msa.sum())
+        num_pair = np.array((msa_chains == 1).sum())
+        num_unpair = num_has_msa - num_pair
+        num_chains = np.array((keys > 1).sum())
+        logits[has_msa] = 1.0 / (num_has_msa + 1e-6)
+        logits[~has_msa] = 0
+        for k in keys:
+            if k > 1:
+                cur_mask = msa_chains == k
+                cur_cnt = np.array(cur_mask.sum())
+                if cur_cnt > 0:
+                    logits[cur_mask] *= num_unpair / (num_chains * cur_cnt)
+        logits = np.log(logits + 1e-6)
+    shuffled = gumbel_argsort_sample_idx(logits) + 1
+    return np.concatenate((np.array([0]), shuffled), axis=0)
+
+
+def sample_msa_v2(msa, msa_chains, msa_mask, max_seq, biased_msa_by_chain=False):
+    """Sample MSA randomly in multimer, remaining sequences are stored as `extra_*`."""
+    num_seq = msa.shape[0]
+    num_sel = min(max_seq, num_seq)
+    msa_chain = (msa_chains if biased_msa_by_chain else None)
+    index_order = gumbel_permutation(msa_mask, msa_chain)
+    num_sel = min(max_seq, num_seq)
+    sel_seq = index_order[:num_sel]
+    not_sel_seq = index_order[num_sel:]
+    is_sel = num_seq - num_sel
+    return is_sel, not_sel_seq, sel_seq
+
+
+def shape_list(x):
+    """get the list of dimensions of an array"""
+    x = np.array(x)
+    if x.ndim is None:
+        return x.shape
+
+    static = x.shape
+    ret = []
+    for _, dimension in enumerate(static):
+        ret.append(dimension)
+    return ret
+
+
+def shaped_categorical(probability):
+    """get categorical shape"""
+    ds = shape_list(probability)
+    num_classes = ds[-1]
+    flat_probs = np.reshape(probability, (-1, num_classes))
+    numbers = list(range(num_classes))
+    res = []
+    for flat_prob in flat_probs:
+        res.append(np.random.choice(numbers, p=flat_prob))
+    return np.reshape(np.array(res, np.int32), ds[:-1])
+
+
+def make_masked_msa(msa, hhblits_profile, uniform_prob, profile_prob, same_prob, replace_fraction, residue_index=None,
+                    msa_mask=None, is_evogen=False):
+    """create masked msa for BERT on raw MSA features"""
+
+    random_aatype = np.array([0.05] * 20 + [0., 0.], dtype=np.float32)
+
+    probability = uniform_prob * random_aatype + profile_prob * hhblits_profile + same_prob * one_hot(22, msa)
+
+    pad_shapes = [[0, 0] for _ in range(len(probability.shape))]
+    pad_shapes[-1][1] = 1
+    mask_prob = 1. - profile_prob - same_prob - uniform_prob
+
+    probability = np.pad(probability, pad_shapes, constant_values=(mask_prob,))
+
+    masked_aatype = np.random.uniform(size=msa.shape, low=0, high=1) < replace_fraction
+
+    bert_msa = shaped_categorical(probability)
+    bert_msa = np.where(masked_aatype, bert_msa, msa)
+
+    bert_mask = masked_aatype.astype(np.int32)
+    true_msa = msa
+    msa = bert_msa
+    if is_evogen:
+        additional_input = np.concatenate((bert_msa[0][:, None], np.asarray(residue_index)[:, None],
+                                           msa_mask[0][:, None],
+                                           bert_mask[0][:, None]),
+                                          axis=-1).astype(np.int32)
+        make_masked_msa_result = bert_mask, true_msa, msa, additional_input
+
+    else:
+        make_masked_msa_result = bert_mask, true_msa, msa
+    return make_masked_msa_result
+
+
+def share_mask_by_entity(mask_position, entity_id, sym_id, num_sym):
+    "share mask by entity"
+    entity_id = entity_id
+    sym_id = sym_id
+    num_sym = num_sym
+    unique_entity_ids = np.unique(entity_id)
+    first_sym_mask = sym_id == 1
+    for cur_entity_id in unique_entity_ids:
+        cur_entity_mask = entity_id == cur_entity_id
+        cur_num_sym = int(num_sym[cur_entity_mask][0])
+        if cur_num_sym > 1:
+            cur_sym_mask = first_sym_mask & cur_entity_mask
+            cur_sym_bert_mask = mask_position[:, cur_sym_mask]
+            mask_position[:, cur_entity_mask] = cur_sym_bert_mask.repeat(cur_num_sym, 0).reshape(
+                cur_sym_bert_mask.shape[0], cur_sym_bert_mask.shape[1] * cur_num_sym)
+    return mask_position
+
+
+def gumbel_max_sample(logits):
+    """Samples from a probability distribution given by 'logits'."""
+    z = gumbel_noise(logits.shape)
+    return np.argmax(logits + z, axis=-1)
+
+
+def make_masked_msa_v2(msa, hhblits_profile, msa_mask, entity_id, sym_id, num_sym,
+                       uniform_prob, profile_prob, same_prob,
+                       replace_fraction, share_mask=False, bert_mask=None):
+    """create masked msa for BERT on raw MSA features"""
+
+    random_aatype = np.array([0.05] * 20 + [0., 0.], dtype=np.float32)
+    probability = uniform_prob * random_aatype + profile_prob * hhblits_profile + same_prob * one_hot(22, msa)
+
+    pad_shapes = [[0, 0] for _ in range(len(probability.shape))]
+    pad_shapes[-1][1] = 1
+    mask_prob = 1.0 - profile_prob - same_prob - uniform_prob
+    assert mask_prob >= 0.0
+    probability = np.pad(probability, pad_shapes, constant_values=(mask_prob,))
+    sh = msa.shape
+    mask_position = np.random.rand(*sh) < replace_fraction
+    mask_position &= np.array(msa_mask, dtype=bool)
+    if bert_mask is not None:
+        mask_position &= np.array(bert_mask, dtype=bool)
+
+    if share_mask:
+        mask_position = share_mask_by_entity(mask_position, entity_id, sym_id, num_sym)
+    logits = np.log(probability + 1e-6)
+    bert_msa = gumbel_max_sample(logits)
+    bert_msa = np.where(mask_position, bert_msa, msa).astype(np.float32)
+    bert_msa *= msa_mask
+
+    mask_position = np.array(mask_position, dtype=np.float32)
+    return mask_position, msa, bert_msa
+
+
+def nearest_neighbor_clusters(msa_mask, msa, extra_msa_mask, extra_msa, gap_agreement_weight=0.):
+    """Assign each extra MSA sequence to its nearest neighbor in sampled MSA."""
+
+    # Determine how much weight we assign to each agreement.  In theory, we could
+    # use a full blosum matrix here, but right now let's just down-weight gap
+    # agreement because it could be spurious.
+    # Never put weight on agreeing on BERT mask
+    weights = np.concatenate([np.ones(21), gap_agreement_weight * np.ones(1), np.zeros(1)], 0)
+
+    # Make agreement score as weighted Hamming distance
+    sample_one_hot = msa_mask[:, :, None] * one_hot(23, msa)
+    num_seq, num_res, _ = sample_one_hot.shape
+
+    array_extra_msa_mask = extra_msa_mask
+    if array_extra_msa_mask.any():
+        extra_one_hot = extra_msa_mask[:, :, None] * one_hot(23, extra_msa)
+        extra_num_seq, _, _ = extra_one_hot.shape
+
+        agreement = np.matmul(
+            np.reshape(extra_one_hot, [extra_num_seq, num_res * 23]),
+            np.reshape(sample_one_hot * weights, [num_seq, num_res * 23]).T)
+        # Assign each sequence in the extra sequences to the closest MSA sample
+        extra_cluster_assignment = np.argmax(agreement, axis=1)
+    else:
+        extra_cluster_assignment = np.array([])
+    return extra_cluster_assignment
+
+
+def nearest_neighbor_clusters_v2(msa, msa_mask, extra_msa, extra_msa_mask,
+                                 deletion_matrix, extra_deletion_matrix, gap_agreement_weight=0.0):
+    """Assign each extra MSA sequence to its nearest neighbor in sampled MSA."""
+
+    # Determine how much weight we assign to each agreement.  In theory, we could
+    # use a full blosum matrix here, but right now let's just down-weight gap
+    # agreement because it could be spurious.
+    # Never put weight on agreeing on BERT mask.
+
+    weights = np.concatenate([np.ones(21), gap_agreement_weight * np.ones(1), np.zeros(1)], 0)
+    msa_one_hot = one_hot(23, msa.astype(np.int32))
+    extra_one_hot = one_hot(23, extra_msa)
+
+    msa_one_hot_masked = msa_mask[:, :, None] * msa_one_hot
+    extra_one_hot_masked = extra_msa_mask[:, :, None] * extra_one_hot
+
+    t1 = weights * msa_one_hot_masked
+    t1 = np.resize(t1, (t1.shape[0], t1.shape[1] * t1.shape[2]))
+    t2 = np.resize(extra_one_hot_masked, (extra_one_hot.shape[0], extra_one_hot.shape[1] * extra_one_hot.shape[2]))
+    agreement = t1 @ t2.T
+    cluster_assignment = softmax(1e3 * agreement, axis=0)
+    cluster_assignment *= np.einsum("mr, nr->mn", msa_mask, extra_msa_mask)
+
+    cluster_count = np.sum(cluster_assignment, axis=-1)
+    cluster_count += 1.0  # We always include the sequence itself.
+
+    msa_sum = np.einsum("nm, mrc->nrc", cluster_assignment, extra_one_hot_masked)
+    msa_sum += msa_one_hot_masked
+
+    cluster_profile = msa_sum / cluster_count[:, None, None]
+
+    del_sum = np.einsum(
+        "nm, mc->nc", cluster_assignment, extra_msa_mask * extra_deletion_matrix
+    )
+    del_sum += deletion_matrix  # Original sequence.
+    cluster_deletion_mean = del_sum / cluster_count[:, None]
+
+    return cluster_profile, cluster_deletion_mean
+
+
+def summarize_clusters(msa, msa_mask, extra_cluster_assignment, extra_msa_mask, extra_msa, extra_deletion_matrix,
+                       deletion_matrix):
+    """Produce profile and deletion_matrix_mean within each cluster."""
+    num_seq = msa.shape[0]
+
+    def csum(x):
+        result = []
+        for i in range(num_seq):
+            result.append(np.sum(x[np.where(extra_cluster_assignment == i)], axis=0))
+        return np.array(result)
+
+    mask = extra_msa_mask
+    mask_counts = 1e-6 + msa_mask + csum(mask)  # Include center
+
+    msa_sum = csum(mask[:, :, None] * one_hot(23, extra_msa))
+    msa_sum += one_hot(23, msa)  # Original sequence
+    cluster_profile = msa_sum / mask_counts[:, :, None]
+
+    del msa_sum
+
+    del_sum = csum(mask * extra_deletion_matrix)
+    del_sum += deletion_matrix  # Original sequence
+    cluster_deletion_mean = del_sum / mask_counts
+    del del_sum
+
+    return cluster_profile, cluster_deletion_mean
+
+
+def crop_extra_msa(extra_msa, max_extra_msa):
+    """MSA features are cropped so only `max_extra_msa` sequences are kept."""
+    if extra_msa.any():
+        num_seq = extra_msa.shape[0]
+        num_sel = np.minimum(max_extra_msa, num_seq)
+        shuffled = list(range(num_seq))
+        np.random.shuffle(shuffled)
+        select_indices = shuffled[:num_sel]
+        return select_indices
+    return None
+
+
+def make_msa_feat(between_segment_residues, aatype, msa, deletion_matrix, cluster_deletion_mean, cluster_profile,
+                  extra_deletion_matrix):
+    """Create and concatenate MSA features."""
+    # Whether there is a domain break. Always zero for chains, but keeping
+    # for compatibility with domain datasets.
+    has_break = np.clip(between_segment_residues.astype(np.float32), np.array(0), np.array(1))
+    aatype_1hot = one_hot(21, aatype)
+
+    target_feat = [np.expand_dims(has_break, axis=-1), aatype_1hot]
+
+    msa_1hot = one_hot(23, msa)
+    has_deletion = np.clip(deletion_matrix, np.array(0), np.array(1))
+    deletion_value = np.arctan(deletion_matrix / 3.) * (2. / np.pi)
+
+    msa_feat = [msa_1hot, np.expand_dims(has_deletion, axis=-1), np.expand_dims(deletion_value, axis=-1)]
+
+    if cluster_profile is not None:
+        deletion_mean_value = (np.arctan(cluster_deletion_mean / 3.) * (2. / np.pi))
+        msa_feat.extend([cluster_profile, np.expand_dims(deletion_mean_value, axis=-1)])
+    extra_has_deletion = None
+    extra_deletion_value = None
+    if extra_deletion_matrix is not None:
+        extra_has_deletion = np.clip(extra_deletion_matrix, np.array(0), np.array(1))
+        extra_deletion_value = np.arctan(extra_deletion_matrix / 3.) * (2. / np.pi)
+
+    msa_feat = np.concatenate(msa_feat, axis=-1)
+    target_feat = np.concatenate(target_feat, axis=-1)
+    res = [extra_has_deletion, extra_deletion_value, msa_feat, target_feat]
+    return res
+
+
+def make_msa_feat_v2(msa, deletion_matrix, cluster_deletion_mean, cluster_profile):
+    """Create and concatenate MSA features."""
+    msa_1hot = one_hot(23, msa.astype(np.int32))
+    has_deletion = np.clip(deletion_matrix, 0.0, 1.0)[..., None]
+    deletion_value = (np.arctan(deletion_matrix / 3.0) * (2.0 / np.pi))[..., None]
+
+    deletion_mean_value = (np.arctan(cluster_deletion_mean / 3.0) * (2.0 / np.pi))[..., None]
+
+    msa_feat = [
+        msa_1hot,
+        has_deletion,
+        deletion_value,
+        cluster_profile,
+        deletion_mean_value,
+    ]
+    msa_feat = np.concatenate(msa_feat, axis=-1)
+    return msa_feat
+
+
+def make_extra_msa_feat(extra_msa, extra_deletion_matrix, extra_msa_mask, num_extra_msa):
+    # 23 = 20 amino acids + 'X' for unknown + gap + bert mask
+    extra_msa = extra_msa[:num_extra_msa]
+    deletion_matrix = extra_deletion_matrix[:num_extra_msa]
+    has_deletion = np.clip(deletion_matrix, 0.0, 1.0)
+    deletion_value = np.arctan(deletion_matrix / 3.0) * (2.0 / np.pi)
+    extra_msa_mask = extra_msa_mask[:num_extra_msa]
+    return {"extra_msa": extra_msa,
+            "extra_msa_mask": extra_msa_mask,
+            "extra_msa_has_deletion": has_deletion,
+            "extra_msa_deletion_value": deletion_value}
+
+
+def make_random_seed(size, seed_maker_t, low=MS_MIN32, high=MS_MAX32, random_recycle=False):
+    if random_recycle:
+        r = np.random.RandomState(seed_maker_t)
+        return r.uniform(size=size, low=low, high=high)
+    np.random.seed(seed_maker_t)
+    return np.random.uniform(size=size, low=low, high=high)
+
+
+def random_crop_to_size(seq_length, template_mask, crop_size, max_templates,
+                        subsample_templates=False, seed=0, random_recycle=False):
+    """Crop randomly to `crop_size`, or keep as is if shorter than that."""
+    seq_length = seq_length
+    seq_length_int = int(seq_length)
+    if template_mask is not None:
+        num_templates = np.array(template_mask.shape[0], np.int32)
+    else:
+        num_templates = np.array(0, np.int32)
+    num_res_crop_size = np.minimum(seq_length, crop_size)
+    num_res_crop_size_int = int(num_res_crop_size)
+
+    # Ensures that the cropping of residues and templates happens in the same way
+    # across ensembling iterations.
+    # Do not use for randomness that should vary in ensembling.
+
+    if subsample_templates:
+        templates_crop_start = int(make_random_seed(size=(), seed_maker_t=seed, low=0, high=num_templates + 1,
+                                                    random_recycle=random_recycle))
+    else:
+        templates_crop_start = 0
+
+    num_templates_crop_size = np.minimum(num_templates - templates_crop_start, max_templates)
+    num_templates_crop_size_int = int(num_templates_crop_size)
+
+    num_res_crop_start = int(make_random_seed(size=(), seed_maker_t=seed, low=0,
+                                              high=seq_length_int - num_res_crop_size_int + 1,
+                                              random_recycle=random_recycle))
+
+    templates_select_indices = np.argsort(make_random_seed(size=[num_templates], seed_maker_t=seed,
+                                                           random_recycle=random_recycle))
+    res = [num_res_crop_size, num_templates_crop_size_int, num_res_crop_start, num_res_crop_size_int, \
+           templates_crop_start, templates_select_indices]
+    return res
+
+
+def atom37_to_torsion_angles(
+        aatype: np.ndarray,
+        all_atom_pos: np.ndarray,
+        all_atom_mask: np.ndarray,
+        alt_torsions=False,
+        is_multimer=False,
+):
+    r"""
+    This function calculates the seven torsion angles of each residue and encodes them in sine and cosine.
+    The order of the seven torsion angles is [pre_omega, phi, psi, chi_1, chi_2, chi_3, chi_4]
+    Here, pre_omega represents the twist angle between a given amino acid and the previous amino acid.
+    The phi represents twist angle between `C-CA-N-(C+1)`, psi represents twist angle between `(N-1)-C-CA-N`.
+
+    Args:
+        aatype (numpy.array):           Amino acid type with shape :math:`(batch\_size, N_{res})`.
+        all_atom_pos (numpy.array):     Atom37 representation of all atomic coordinates with
+                                        shape :math:`(batch\_size, N_{res}, 37, 3)`.
+        all_atom_mask (numpy.array):    Atom37 representation of the mask on all atomic coordinates with
+                                        shape :math:`(batch\_size, N_{res})`.
+        alt_torsions (bool):            Indicates whether to set the sign angle of shielding torsion to zero.
+                                        Default: False.
+        is_multimer (bool):             It will be True when multimer is used. Default: False
+
+    Returns:
+        Dict containing
+
+        - torsion_angles_sin_cos (numpy.array), with shape :math:`(N_{res}, 7, 2)` where
+          the final 2 dimensions denote sin and cos respectively. If is_multimer is True, the shape will
+          be :math:`(N_{seq}, N_{res}, 7, 2)` .
+        - alt_torsion_angles_sin_cos (numpy.array), same as 'torsion_angles_sin_cos', but with the angle shifted
+          by pi for all chi angles affected by the naming ambiguities. shape is :math:`(N_{res}, 7, 2)`.
+          If is_multimer is True, the shape will be :math:`(N_{seq}, N_{res}, 7, 2)` .
+        - torsion_angles_mask (numpy.array), Mask for which chi angles are present. shape is :math:`(N_{res}, 7)` .
+          If is_multimer is True, the shape will be :math:`(N_{seq}, N_{res}, 7, 2)` .
+
+    Supported Platforms:
+        ``Ascend`` ``GPU`` ``CPU``
+
+    Examples:
+        >>> import numpy as np
+        >>> from mindsponge.data.data_transform import atom37_to_torsion_angles
+        >>> n_res = 16
+        >>> bs = 1
+        >>> aatype = np.random.randn(bs, n_res).astype(np.int32)
+        >>> all_atom_pos = np.random.randn(bs, n_res, 37, 3).astype(np.float32)
+        >>> all_atom_mask = np.random.randn(bs, n_res, 37).astype(np.float32)
+        >>> angle_label_feature = atom37_to_torsion_angles(aatype, all_atom_pos, all_atom_mask)
+        >>> print(angle_label_feature.keys())
+        dict_keys(['torsion_angles_sin_cos', 'alt_torsion_angles_sin_cos', 'torsion_angles_mask'])
+    """
+
+    true_aatype = np.minimum(aatype, 20)
+
+    # get the number residue
+    num_batch, num_res = true_aatype.shape
+
+    paddings = np.zeros([num_batch, 1, 37, 3], np.float32)
+    padding_atom_pos = np.concatenate([paddings, all_atom_pos[:, :-1, :, :]], axis=1)
+    paddings = np.zeros([num_batch, 1, 37], np.float32)
+    padding_atom_mask = np.concatenate([paddings, all_atom_mask[:, :-1, :]], axis=1)
+
+    # compute padding atom position for omega, phi and psi
+    omega_atom_pos_padding = np.concatenate(
+        [padding_atom_pos[..., 1:3, :],
+         all_atom_pos[..., 0:2, :]
+         ], axis=-2)
+    phi_atom_pos_padding = np.concatenate(
+        [padding_atom_pos[..., 2:3, :],
+         all_atom_pos[..., 0:3, :]
+         ], axis=-2)
+    psi_atom_pos_padding = np.concatenate(
+        [all_atom_pos[..., 0:3, :],
+         all_atom_pos[..., 4:5, :]
+         ], axis=-2)
+
+    # compute padding atom position mask for omega, phi and psi
+    omega_mask_padding = (np.prod(padding_atom_mask[..., 1:3], axis=-1) *
+                          np.prod(all_atom_mask[..., 0:2], axis=-1))
+    phi_mask_padding = (padding_atom_mask[..., 2] * np.prod(all_atom_mask[..., 0:3], axis=-1))
+    psi_mask_padding = (np.prod(all_atom_mask[..., 0:3], axis=-1) * all_atom_mask[..., 4])
+
+    chi_atom_pos_indices = get_chi_atom_pos_indices()
+    if is_multimer:
+        atom_pos_indices = chi_atom_pos_indices[..., true_aatype, :, :]
+    else:
+        atom_pos_indices = np_gather_ops(chi_atom_pos_indices, true_aatype, 0, 0)
+
+    chi_atom_pos = np_gather_ops(all_atom_pos, atom_pos_indices, -2, 2, is_multimer)
+
+    angles_mask = list(chi_angles_mask)
+    angles_mask.append([0.0, 0.0, 0.0, 0.0])
+    angles_mask = np.array(angles_mask)
+
+    if is_multimer:
+        chis_mask = angles_mask[true_aatype, :]
+    else:
+        chis_mask = np_gather_ops(angles_mask, true_aatype, 0, 0)
+
+    chi_angle_atoms_mask = np_gather_ops(all_atom_mask, atom_pos_indices, -1, 2, is_multimer)
+
+    chi_angle_atoms_mask = np.prod(chi_angle_atoms_mask, axis=-1)
+    chis_mask = chis_mask * chi_angle_atoms_mask.astype(np.float32)
+    torsions_atom_pos_padding = np.concatenate(
+        [omega_atom_pos_padding[:, :, None, :, :],
+         phi_atom_pos_padding[:, :, None, :, :],
+         psi_atom_pos_padding[:, :, None, :, :],
+         chi_atom_pos
+         ], axis=2)
+    torsion_angles_mask_padding = np.concatenate(
+        [omega_mask_padding[:, :, None],
+         phi_mask_padding[:, :, None],
+         psi_mask_padding[:, :, None],
+         chis_mask
+         ], axis=2)
+    torsion_frames = geometry.rigids_from_3_points(
+        point_on_neg_x_axis=geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 1, :]),
+        origin=geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 2, :]),
+        point_on_xy_plane=geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 0, :]))
+    inv_torsion_frames = geometry.invert_rigids(torsion_frames)
+    vecs = geometry.vecs_from_tensor(torsions_atom_pos_padding[:, :, :, 3, :])
+    forth_atom_rel_pos = geometry.rigids_mul_vecs(inv_torsion_frames, vecs)
+    torsion_angles_sin_cos = np.stack(
+        [forth_atom_rel_pos[2], forth_atom_rel_pos[1]], axis=-1)
+    torsion_angles_sin_cos /= np.sqrt(
+        np.sum(np.square(torsion_angles_sin_cos), axis=-1, keepdims=True)
+        + 1e-8)
+
+    if is_multimer:
+        torsion_angles_sin_cos = torsion_angles_sin_cos * np.array(
+            [1., 1., -1., 1., 1., 1., 1.])[((None,) * len(torsion_angles_sin_cos.shape[:-2])) + (slice(None), None)]
+        chi_is_ambiguous = np.array(chi_pi_periodic)[true_aatype, ...]
+    else:
+        torsion_angles_sin_cos *= np.array(
+            [1., 1., -1., 1., 1., 1., 1.])[None, None, :, None]
+
+        chi_is_ambiguous = np_gather_ops(
+            np.array(chi_pi_periodic), true_aatype)
+
+    mirror_torsion_angles = np.concatenate(
+        [np.ones([num_batch, num_res, 3]),
+         1.0 - 2.0 * chi_is_ambiguous], axis=-1)
+    alt_torsion_angles_sin_cos = (torsion_angles_sin_cos * mirror_torsion_angles[:, :, :, None])
+
+    if alt_torsions:
+        fix_torsions = np.stack([np.ones(torsion_angles_sin_cos.shape[:-1]),
+                                 np.zeros(torsion_angles_sin_cos.shape[:-1])], axis=-1)
+        torsion_angles_sin_cos = torsion_angles_sin_cos * torsion_angles_mask_padding[
+            ..., None] + fix_torsions * (1 - torsion_angles_mask_padding[..., None])
+        alt_torsion_angles_sin_cos = alt_torsion_angles_sin_cos * torsion_angles_mask_padding[
+            ..., None] + fix_torsions * (1 - torsion_angles_mask_padding[..., None])
+
+    if is_multimer:
+        return {
+            'torsion_angles_sin_cos': torsion_angles_sin_cos,
+            'alt_torsion_angles_sin_cos': alt_torsion_angles_sin_cos,
+            'torsion_angles_mask': torsion_angles_mask_padding
+        }
+    return {
+        'torsion_angles_sin_cos': torsion_angles_sin_cos[0],  # (N, 7, 2)
+        'alt_torsion_angles_sin_cos': alt_torsion_angles_sin_cos[0],  # (N, 7, 2)
+        'torsion_angles_mask': torsion_angles_mask_padding[0]  # (N, 7)
+    }
+
+
+def atom37_to_frames(
+        aatype,
+        all_atom_positions,
+        all_atom_mask,
+        is_affine=False
+):
+    r"""
+    Computes the torsion angle of up to 8 rigid groups for each residue, shape is :math:`[N_{res}, 8, 12]`,
+    where 8 is indicates that each residue can be divided into up to 8 rigid groups according to the dependence of
+    the atom on the torsion angle, there are 1 backbone frame and 7 side-chain frames.
+    For the meaning of 12 ,the first 9 elements are the 9 components of rotation matrix, the last
+    3 elements are the 3 component of translation matrix.
+
+
+    Args:
+        aatype(numpy.array):                Amino acid sequence, :math:`[N_{res}]` .
+        all_atom_positions(numpy.array):    The coordinates of all atoms, presented as atom37, :math:`[N_{res}, 37, 3]`.
+        all_atom_mask(numpy.array):         Mask of all atomic coordinates, :math:`[N_{res}, 37]`.
+        is_affine(bool):                    Whether to perform affine, the default value is False.
+
+    Returns:
+        Dictionary, the specific content is as follows.
+
+        - **rigidgroups_gt_frames** (numpy.array) - The torsion angle of the 8 rigid body groups for each residue,
+          :math:`[N_{res}, 8, 12]`.
+        - **rigidgroups_gt_exists** (numpy.array) - The mask of rigidgroups_gt_frames denoting whether the rigid body
+          group exists according to the experiment, :math:`[N_{res}, 8]`.
+        - **rigidgroups_group_exists** (numpy.array) - Mask denoting whether given group is in principle present
+          for given amino acid type, :math:`[N_{res}, 8]` .
+        - **rigidgroups_group_is_ambiguous** (numpy.array) - Indicates that the position is chiral symmetry,
+          :math:`[N_{res}, 8]` .
+        - **rigidgroups_alt_gt_frames** (numpy.array) - 8 Frames with alternative atom renaming
+          corresponding to 'all_atom_positions' represented as flat
+          12 dimensional array :math:`[N_{res}, 8, 12]` .
+        - **backbone_affine_tensor** (numpy.array) - The translation and rotation of the local coordinates of each
+          amino acid relative to the global coordinates, :math:`[N_{res}, 7]` , for the last dimension, the first 4
+          elements are the affine tensor which contains the rotation information, the last 3 elements are the
+          translations in space.
+
+    Supported Platforms:
+        ``Ascend`` ``GPU`` ``CPU``
+
+    Examples:
+        >>> import numpy as np
+        >>> from mindsponge.data import atom37_to_frames
+        >>> from mindspore import dtype as mstype
+        >>> from mindspore import Tensor
+        >>> aatype = np.ones(193,dtype=np.int32)
+        >>> all_atom_positions = np.ones((193,37,3),dtype=np.float32)
+        >>> all_atom_mask = np.ones((193,37),dtype=np.int32)
+        >>> result = atom37_to_frames(aatype,all_atom_positions,all_atom_mask)
+        >>> for key in result.keys():
+        >>>     print(key,result[key].shape)
+        rigidgroups_gt_frames (193, 8, 12)
+        rigidgroups_gt_exists (193, 8)
+        rigidgroups_group_exists (193, 8)
+        rigidgroups_group_is_ambiguous (193, 8)
+        rigidgroups_alt_gt_frames (193, 8, 12)
+    """
+    aatype_shape = aatype.shape
+
+    flat_aatype = np.reshape(aatype, [-1])
+    all_atom_positions = np.reshape(all_atom_positions, [-1, 37, 3])
+    all_atom_mask = np.reshape(all_atom_mask, [-1, 37])
+
+    rigid_group_names_res = np.full([21, 8, 3], '', dtype=object)
+
+    # group 0: backbone frame
+    rigid_group_names_res[:, 0, :] = ['C', 'CA', 'N']
+
+    # group 3: 'psi'
+    rigid_group_names_res[:, 3, :] = ['CA', 'C', 'O']
+
+    # group 4,5,6,7: 'chi1,2,3,4'
+    for restype, letter in enumerate(restypes):
+        restype_name = restype_1to3[letter]
+        for chi_idx in range(4):
+            if chi_angles_mask[restype][chi_idx]:
+                atom_names = chi_angles_atoms[restype_name][chi_idx]
+                rigid_group_names_res[restype, chi_idx + 4, :] = atom_names[1:]
+
+    # create rigid group mask
+    rigid_group_mask_res = np.zeros([21, 8], dtype=np.float32)
+    rigid_group_mask_res[:, 0] = 1
+    rigid_group_mask_res[:, 3] = 1
+    rigid_group_mask_res[:20, 4:] = chi_angles_mask
+
+    lookup_table = atom_order.copy()
+    lookup_table[''] = 0
+    rigid_group_atom37_idx_restype = np.vectorize(lambda x: lookup_table[x])(
+        rigid_group_names_res)
+
+    rigid_group_atom37_idx_residx = np_gather_ops(
+        rigid_group_atom37_idx_restype, flat_aatype)
+
+    base_atom_pos = np_gather_ops(
+        all_atom_positions,
+        rigid_group_atom37_idx_residx,
+        batch_dims=1)
+
+    gt_frames = geometry.rigids_from_3_points(
+        point_on_neg_x_axis=geometry.vecs_from_tensor(base_atom_pos[:, :, 0, :]),
+        origin=geometry.vecs_from_tensor(base_atom_pos[:, :, 1, :]),
+        point_on_xy_plane=geometry.vecs_from_tensor(base_atom_pos[:, :, 2, :]))
+
+    # get the group mask
+    group_masks = np_gather_ops(rigid_group_mask_res, flat_aatype)
+
+    # get the atom mask
+    gt_atoms_exists = np_gather_ops(
+        all_atom_mask.astype(np.float32),
+        rigid_group_atom37_idx_residx,
+        batch_dims=1)
+    gt_masks = np.min(gt_atoms_exists, axis=-1) * group_masks
+
+    rotations = np.tile(np.eye(3, dtype=np.float32), [8, 1, 1])
+    rotations[0, 0, 0] = -1
+    rotations[0, 2, 2] = -1
+    gt_frames = geometry.rigids_mul_rots(gt_frames, geometry.rots_from_tensor(rotations, use_numpy=True))
+
+    rigid_group_is_ambiguous_res = np.zeros([21, 8], dtype=np.float32)
+    rigid_group_rotations_res = np.tile(np.eye(3, dtype=np.float32), [21, 8, 1, 1])
+
+    for restype_name, _ in residue_atom_renaming_swaps.items():
+        restype = restype_order[restype_3to1[restype_name]]
+        chi_idx = int(sum(chi_angles_mask[restype]) - 1)
+        rigid_group_is_ambiguous_res[restype, chi_idx + 4] = 1
+        rigid_group_rotations_res[restype, chi_idx + 4, 1, 1] = -1
+        rigid_group_rotations_res[restype, chi_idx + 4, 2, 2] = -1
+
+    # Gather the ambiguity information for each residue.
+    rigid_group_is_ambiguous_res_index = np_gather_ops(
+        rigid_group_is_ambiguous_res, flat_aatype)
+    rigid_group_ambiguity_rotation_res_index = np_gather_ops(
+        rigid_group_rotations_res, flat_aatype)
+
+    # Create the alternative ground truth frames.
+    alt_gt_frames = geometry.rigids_mul_rots(
+        gt_frames, geometry.rots_from_tensor(rigid_group_ambiguity_rotation_res_index, use_numpy=True))
+
+    gt_frames_flat12 = np.stack(list(gt_frames[0]) + list(gt_frames[1]), axis=-1)
+    alt_gt_frames_flat12 = np.stack(list(alt_gt_frames[0]) + list(alt_gt_frames[1]), axis=-1)
+    # reshape back to original residue layout
+    gt_frames_flat12 = np.reshape(gt_frames_flat12, aatype_shape + (8, 12))
+    gt_masks = np.reshape(gt_masks, aatype_shape + (8,))
+    group_masks = np.reshape(group_masks, aatype_shape + (8,))
+    gt_frames_flat12 = np.reshape(gt_frames_flat12, aatype_shape + (8, 12))
+    rigid_group_is_ambiguous_res_index = np.reshape(rigid_group_is_ambiguous_res_index, aatype_shape + (8,))
+    alt_gt_frames_flat12 = np.reshape(alt_gt_frames_flat12,
+                                      aatype_shape + (8, 12,))
+    if not is_affine:
+        return {
+            'rigidgroups_gt_frames': gt_frames_flat12,  # shape (..., 8, 12)
+            'rigidgroups_gt_exists': gt_masks,  # shape (..., 8)
+            'rigidgroups_group_exists': group_masks,  # shape (..., 8)
+            'rigidgroups_group_is_ambiguous':
+                rigid_group_is_ambiguous_res_index,  # shape (..., 8)
+            'rigidgroups_alt_gt_frames': alt_gt_frames_flat12,  # shape (..., 8, 12)
+        }
+
+    rotation = [[gt_frames[0][0], gt_frames[0][1], gt_frames[0][2]],
+                [gt_frames[0][3], gt_frames[0][4], gt_frames[0][5]],
+                [gt_frames[0][6], gt_frames[0][7], gt_frames[0][8]]]
+    translation = [gt_frames[1][0], gt_frames[1][1], gt_frames[1][2]]
+    backbone_affine_tensor = to_tensor(rotation, translation)[:, 0, :]
+    return {
+        'rigidgroups_gt_frames': gt_frames_flat12,  # shape (..., 8, 12)
+        'rigidgroups_gt_exists': gt_masks,  # shape (..., 8)
+        'rigidgroups_group_exists': group_masks,  # shape (..., 8)
+        'rigidgroups_group_is_ambiguous': rigid_group_is_ambiguous_res_index,  # shape (..., 8)
+        'rigidgroups_alt_gt_frames': alt_gt_frames_flat12,  # shape (..., 8, 12)
+        'backbone_affine_tensor': backbone_affine_tensor,  # shape (..., 7)
+    }
+
+
+def get_chi_atom_pos_indices():
+    """get the atom indices for computing chi angles for all residue types"""
+    chi_atom_pos_indices = []
+    for residue_name in restypes:
+        residue_name = restype_1to3[residue_name]
+        residue_chi_angles = chi_angles_atoms[residue_name]
+        atom_pos_indices = []
+        for chi_angle in residue_chi_angles:
+            atom_pos_indices.append([atom_order[atom] for atom in chi_angle])
+        for _ in range(4 - len(atom_pos_indices)):
+            atom_pos_indices.append([0, 0, 0, 0])  # For chi angles not defined on the AA.
+        chi_atom_pos_indices.append(atom_pos_indices)
+
+    chi_atom_pos_indices.append([[0, 0, 0, 0]] * 4)  # For UNKNOWN residue.
+
+    return np.array(chi_atom_pos_indices)
+
+
+def gather(params, indices, axis=0):
+    """gather operation"""
+    func = lambda p, i: np.take(p, i, axis=axis)
+    return func(params, indices)
+
+
+def np_gather_ops(params, indices, axis=0, batch_dims=0, is_multimer=False):
+    """np gather operation"""
+    if is_multimer:
+        assert axis < 0 or axis - batch_dims >= 0
+        ranges = []
+        for i, s in enumerate(params.shape[:batch_dims]):
+            r = np.arange(s)
+            r = np.resize(r, (1,) * i + r.shape + (1,) * (len(indices.shape) - i - 1))
+            ranges.append(r)
+        remaining_dims = [slice(None) for _ in range(len(params.shape) - batch_dims)]
+        remaining_dims[axis - batch_dims if axis >= 0 else axis] = indices
+        ranges.extend(remaining_dims)
+        return params[tuple(ranges)]
+
+    if batch_dims == 0:
+        return gather(params, indices)
+    result = []
+    if batch_dims == 1:
+        for p, i in zip(params, indices):
+            axis = axis - batch_dims if axis - batch_dims > 0 else 0
+            r = gather(p, i, axis=axis)
+            result.append(r)
+        return np.stack(result)
+    for p, i in zip(params[0], indices[0]):
+        r = gather(p, i, axis=axis)
+        result.append(r)
+    res = np.stack(result)
+    return res.reshape((1,) + res.shape)
+
+
+def rot_to_quat(rot, unstack_inputs=False):
+    """transfer the rotation matrix to quaternion matrix"""
+    if unstack_inputs:
+        rot = [np.moveaxis(x, -1, 0) for x in np.moveaxis(rot, -2, 0)]
+    [[xx, xy, xz], [yx, yy, yz], [zx, zy, zz]] = rot
+
+    k = [[xx + yy + zz, zy - yz, xz - zx, yx - xy],
+         [zy - yz, xx - yy - zz, xy + yx, xz + zx],
+         [xz - zx, xy + yx, yy - xx - zz, yz + zy],
+         [yx - xy, xz + zx, yz + zy, zz - xx - yy]]
+
+    k = (1. / 3.) * np.stack([np.stack(x, axis=-1) for x in k],
+                             axis=-2)
+
+    # compute eigenvalues
+    _, qs = np.linalg.eigh(k)
+    return qs[..., -1]
+
+
+def to_tensor(rotation, translation):
+    """get affine based on rotation and translation"""
+    quaternion = rot_to_quat(rotation)
+    return np.concatenate(
+        [quaternion] +
+        [np.expand_dims(x, axis=-1) for x in translation],
+        axis=-1)
+
+
+def convert_monomer_features(chain_id, aatype, template_aatype):
+    """Reshapes and modifies monomer features for multimer models."""
+
+    auth_chain_id = np.asarray(chain_id, dtype=np.object_)
+    new_order_list = MAP_HHBLITS_AATYPE_TO_OUR_AATYPE
+    monomer_aatype = np.argmax(aatype, axis=-1).astype(np.int32)
+    monomer_template_aatype = np.argmax(template_aatype, axis=-1).astype(np.int32)
+    monomer_template_aatype = np.take(new_order_list, monomer_template_aatype.astype(np.int32), axis=0)
+
+    return auth_chain_id, monomer_aatype, monomer_template_aatype
+
+
+def convert_unnecessary_leading_dim_feats(sequence, domain_name, num_alignments, seq_length):
+    """get first dimension data of unnecessary features."""
+
+    monomer_sequence = np.asarray(sequence[0], dtype=sequence.dtype)
+    monomer_domain_name = np.asarray(domain_name[0], dtype=domain_name.dtype)
+    monomer_num_alignments = np.asarray(num_alignments[0], dtype=num_alignments.dtype)
+    monomer_seq_length = np.asarray(seq_length[0], dtype=seq_length.dtype)
+
+    converted_feature = (monomer_sequence, monomer_domain_name, monomer_num_alignments, monomer_seq_length)
+    return converted_feature
+
+
+def process_unmerged_features(deletion_matrix_int, deletion_matrix_int_all_seq, aatype, entity_id, num_chains):
+    """Postprocessing stage for per-chain features before merging."""
+    # Convert deletion matrices to float.
+    deletion_matrix = np.asarray(deletion_matrix_int, dtype=np.float32)
+    deletion_matrix_all_seq = np.asarray(deletion_matrix_int_all_seq, dtype=np.float32)
+
+    all_atom_mask = STANDARD_ATOM_MASK[aatype]
+    all_atom_mask = all_atom_mask
+    all_atom_positions = np.zeros(list(all_atom_mask.shape) + [3])
+    deletion_mean = np.mean(deletion_matrix, axis=0)
+
+    # Add assembly_num_chains.
+    assembly_num_chains = np.asarray(num_chains)
+    entity_mask = (entity_id != 0).astype(np.int32)
+    post_feature = (deletion_matrix, deletion_matrix_all_seq, deletion_mean, all_atom_mask, all_atom_positions,
+                    assembly_num_chains, entity_mask)
+
+    return post_feature
+
+
+def get_crop_size(num_alignments_all_seq, msa_all_seq, msa_crop_size, msa_size):
+    """get maximum msa crop size
+
+    Args:
+        num_alignments_all_seq: num_alignments for all sequence, which record the total number of msa
+        msa_all_seq: un-paired sequences for all msa.
+        msa_crop_size: The total number of sequences to crop from the MSA.
+        msa_size: number of msa
+
+    Returns:
+        msa_crop_size: msa sized to be cropped
+        msa_crop_size_all_seq: msa_crop_size for features with "_all_seq"
+
+    """
+
+    msa_size_all_seq = num_alignments_all_seq
+    msa_crop_size_all_seq = np.minimum(msa_size_all_seq, msa_crop_size // 2)
+
+    # We reduce the number of un-paired sequences, by the number of times a
+    # sequence from this chain's MSA is included in the paired MSA.  This keeps
+    # the MSA size for each chain roughly constant.
+    msa_all_seq = msa_all_seq[:msa_crop_size_all_seq, :]
+    num_non_gapped_pairs = np.sum(np.any(msa_all_seq != restypes_with_x_and_gap.index('-'), axis=1))
+    num_non_gapped_pairs = np.minimum(num_non_gapped_pairs, msa_crop_size_all_seq)
+
+    # Restrict the unpaired crop size so that paired+unpaired sequences do not
+    # exceed msa_seqs_per_chain for each chain.
+    max_msa_crop_size = np.maximum(msa_crop_size - num_non_gapped_pairs, 0)
+    msa_crop_size = np.minimum(msa_size, max_msa_crop_size)
+    return msa_crop_size, msa_crop_size_all_seq
+
+
+def make_seq_mask(entity_id):
+    """seq mask info, True for entity_id > 0, False for entity_id <= 0."""
+
+    seq_mask = (entity_id > 0).astype(np.float32)
+    return seq_mask
+
+
+def make_msa_mask(msa, entity_id):
+    """Mask features are all ones, but will later be zero-padded."""
+
+    msa_mask = np.ones_like(msa, dtype=np.float32)
+
+    seq_mask = (entity_id > 0).astype(np.float32)
+    msa_mask *= seq_mask[None]
+
+    return msa_mask
+
+
+def add_padding(feature_name, feature):
+    """get padding data with specified shapes of feature"""
+
+    num_res = feature.shape[1]
+    padding = MSA_PAD_VALUES.get(feature_name) * np.ones([1, num_res], feature.dtype)
+    return padding
+
+
+def generate_random_sample(cfg, model_config):
+    '''generate_random_sample'''
+    np.random.seed(0)
+    num_noise = model_config.model.latent.num_noise
+    latent_dim = model_config.model.latent.latent_dim
+
+    context_true_prob = np.absolute(model_config.train.context_true_prob)
+    keep_prob = np.absolute(model_config.train.keep_prob)
+
+    available_msa = int(model_config.train.available_msa_fraction * model_config.train.max_msa_clusters)
+    available_msa = min(available_msa, model_config.train.max_msa_clusters)
+
+    evogen_random_data = np.random.normal(
+        size=(num_noise, model_config.train.max_msa_clusters, cfg.eval.crop_size, latent_dim)).astype(np.float32)
+
+    # (Nseq,):
+    context_mask = np.zeros((model_config.train.max_msa_clusters,), np.int32)
+    z1 = np.random.random(model_config.train.max_msa_clusters)
+    context_mask = np.asarray([1 if x < context_true_prob else 0 for x in z1], np.int32)
+    context_mask[available_msa:] *= 0
+
+    # (Nseq,):
+    target_mask = np.zeros((model_config.train.max_msa_clusters,), np.int32)
+    z2 = np.random.random(model_config.train.max_msa_clusters)
+    target_mask = np.asarray([1 if x < keep_prob else 0 for x in z2], np.int32)
+
+    context_mask[0] = 1
+    target_mask[0] = 1
+
+    evogen_context_mask = np.stack((context_mask, target_mask), -1)
+    return evogen_random_data, evogen_context_mask
+
+
+def to_tensor_4x4(feature):
+    rots = feature[..., :9]
+    trans = feature[..., 9:]
+    arrays = np.zeros(feature.shape[:-1] + (4, 4))
+    rots = np.reshape(rots, rots.shape[:-1] + (3, 3))
+    arrays[..., :3, :3] = rots
+    arrays[..., :3, 3] = trans
+    arrays[..., 3, 3] = 1
+    return arrays
```

## mindsponge/function/functions.py

```diff
@@ -27,19 +27,15 @@
 from typing import Union
 import numpy as np
 from numpy import ndarray
 import mindspore as ms
 import mindspore.numpy as msnp
 from mindspore import ops
 from mindspore import jit
-from mindspore.ops import function as F
-from mindspore import Tensor, Parameter, context
-from mindspore.ops._grad.grad_base import bprop_getters
-from mindspore.ops._utils.utils import generate_shape_index
-from mindspore.ops.composite.multitype_ops.zeros_like_impl import zeros_like
+from mindspore import Tensor, Parameter
 
 __all__ = [
     'PI',
     'inv',
     'keepdim_sum',
     'keepdim_mean',
     'keepdim_prod',
@@ -84,90 +80,15 @@
 keepdim_mean = ops.ReduceMean(keep_dims=True)
 keepdim_prod = ops.ReduceProd(keep_dims=True)
 reduce_any = ops.ReduceAny()
 reduce_all = ops.ReduceAll()
 concat_last_dim = ops.Concat(-1)
 concat_penulti = ops.Concat(-2)
 identity = ops.Identity()
-dyn_shape_op = ops.TensorShape()
-unsorted_segment_sum = ops.UnsortedSegmentSum()
-
-
-@bprop_getters.register(ops.Slice)
-def get_bprop_slice(self):
-    """Bprop for slice"""
-    # pylint: disable=W0613
-    concat = ops.Concat(axis=2)
-    def bprop(x, begin, size, out, dout):
-        # pylint: disable=W0613
-        dtype = x.dtype
-        begin = begin[-1]
-        size = size[-1]
-        if begin != 0:
-            left_tensor = ops.zeros(x.shape[:-1] + (begin,), dtype)
-            dout = concat((left_tensor, dout))
-        shape = x.shape[-1]
-        if shape != begin + size:
-            right_tensor = ops.zeros(x.shape[:-1] + (shape - begin - size,), dtype)
-            dout = concat((dout, right_tensor))
-        return (dout, zeros_like(begin), zeros_like(size))
-
-    return bprop
-
-
-def _generate_inverse_index(x_shape, axis):
-    x_rank = len(x_shape)
-    index = tuple(range(x_rank))
-    if axis < 0:
-        axis += x_rank
-    perm = index[1:1 + axis] + (0,) + index[1 + axis:]
-    return perm
-
-
-def _regenerate_output_shape(x_shp, ind_shp, axis):
-    rank = len(x_shp)
-    if axis < 0:
-        axis += rank
-    out_shape = x_shp[:axis] + ind_shp + x_shp[axis + 1:]
-    return out_shape
-
-
-class GatherNet(ms.nn.Cell):
-    """Redefine bprop for gather to run unsorted_segment_sum on aicpu"""
-    def construct(self, data, indices, axis):
-        return ops.gather(data, indices, axis)
-
-    def bprop(x, indices, axis, out, dout):
-        """bprop for gather"""
-        # pylint: disable=E0213, W0613
-        orig_indices = indices
-        if ops.rank(dout) == 0:
-            dout = ops.ExpandDims()(dout, -1)
-        if ops.rank(indices) == 0:
-            indices = ops.ExpandDims()(indices, -1)
-            x_shp = ops.shape(x)
-            ind_shp = ops.shape(indices)
-            out_shp = _regenerate_output_shape(x_shp, ind_shp, axis)
-            dout = ops.reshape(dout, out_shp)
-
-        x_shp = ops.shape(x)
-        out_shp = ops.shape(dout)
-        ind_shp = ops.shape(indices)
-        perm_1 = generate_shape_index(out_shp, ind_shp, axis)
-        values_transpose = ops.transpose(dout, perm_1)
-        if F.is_sequence_value_unknown(ops.shape(x)):
-            params_grad = unsorted_segment_sum(values_transpose, indices, dyn_shape_op(x)[axis])
-        else:
-            params_grad = unsorted_segment_sum(values_transpose, indices, ops.shape(x)[axis])
-        perm_2 = _generate_inverse_index(x_shp, axis)
-        params_grad = ops.transpose(params_grad, perm_2)
-        return params_grad, zeros_like(orig_indices), zeros_like(axis)
-
-
-gather = GatherNet() if context.get_context("device_target") == "Ascend" else ops.Gather()
+gather = ops.Gather()
 
 
 @jit
 def norm_last_dim(vector: Tensor) -> Tensor:
     r"""Compute the norm of vector, delete the last dims
 
     Args:
```

## mindsponge/metrics/structure_violations.py

```diff
@@ -55,30 +55,32 @@
         tolerance_factor_hard=12.0
 ):
     """
     Flat-bottom loss to penalize structural violations between residues. This is a loss penalizing any violation
     of the geometry around the peptide bond between consecutive amino acids.
 
     Args:
-        pred_atom_positions (Tensor):  Atom positions in atom37/14 representation, shape :math:`(N_{res}, 37, 3)`.
-                                      or shape :math:`(N_{res}, 14, 3)` .
-        pred_atom_mask (Tensor):       Atom mask in atom37/14 representation. shape :math:`(N_{res}, 37)` or
-                                      shape :math:`(N_{res}, 14)` .
-        residue_index (Tensor):        Residue index for given amino acid, this is assumed to be monotonically
-                                      increasing. shape :math:`(N_{res}, )` .
-        aatype (Tensor):               amino acid types. shape :math:`(N_{res}, )` .
-        tolerance_factor_soft (float): soft tolerance factor measured in standard deviations of pdb distributions.
-                                      Default: 12.0 .
-        tolerance_factor_hard (float): hard tolerance factor measured in standard deviations of pdb distributions.
-                                      Default: 12.0 .
+        pred_atom_positions (Tensor):   Atom positions in atom37/14 representation, shape :math:`(N_{res}, 37, 3)`.
+                                        or shape :math:`(N_{res}, 14, 3)` .
+        pred_atom_mask (Tensor):        Atom mask in atom37/14 representation. shape :math:`(N_{res}, 37)` or
+                                        shape :math:`(N_{res}, 14)` .
+        residue_index (Tensor):         Residue index for given amino acid, this is assumed to be monotonically
+                                        increasing. Range from 1 to :math:`N_{res}`. shape :math:`(N_{res}, )` .
+        aatype (Tensor):                amino acid types. Range is :math:`[0,20]`. shape :math:`(N_{res}, )` .
+        tolerance_factor_soft (float):  soft tolerance factor measured in standard deviations of pdb distributions.
+                                        Default: 12.0 .
+        tolerance_factor_hard (float):  hard tolerance factor measured in standard deviations of pdb distributions.
+                                        Default: 12.0 .
 
     Returns:
-        - Tensor, c_n_loss_mean, loss for peptide bond length violations. shape is () .
-        - Tensor, ca_c_n_loss_mean, loss for violations of bond angle around C spanned by CA, C, N. shape is () .
-        - Tensor, c_n_ca_loss_mean, loss for violations of bond angle around N spanned by C, N, CA. shape is () .
+        - Tensor, c_n_loss_mean, loss for peptide bond length violations. shape is :math:`( )` .
+        - Tensor, ca_c_n_loss_mean, loss for violations of bond angle around C spanned by CA, C, N.
+          shape is :math:`( )` .
+        - Tensor, c_n_ca_loss_mean, loss for violations of bond angle around N spanned by C, N, CA.
+          shape is :math:`( )` .
         - Tensor, per_residue_loss_sum, sum of all losses of each residue. shape is :math:`(N_{res}, )` .
         - Tensor, per_residue_violation_mask, mask denoting all residues with violation present.
           shape is :math:`(N_{res}, )` .
 
     Symbol:
         :math:`N_{res}`, number of amino acids.
 
@@ -199,24 +201,25 @@
 
     Args:
         atom14_pred_positions (Tensor): predicted positions of atoms in global prediction frame.
                                         shape is :math:`(N_{res}, 14, 3)` .
         atom14_atom_exists (Tensor):    mask denoting whether atom at positions exists for given amino acid type.
                                         shape is :math:`(N_{res}, 14)` .
         atom14_atom_radius (Tensor):    Van der Waals radius for each atom. shape is :math:`(N_{res}, 14)` .
-        residue_index (Tensor):         Residue index for given amino acid. shape is :math:`(N_{res}, )` .
+        residue_index (Tensor):         Residue index for given amino acid. shape is :math:`(N_{res}, )` ,
+                                        range from 1 to :math:`N_{res}` .
         c_one_hot (Tensor):             one hot encoding for C atoms (using atom14 representation). shape is (14, ) .
         n_one_hot (Tensor):             one hot encoding for N atoms (using atom14 representation). shape is (14, ) .
         overlap_tolerance_soft (float): soft tolerance factor. in default: 12.0.
         overlap_tolerance_hard (float): hard tolerance factor. in default: 1.5.
         cys_sg_idx (Tensor):            CYS amino acid index. Default: 5.
-                                        see more at `mindsponge.common.residue_constants`.
+                                        see more at `mindsponge.common.residue_constants`. Shape: `()` .
 
     Returns:
-        - Tensor, mean_loss, average clash loss. Shape is () .
+        - Tensor, mean_loss, average clash loss. Shape is `()` .
         - Tensor, per_atom_loss_sum, sum of all clash losses per atom, shape is :math:`(N_{res}, 14)` .
         - Tensor, per_atom_clash_mask, mask whether atom clashes with any other atom,
           shape is :math:`(N_{res}, 14)` .
 
     Symbol:
         :math:`N_{res}`, number of amino acids.
 
@@ -354,27 +357,30 @@
                               c_one_hot=C_ONE_HOT, n_one_hot=N_ONE_HOT, dists_mask_i=DISTS_MASK_I,
                               cys_sg_idx=CYS_SG_IDX):
     """Computes several checks for structural violations.
 
     Args:
         atom14_atom_exists (Tensor):        mask denoting whether atom at positions exists for given amino acid type.
                                             shape :math:`(N_{res}, 14)` .
-        residue_index (Tensor):             Residue index for given amino acid. shape :math:`(N_{res}, )` .
-        aatype (Tensor):                    amino acid types. shape :math:`(N_{res}, )` .
+        residue_index (Tensor):             Residue index for given amino acid range from 0 to :math:`N_{res} - 1`.
+                                            Shape :math:`(N_{res}, )` .
+        aatype (Tensor):                    amino acid types. shape :math:`(N_{res}, )` . Range is  :math:`[0,20]` .
         residx_atom14_to_atom37 (Tensor):   mapping for (residx, atom14) --> atom37. shape :math:`(N_{res}, 14)` .
         atom14_pred_positions (Tensor):     predicted positions of atoms in global prediction frame.
                                             shape :math:`(N_{res}, 14, 3)` .
         violation_tolerance_factor (float): violation between amino acid tolerance factor. Default: 12.0 .
         clash_overlap_tolerance (float):    clash overlap tolerance factor. Default: 1.5 .
         lower_bound (Tensor):               lower bond on allowed distances. shape :math:`(N_{res}, 14, 14)` .
         upper_bound (Tensor):               upper bond on allowed distances. shape :math:`(N_{res}, 14, 14)` .
-        atomtype_radius (Tensor):           Van der Waals radius for each amino acid. shape: (37, ) .
-        c_one_hot (Tensor):                 one hot encoding for C atoms (using atom14 representation). shape: (14, ) .
-        n_one_hot (Tensor):                 one hot encoding for N atoms (using atom14 representation). shape: (14, ) .
-        dists_mask_i (Tensor):              initial distants mask, shape: (14, 14) .
+        atomtype_radius (Tensor):           Van der Waals radius for each amino acid. shape: :math:`(37, )` .
+        c_one_hot (Tensor):                 one hot encoding for C atoms (using atom14 representation).
+                                            shape: :math:`(14, )` .
+        n_one_hot (Tensor):                 one hot encoding for N atoms (using atom14 representation).
+                                            shape: :math:`(14, )` .
+        dists_mask_i (Tensor):              initial distants mask, shape: :math:`(14, 14)` .
         cys_sg_idx (Tensor):                CYS amino acid index. Default: 5 .
                                             see more at `mindsponge.common.residue_constants`.
 
     Returns:
         - bonds_c_n_loss_mean (Tensor), loss for peptide bond length violations. shape is () .
         - angles_ca_c_n_loss_mean (Tensor), loss for violations of bond angle around C spanned by CA, C, N. shape is ().
         - angles_c_n_ca_loss_mean (Tensor), loss for violations of bond angle around N spanned by C, N, CA. shape is ().
@@ -581,29 +587,29 @@
                                   positions_mask,
                                   length_scale,
                                   l1_clamp_distance):
     r"""Measure point error under different alignments which computes error between two
     structures with B points under A alignments derived from the given pairs of frames.
     Similar with the `frame_aligned_point_error` function. The difference is this is a
     batched version which return batch error for each group of local frames individually,
-    this version considers only backbone frames.
+    this version considers only backbone frames :math:`C\alpha` .
 
     Args:
         pred_frames (list): The predicted backbone frames which is a 2-dimensional list,
             the first element of pred_frames is a list of 9 tensors which are the 9 components of
             rotation matrix; the second element of pred_frames is a list of 3 tensors are the 3
             component of translation matrix. All tensors are of shape :math:`(N_{recycle}, N_{res})`.
             with :math:`N_{recycle}` the recycle number of FoldIteration in Structure module, :math:`N_{res}` the
             number of residues in protein.
         target_frames (list): The ground truth backbone frames which is also a 2-dimensional
             list, the same as pred_frames except that the shape of tensors is :math:`(N_{res},)`.
         frames_mask (Tensor): The binary mask for frames of shape  :math:`(N_{res},)`.
-        pred_positions (list):  The predicted Ca atom positions which is a list of 3
+        pred_positions (list):  The predicted :math:`C\alpha` atom positions which is a list of 3
             tensors of shape :math:`(N_{recycle}, N_{res},)`.
-        target_positions (list):  The ground truth Ca atom positions which is a list
+        target_positions (list):  The ground truth :math:`C\alpha` atom positions which is a list
             of 3 tensors of shape :math:`(N_{res},)`.
         positions_mask (Tensor): The binary mask for Ca atom positions of shape :math:`(N_{res},)`.
         length_scale (float): The unit distance which is used to scale distances.
         l1_clamp_distance (float): Distance cutoff on error beyond which gradients will
             be zero.
 
     Returns:
@@ -722,33 +728,33 @@
     Backbone FAPE Loss using `frame_aligned_point_error_map` function.
     `Jumper et al. (2021) Suppl. Alg. 20 "StructureModule" line 17
     <https://static-content.springer.com/esm/art%3A10.1038%2Fs41586-021-03819-2/
     MediaObjects/41586_2021_3819_MOESM1_ESM.pdf>`_.
 
     Args:
         traj (Tensor): The series of backbone frames(trajectory) generated by Structure
-            module, the shape is :math:`(N_{recycle}, N_{res}, 7)` with :math:`(N_{recycle},)` the
-            recycle number of recycle in Structure module, :math:`(N_{res},)` the number of residues
+            module, the shape is :math:`(N_{recycle}, N_{res}, 7)` with :math:`N_{recycle}` the
+            recycle number of recycle in Structure module, :math:`N_{res}` the number of residues
             in protein, for the last dimension, the first 4 elements are the affine tensor which
             contains the rotation information, the last 3 elements are the translations in space.
         backbone_affine_tensor (Tensor): The ground truth backbone frames of shape :math:`(N_{res}, 7)`.
         backbone_affine_mask (Tensor): The binary mask for backbone frames of shape :math:`(N_{res},)`.
         fape_clamp_distance (float):  Distance cutoff on error beyond which gradients will
             be zero.
         fape_loss_unit_distance (float): The unit distance of backbone FAPE loss, used to scale
             distances.
         use_clamped_fape (float): The indicator that if backbone FAPE loss is clamped,
             0 or 1, 1 means clamping.
 
     Returns:
         - **fape** (Tensor) - Backbone FAPE loss (clamped if use_clamped_fape is 1) of last recycle
-          of Structure module with shape ().
+          of Structure module with shape :math:`()` .
         - **loss** (Tensor) - Averaged Backbone FAPE loss (clamped if use_clamped_fape is 1) of all recycle of
-          Structure module with shape ().
-        - **no_clamp** (Tensor) - Backbone FAPE loss of last recycle of Structure module with shape ().
+          Structure module with shape :math:`()` .
+        - **no_clamp** (Tensor) - Backbone FAPE loss of last recycle of Structure module with shape :math:`()` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> np.random.seed(0)
@@ -949,15 +955,15 @@
             are the 9 components of rotation matrix; the last 3 elements are the 3 component of
             translation matrix.
         rigidgroups_alt_gt_frames (Tensor): The alternative ground truth locals frames due to
             symmetry of amino acids. This tensor has the same shape as rigidgroups_gt_frames
         rigidgroups_gt_exists (Tensor): The binary mask for gt frames of shape :math:`(N_{res}, 8)`.
         renamed_atom14_gt_positions (Tensor): The mask for ground truth positions after renaming
             swaps are performed(swaps are needed for some amino acids due to symmetry
-            `compute_renamed_ground_truth`), its shape is :math:`(N_{res}, 14)`.It takes the 14-types
+            `compute_renamed_ground_truth`), its shape is :math:`(N_{res}, 14, 3)`.It takes the 14-types
             atoms encoding.
         renamed_atom14_gt_exists (Tensor): The mask for ground truth positions after renaming
             swap is performed after renaming swaps are performed, its shape is :math:`(N_{res}, 14)`.
         sidechain_atom_clamp_distance (float): Distance cutoff on error beyond which gradients
             will be zero.
         sidechain_length_scale (float): The unit distance of sidechain FAPE loss, used to scale
             distances.
@@ -965,15 +971,15 @@
             :math:`(N_{recycle},)` is the recycle number of FoldIteration in Structure module. Only the frames of
             last recycle is used in side-chain FAPE loss. 12 has the same meaning as the third dimension of
             rigidgroups_gt_frames.
         pred_positions (Tensor): The predicted positions of shape :math:`(3, N_{recycle}, N_{res}, 14)`.
             Only the positions of last recycle is used in side-chain FAPE loss, encoded atom-14 encoding.
 
     Returns:
-        Tensor, fape. Clamped side-chian FAPE loss with shape ().
+        Tensor, fape. Clamped side-chian FAPE loss with shape :math:`()`.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> np.random.seed(0)
@@ -1051,15 +1057,15 @@
         chi_weight (float): The weight of chi angle difference loss term, constant.
         angle_norm_weight (float): The weight of angle norm loss term, constant.
         chi_pi_periodic (Tensor): Chi angles that are pi periodic: they can be rotated
             by a multiple of pi without affecting the structure. Constants of residues of shape
             :math:`(21, 4)`, 20 types of amino acids + unknown.
 
     Returns:
-        - **loss** (Tensor) - Supervised chi angle loss with shape ().
+        - **loss** (Tensor) - Supervised chi angle loss with shape :math:`()` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> np.random.seed(0)
```

## Comparing `mindsponge_ascend-1.0.0a0.dist-info/METADATA` & `mindsponge_ascend-1.0.0rc1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsponge-ascend
-Version: 1.0.0a0
+Version: 1.0.0rc1
 Summary: simulation package of next generation molecular modeling in mindspore
 Home-page: https://www.mindspore.cn/
 Author: The MindSpore Authors
 Author-email: contact@mindspore.cn
 License: Apache 2.0
 Download-URL: https://gitee.com/mindspore/mindscience/tags
 Project-URL: Sources, https://gitee.com/mindspore/mindscience
```

