BootStrap:docker
From:tensorflow/tensorflow:1.0.1-gpu

%runscript
  exec python "$@" 

%post
  # Enables access to ACCRE storage
  mkdir /scratch /data /gpfs22 /gpfs23 /dors
  
  pip install dill h5py hyperopt keras pandas \
    protobuf pymongo scikit-learn seaborn

%test
  python -c "import tensorflow; import keras"

