# b0_atlas_coreg_app

This is a dummy repo so singularity hub can host the singularity container.

[Docker Hub](https://hub.docker.com/r/justinblaber/b0_atlas_coreg_app/tags/)

[Singularity Hub](https://www.singularity-hub.org/collections/3093)

# Run Instructions:
For docker:
```
sudo docker run --rm \
-v $(pwd)/INPUTS/:/INPUTS/ \
-v $(pwd)/OUTPUTS:/OUTPUTS/ \
--user $(id -u):$(id -g) \ls
justinblaber/b0_atlas_coreg
```
For singularity:
```
singularity run -e \
-B INPUTS/:/INPUTS \
-B OUTPUTS/:/OUTPUTS \
shub://justinblaber/b0_atlas_coreg_app
