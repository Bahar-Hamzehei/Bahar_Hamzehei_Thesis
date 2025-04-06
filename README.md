<pre>
Marker code

np.str_('DC Correction/') 10001
np.str_('New Segment/')	99999

Block1:

Used Annotations descriptions: [np.str_('DC Correction/'), np.str_('New Segment/'), np.str_('Stimulus/S 11'), np.str_('Stimulus/S 12'), np.str_('Stimulus/S 13'), np.str_('Stimulus/S110'), np.str_('Stimulus/S114'), np.str_('Stimulus/S120'), np.str_('Stimulus/S124'), np.str_('Stimulus/S134')]

cs_code	shock	stim_marker number_of_times TMS_marker
csm 	no	       S 13		      20           S134
csp_l	left	     S 11		      14           S114
csp_r	right	     S 12		      14           S124
csp_r	no	       S120		      6            S124
csp_l	no	       S110		      6            S114



Block2:

Used Annotations descriptions: [np.str_('DC Correction/'), np.str_('New Segment/'), np.str_('Stimulus/S 21'), np.str_('Stimulus/S 22'), np.str_('Stimulus/S 23'), np.str_('Stimulus/S210'), np.str_('Stimulus/S214'), np.str_('Stimulus/S220'), np.str_('Stimulus/S224'), np.str_('Stimulus/S234')]

cs_code	shock	stim_marker number_of_times TMS_marker
csm 	no	       S 23		      20           S234
csp_l	left	     S 21		      14           S214
csp_r	right	     S 22		      14           S224
csp_r	no	       S220		      6            S224
csp_l	no	       S210		      6            S214

To label the data elements of the EEG data, you have to keep in mind that participants were seeing the colored circle from the stim_trigger to TMS_trigger




Information to figure out what colors corresponded to stim_marker for each participant
scenario 1 - Block 1
cs_code	shock	stim_marker number_of_times TMS_marker	color
csm 	no	       S 13		      20       S234	        yellow
csp_l	left	     S 11		      14       S214	        blue
csp_r	right	     S 12		      14       S224	        violet
csp_r	no	       S120		      6        S224	        violet
csp_l	no	       S110		      6        S214	        blue

scenario 2 - Block 1
cs_code	shock	stim_marker number_of_times TMS_marker	color
csm 	no	      S 13		      20        S234	    blue
csp_l	left	    S 11		      14        S214	    violet
csp_r	right	    S 12		      14        S224 	    yellow
csp_r	no	      S120		      6         S224	    yellow
csp_l	no	      S110		      6         S214	    violet

scenario 3 - Block 1
cs_code	shock	stim_marker number_of_times TMS_marker	color
csm 	no	       S 13		      20        S234	    violet
csp_l	left	     S 11		      14        S214	    yellow
csp_r	right	     S 12		      14        S224	    blue
csp_r	no	       S120		      6         S224	    blue
csp_l	no	       S110		      6         S214	    yellow

ID	Scenario
01ln	1
02gd	2
03as	3
04ep	1
05br	2
06nc	3
07fs	1
08am	2
09dm	3
10lc	1
11gb	2
12ag	3
13cg	1
14es	2
15kf	3
16gd	1
17st	2
18gf	3
19tm	1
20md	2
21es	3
22mc	1
23lp	2
24cs	3
25vt	1
26fs	2
27rv	3
28gv	1
29bc	2
</pre>
