BootStrap:docker
From:tensorflow/tensorflow:1.0.1-gpu

%runscript
  exec pip list

%post
  # Enables access to ACCRE storage
  mkdir /scratch /data /gpfs22 /gpfs23 /dors
  pip install keras


%test
  python -c "import tensorflow; import keras"

