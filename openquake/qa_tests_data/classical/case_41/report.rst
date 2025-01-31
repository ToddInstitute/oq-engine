PEER 2015 Validation Project, Set 3, Test 3.1a as Characteristic Source w/SERA Site Amplification Models
========================================================================================================

============== ===================
checksum32     2,245,592,391      
date           2019-10-02T10:07:34
engine_version 3.8.0-git6f03622c6e
============== ===================

num_sites = 2, num_levels = 12, num_rlzs = 6

Parameters
----------
=============================== ==================
calculation_mode                'preclassical'    
number_of_logic_tree_samples    0                 
maximum_distance                {'default': 200.0}
investigation_time              1.0               
ses_per_logic_tree_path         1                 
truncation_level                3.0               
rupture_mesh_spacing            2.0               
complex_fault_mesh_spacing      2.0               
width_of_mfd_bin                0.0001            
area_source_discretization      5.0               
ground_motion_correlation_model None              
minimum_intensity               {}                
random_seed                     1                 
master_seed                     0                 
ses_seed                        42                
=============================== ==================

Input files
-----------
======================= ======================================================================
Name                    File                                                                  
======================= ======================================================================
gsim_logic_tree         `gmpe_logic_tree_site_amp.xml <gmpe_logic_tree_site_amp.xml>`_        
job_ini                 `job.ini <job.ini>`_                                                  
site_model              `site_model.xml <site_model.xml>`_                                    
source_model_logic_tree `peer_source_model_logic_tree.xml <peer_source_model_logic_tree.xml>`_
======================= ======================================================================

Composite source model
----------------------
========= ======= =============== ================
smlt_path weight  gsim_logic_tree num_realizations
========= ======= =============== ================
PEERBend  1.00000 simple(6)       6               
========= ======= =============== ================

Required parameters per tectonic region type
--------------------------------------------
====== ===================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================== ========= ====================================================== ==============
grp_id gsims                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 distances siteparams                                             ruptparams    
====== ===================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================== ========= ====================================================== ==============
0      '[Eurocode8AmplificationDefault]\ngmpe_name = "KothaEtAl2019SERA"' '[Eurocode8Amplification]\ngmpe_name = "KothaEtAl2019SERA"' '[KothaEtAl2019SERASlopeGeology]' '[KothaEtAl2019SERA]' '[PitilakisEtAl2018]\ngmpe_name = "KothaEtAl2019SERA"' '[SandikkayaDinsever2018]\ngmpe_name = "KothaEtAl2019SERA"\n[SandikkayaDinsever2018.phi_0]\n"PGV" = 0.483487360873615\n"PGA" = 0.510861957895391\n"SA(0.01)" = 0.510104205329196\n"SA(0.025)" = 0.512392066661141\n"SA(0.04)" = 0.518461715489209\n"SA(0.05)" = 0.524129983454523\n"SA(0.07)" = 0.527258463232455\n"SA(0.1)" =  0.534721815465482\n"SA(0.15)" = 0.536676157950607\n"SA(0.2)" = 0.53218876544647\n"SA(0.25)" = 0.526995694991015\n"SA(0.3)" = 0.521904513113003\n"SA(0.35)" = 0.517473487991425\n"SA(0.4)" = 0.510214230044972\n"SA(0.45)" = 0.503982756931627\n"SA(0.5)" = 0.496744390517092\n"SA(0.6)" = 0.485887400763896\n"SA(0.7)" = 0.477975448246383\n"SA(0.75)" = 0.47483174831358\n"SA(0.8)" = 0.470675816183951\n"SA(0.9)" = 0.461879366570655\n"SA(1.0)" = 0.455552800346687\n"SA(1.2)" = 0.44487835024961\n"SA(1.4)" = 0.436849421688952\n"SA(1.6)" = 0.431989239017968\n"SA(1.8)" = 0.428737629779977\n"SA(2.0)" = 0.427120153573043\n"SA(2.5)" = 0.425817651524798\n"SA(3.0)" = 0.422252639239821\n"SA(3.5)" = 0.421148406228811\n"SA(4.0)" = 0.42300333740049\n"SA(4.5)" = 0.408704987873161\n"SA(5.0)" = 0.409277420621721\n"SA(6.0)" = 0.401597199934827\n"SA(7.0)" = 0.401052676368561\n"SA(8.0)" = 0.401323166589614' rjb       ec8 ec8_p18 geology h800 slope vs30 vs30measured z1pt0 hypo_depth mag
====== ===================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================== ========= ====================================================== ==============

Realizations per (GRP, GSIM)
----------------------------

::

  <RlzsAssoc(size=36, rlzs=6)>

Number of ruptures per source group
-----------------------------------
====== ========= ============ ============
grp_id num_sites num_ruptures eff_ruptures
====== ========= ============ ============
0      2.00000   1            1.00000     
====== ========= ============ ============

Slowest sources
---------------
======================= ====== ==== ============ ========= ========= ============
source_id               grp_id code num_ruptures calc_time num_sites eff_ruptures
======================= ====== ==== ============ ========= ========= ============
PEERWestDipBendingFault 0      X    1            0.00250   2.00000   1.00000     
======================= ====== ==== ============ ========= ========= ============

Computation times by source typology
------------------------------------
==== ========= ======
code calc_time counts
==== ========= ======
X    0.00250   1     
==== ========= ======

Information about the tasks
---------------------------
================== ======= ====== ======= ======= =======
operation-duration mean    stddev min     max     outputs
SourceReader       0.01190 NaN    0.01190 0.01190 1      
preclassical       0.00303 NaN    0.00303 0.00303 1      
================== ======= ====== ======= ======= =======

Data transfer
-------------
============ ======================================= ========
task         sent                                    received
SourceReader                                         10.6 KB 
preclassical srcs=7.28 KB gsims=3.88 KB params=660 B 342 B   
============ ======================================= ========

Slowest operations
------------------
====================== ========= ========= ======
calc_29525             time_sec  memory_mb counts
====================== ========= ========= ======
composite source model 0.02478   0.0       1     
total SourceReader     0.01190   0.0       1     
total preclassical     0.00303   0.0       1     
store source_info      0.00247   0.0       1     
aggregate curves       2.480E-04 0.0       1     
====================== ========= ========= ======