# Perfume dance


## Extract Skeleton and VRM

1. The Blender scene is 30 fps
1. Use Blender 3.2
1. Import BVH at 0.01 scale and expand duration
1. Select armature
1. Export as glb with all influences and limited to selected
1. Use `perfume_vrm_mappings.json` to construct mappings.
1. Fill in copyright.
1. Apply `core/make_skeleton_mesh.py` script to generate mesh.
1. Export as vrm.