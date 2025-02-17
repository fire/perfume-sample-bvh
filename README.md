# Perfume dance


## Extract Skeleton and VRM

1. The Blender scene is 30 fps
1. Use Blender 3.2
1. Import BVH at 0.01 scale and expand duration
1. Select armature
1. Export as glb with all influences and limited to selected
1. Use `perfume_vrm_mappings.json` to construct mappings.
1. Fill in meta information like copyright.
1. Apply `core/make_skeleton_mesh.py` script to generate mesh.
1. Export as vrm.

## Notes

Blender 3.2 is unstable with VRM. Try Blender 3.0 if necessary.

## Playback the animation

* go to the VRM and you copy the animation's retarget mapping 
* go to the animation glb 
* put the mapping onto the animation retarget setting and also the profile, and the skeleton path
* change retarget options as necessary. The default is global animation.
* go to the dance anim 
* go to the retarget track and select the extract? animation 
* select remove un shared tracks (I forget the exact dialog name) 
* copy the animation resource
* go to any vrm with the same profile
* copy the animation from the dance animation glb scene
* select the third person animation
* paste the anim track with the sharable 
* OPTIONAL - restore the retargeted animation (menu item) allows gltf export of the entire scene with the dance 
* play animation
