From:nfcore/base
Bootstrap:docker

%labels
    DESCRIPTION Singularity image containing all requirements for the nf-core/roary pipeline
    VERSION 1.0dev

%environment
    PATH=/opt/conda/envs/nf-core-roary-1.0dev/bin:$PATH
    export PATH

%files
    environment.yml /

%post
    /opt/conda/bin/conda env create -f /environment.yml
    /opt/conda/bin/conda clean -a
