# PCC Generator tool
<p>
The code creates Combinatorial Discrete Cell Complexes and related measures based on the <a href="https://neper.info/" target="_blank"> Neper </a> output '*.tess' files of 2D/3D space tessellations.
</p>

<p>
Combinatorial (../combinatorial/):
'number_of_cells' - numbers of 0-cells (first line), 1-cells (second line), 2-cells (third line) and 3-cells (fourth line) in the PCC
'vertex_set' - a simple list of vertex IDs
'edge_set'  - a list of edges represented as a couples of vertex IDs written in each line
'face_set'  - a list of faces represented as a sets of vert IDs written in each line
'grain_set'  - a list of grains represented as a set of vertex IDs written in each line

Boundaries:
'node_tboundaries' - 0-cells belonging to the tessellation geometric bounbdaries
'edge_tboundaries' - 0-cells belonging to the tessellation geometric bounbdaries
'face_tboundaries' - 0-cells belonging to the tessellation geometric bounbdaries
'grain_tboundaries' - 0-cells belonging to the tessellation geometric bounbdaries

Adjacency matrices (../algebraic/):
'A0' - adjacency 0-cells x 0-cells  sparse matrix
'D0' - diagonal degree matrix of 0-cells (contains number of neighbours for each 0-cell)
'A1' - adjacency 1-cells x 1-cells sparse matrix\
'D1' - diagonal degree matrix of 1-cells (contains number of neighbours for each 1-cell)
'A2' - adjacency 2-cells x 2-cells sparse matrix
'D2' - diagonal degree matrix of 2-cells (contains number of neighbours for each 2-cell)
'A3' - adjacency 3-cells x 3-cells sparse matrix
'D3' - diagonal degree matrix of 3-cells (contains number of neighbours for each 3-cell)

Incidence matrices(../algebraic/):
'B1' - incidence 1-cells x 0-cells sparse matrix
'B2' - incidence 2-cells x 1-cells sparse matrix
'B3' - incidence 3-cells x 2-cells sparse matrix

Coordinates (../coordinates/):
'vertex_seeds' - vertices Cartesian coordinates from the initial tessellation of space
'edge_barycenter_seeds' - edges Cartesian coordinates from the initial tessellation of space
'face_barycenter_seeds' - faces Cartesian coordinates from the initial tessellation of space
'volume_barycenter_seeds' - polyhedra Cartesian coordinates from the initial tessellation of space

Measures (../measures/):
'edge_lengths' - lengths of edges from the initial tessellation of space
'face_areas' - areas of faces from the initial tessellation of space
'grain_volumes' - areas of faces from the initial tessellation of space

Other (../other/):
'face_normals' - normal vector to each face in the initial tessellation of space

Tessellation (../tessellation/):
'initial_Neper_tessellation' - jpg figure with the initial tessellation of space]
'*.tess' - Neper (https://neper.info/) output file containing the initial tessellation of space

Reference configurations (../design_vectors/):
Random (../references/random/):
'special_grains' - random based sequence of special grains (3-cells) in the PCC 
'special_faces' - random based sequence of special faces (2-cells) in the PCC 
'special_edges' - random based sequence of special edges (1-cells) in the PCC 
'special_nodes' - random based sequence of special nodes (0-cells) in the PCC 

S_max  (../references/Smax/):
'special_grains' - maximum configuration entropy production principle (MEPP) based sequence of special grains (3-cells) in the PCC 
'special_faces' -  maximum configuration entropy production principle (MEPP) based sequence of special faces (2-cells) in the PCC 
'special_edges' -  maximum configuration entropy production principle (MEPP) based sequence of special edges (1-cells) in the PCC 
'special_nodes' -  maximum configuration entropy production principle (MEPP) based sequence of special nodes (0-cells) in the PCC 

S_min  (../references/S_min/):
'special_grains' -  minimum configuration entropy production principle (MIEPP) based sequence of special grains (3-cells) in the PCC 
'special_faces' - minimum configuration entropy production principle (MIEPP) based sequence of special faces (2-cells) in the PCC 
'special_edges' - minimum configuration entropy production principle (MIEPP) based sequence of special edges (1-cells) in the PCC 
'special_nodes' - minimum configuration entropy production principle (MIEPP) based sequence of special nodes (0-cells) in the PCC 
</p>
