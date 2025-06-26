--------------------- CASTpFold server results ---------------------
The results were downloaded from the CASTpFold server (https://cfold.bme.uic.edu/castpfold/).
Please cite the paper below if you used the CASTpFold server in your research or project:

Bowei et al., CASTpFold: Computed Atlas of Surface Topography of the universe of protein Folds.

Your citation is important for us.

--------------------------------------------------------------------

Description of files

.pdb
	The original pdb file used for pocket computation.

.mouth
	The atoms form the mouth of each pocket.
	The characters 1 to 66 of each line in the .mouth file are exactly the data of the corresponding atoms in .pdb file.
	The column after the character 66 shows the pocket id of the atoms.

.poc
	The atoms form each pocket.
	The format is the same as .mouth file

.mouthInfo
	The mouth information of each pockt.
		ID: pocket id
		N_mth: the number of mouths that this pocket has
		Area_sa: the total area of the mouths; calculated using the solvent accessible way
		Area_ms: the total area of the mouths; calculated using the vdw radius
		Len_sa: the total length of the perimeter of the mouths; calculated using the solvent accessible way
		Len_ms: the total length of the perimeter of the mouths; calculated using the vdw radius
		Ntri: not useful for end-users (the total number of triangles of the mouths)

.pocInfo
	The information of each pockt.
	The meaning of columns are almost same with those in .mouthInfo file, except the following
		Lenth: not useful for end-users (sum of arc length where two pocket atoms i, j  meet (the alpha value of this edge ij < 0))
		cnr: not useful for end-users (number of surface triangles excluding the mouth triangles)

.4.contrib.csv
	The absolute values and ratios of atom-level surface exposed areas and volumes for both SA and MS model 
	
.bulb.json
	Not for general user, which is used for display the red imprint on CASTpFold

--------------------------------------------------------------------
Local visualization
The pocket results can be visualized using either our PyMol plugin CASTpFoldMOL (https://cfold.bme.uic.edu/castpfold/about?localvisul)
or UCSF Chimera (https://www.cgl.ucsf.edu/chimera/)


