# 3D Gaussian Splatting for Real-Time Radiance Field Rendering For C Kernel mainly on CPU

```shell
# clone
git clone git@github.com:graphdeco-inria/gaussian-splatting.git --recursive
# env
conda env create -f environment.yml
# 
pip install -e ./submodules/diff-gaussian-rasterization
pip install -e ./submodules/simple-knn

# Download models and db
...

# render
python render.py -m models/drjohnson/ -s db/drjohnson/ --data_device cpu --resolution 100
python metrics.py -m models/drjohnson/
```