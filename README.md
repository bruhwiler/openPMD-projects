Projects using openPMD
----------------------

The following list of projects use the
[**openPMD** standard](https://github.com/openPMD/openPMD-standard)
to describe their data. For additional information, we list
third-party projects marked with a (`third party`) to acknowledge the
the work provided in those for our format handling.

### Documents

- [openPMD Standard](https://github.com/openPMD/openPMD-standard/blob/latest/STANDARD.md)
  - domain: the fundamental, technical documents that serve as a basis for the
            whole openPMD environment
  - maintainer and initial author: A Huebl @ax3l
  - contributions: [full list of contributors](https://github.com/openPMD/openPMD-standard/blob/latest/AUTHORS.md)
  - [repository](https://github.com/openPMD/openPMD-standard)
    ([CC-BY 4.0](https://github.com/openPMD/openPMD-standard/releases))
  - status:
    - [`1.0.0` released](https://github.com/openPMD/openPMD-standard/releases/tag/1.0.0),
      doi: [10.5281/zenodo.33624](https://dx.doi.org/10.5281/zenodo.33624)
    - [`1.0.1` released](https://github.com/openPMD/openPMD-standard/releases/tag/1.0.1),
      doi: [10.5281/zenodo.1069534](https://dx.doi.org/10.5281/zenodo.1069534)
    - [`1.1.0` released](https://github.com/openPMD/openPMD-standard/releases/tag/1.1.0),
      doi: [10.5281/zenodo.1167843](https://doi.org/10.5281/zenodo.1167843)
    - [`2.0.0` in progress](https://github.com/openPMD/openPMD-standard/projects/3)


### Scientific Simulations

- [PIConGPU](http://picongpu.hzdr.de) (HZDR, Germany)
  - domain: electro-dynamic particle-in-cell code
  - [repository](https://github.com/ComputationalRadiationPhysics/picongpu) (GPLv3+/LGPLv3+)
  - maintainers: A Huebl @ax3l, M Bussmann @bussmann et al.
  - status: implemented (base standard + ED-PIC)

- [Warp](http://warp.lbl.gov) (LBNL & LLNL, United States)
  - domain: electro-dynamic/static particle-in-cell code
  - [repository](https://bitbucket.org/berkeleylab/warp) (BSD-3-Clause-LBNL)
  - maintainers: JL Vay @jlvay, D Grote @dpgrote, R Lehe @RemiLehe et al.
  - status: implemented (base standard + ED-PIC)

- [FBPIC](http://fbpic.github.io) (LBNL, CFEL Hamburg University)
  - domain: electro-dynamic particle-in-cell code with spetral solver and
            Fourier-Bessel decomposition in cylindrical geometry
  - [repository](https://github.com/fbpic/fbpic) (BSD-3-Clause-LBNL)
  - maintainers: R Lehe @RemiLehe, M Kirchen @MKirchen et al.
  - status: implemented (base standard + ED-PIC)

- SIMEX Platform (EUCALL, European XFEL)
  - domain: software platform for simulation of advanced photon experiments
  - [repository](https://github.com/eucall-software/simex_platform) (GPLv3+)
  - maintainer: C Fortmann-Grote @CFGrote
  - status: implemented (base standard)

- ParaTAXIS (HZDR, Germany)
  - domain: parallel tracer for arbitrary X-ray interaction and scattering
  - [repository](https://github.com/ComputationalRadiationPhysics/parataxis) (GPLv3+)
  - maintainers: M Bussmann @bussmann et al.
  - original author: A Grund @Flamefire
  - status: implemented (base standard for X-ray laser & density profiles)

- OSIRIS (UCLA, USA and IST, Portugal)
  - domain: electro-dynamic particle-in-cell code
  - repository: closed, available through MoU
  - maintainers: OSIRIS Consortium (UCLA/IST)
  - original author: R G Hemker (UCLA)
  - an openPMD fork for OSIRIS 4.0 is available from UCLA; existing grid data
    can be converted from the previous OSIRIS file format to openPMD format by
    using the python library https://github.com/Wen-Han/pyVisOS

- UPIC-Emma (UCLA, USA)
  - domain: 2-1/2D electromagnetic particle-in-cell code
  - [repository](https://github.com/UCLA-Plasma-Simulation-Group/upic-emma-2.0) (UCLA-NC)
  - maintainer: F Tsung @tsung1029
  - original author: V Decyk
  - status: implemented

### Data Processing and Visualization

- [openPMD-viewer](https://github.com/openPMD/openPMD-viewer) (LBNL, CFEL Hamburg University)
  - domain: high level python api and interactive IPython notebook GUI
  - [repository](https://github.com/openPMD/openPMD-viewer) (BSD-3-Clause-LBNL)
  - maintainer: R Lehe @RemiLehe et al.
  - status: implemented

- [yt project](http://yt-project.org) ([Members](http://yt-project.org/members.html), `third party`)
  - domain: analysis and visualization
  - [repository](https://github.com/yt-project/yt) (BSD-3-Clause)
  - [openPMD tutorial](https://gist.github.com/C0nsultant/5808d5f61b271b8f969d5c09f5ca91dc)
  - [openPMD wishlist/issue tracker](https://bitbucket.org/C0nsultant/openpmd/issues)
  - maintainers: [yt project members](http://yt-project.org/members.html)
                 (HZDR: openPMD reader contribution by @C0nsultant)
  - status:
    - 3.4.0+: implemented (HDF5 reader for base standard: 1.0.0-1.0.1)
    - 3.5.0+: upcoming (HDF5 reader for base standard: 1.0.0-1.1.0)

- [VisIt](https://visit.llnl.gov) (LLNL, `third party`)
  - domain: analysis and visualization
  - [repository](http://www.visitusers.org/index.php?title=Version_Control) (BSD-3-Clause)
  - [plugin repository](https://github.com/openPMD/openPMD-visit-plugin) (BSD-3-Clause-LBNL)
  - maintainers: VisIt collaborators
    (LBNL: reader plugin contribution by M Lobet @xxirii, ORNL: support by D Pugmire)
  - status: implemented HDF5 reader plugin (ADIOS planned) for base standard

- [ParaView](https://www.paraview.org/) (Kitware, `third party`)
  - domain: analysis and visualization
  - [repository](https://gitlab.kitware.com/paraview/paraview) (BSD-3-Clause)
  - [plugin repository](https://github.com/jfavre/ParaViewDev)
  - maintainers: Kitware
    (CSCS: reader plugin contribution by J Favre @jfavre)
  - status: implementing an ADIOS1 reader plugin (HDF5 planned) for base standard

- [postpic](https://github.com/skuschel/postpic) (U Jena, Germany)
  - domain: post-processing and visualization tool for particle-in-cell data
  - [repository](https://github.com/skuschel/postpic) (GPLv3+)
  - maintainer: S Kuschel @skuschel
  - status: implemented (HDF5 reader for base standard + ED-PIC)

Note: For third-party frameworks, the general idea is to implement our readers
[upstream](https://en.wikipedia.org/wiki/Upstream_%28software_development%29)
as soon as they are working.

Please check the individual repositories and feel free to contribute.

### Libraries

- [openPMD-api](https://openpmd-api.readthedocs.io/) (HZDR, Germany)
  - domain: C++ & Python API for writing & reading (H5, BP, ...), serial & parallel (MPI)
  - [repository](https://github.com/openPMD/openPMD-api) (LGPLv3+)
  - maintainers: F Koller @C0nsultant, A Huebl @ax3l
  - status:
    - implemented: HDF5 serial & parallel C++ API for base standard (1.0.0 - 1.1.0)
    - first stable release soon
  - will supersede our legacy C++ library:
    - [libSplash](https://github.com/ComputationalRadiationPhysics/libSplash) (TU Dresden/HZDR, Germany)
      - domain: high-level C++ HDF5 library for mesh and particle records
      - [repository](https://github.com/ComputationalRadiationPhysics/libSplash) (LGPLv3+)
      - maintainers: F Schmitt @f-schmitt-zih, A Huebl @ax3l
      - status:
        - 1.4.0+: full API available to fulfill the standard (read+write)

- [Fortran openPMD writer](https://github.com/UCLA-Plasma-Simulation-Group/Fortran-OpenPMD-File-Writers) (UCLA, USA)
  - domain: Fortran 2003 HDF5 File Writers in openPMD Standard
  - [repository](https://github.com/UCLA-Plasma-Simulation-Group/Fortran-OpenPMD-File-Writers) (UCLA-NC)
  - maintainer: Weiming An @caozigao
  - status: openPMD 1.0 implemented

- [HDF5](https://www.hdfgroup.org/HDF5/) (`third party`)
  - domain: libraries for reading & writing the HDF5 format C/C++/Fortran
  - maintainer: HDF Group

- [ADIOS](https://www.olcf.ornl.gov/center-projects/adios/) (ORNL, United States; `third party`)
  - domain: libraries for reading & writing the HDF5 format C/C++/Fortran/Java/Python
  - [repository](https://github.com/ornladios/ADIOS) (BSD-3-Clause-DOE)
  - maintainers: N Podhorszki @pnobert, S Klasky @sklasky at al.

- [h5py](http://www.h5py.org/) (`third party`)
  - domain: python bindings for HDF5
  - [repository](https://github.com/h5py/h5py)
  - maintainer: A Collette @andrewcollette et al.

### Tools & Converters

Please be aware that *all existing tools* for general file handling
(HDF5, ADIOS, ...) are also usable with openPMD flavoured files!

A non-complete list of third party software for your consideration:

- openPMD-validator (HZDR, LBNL)
  - domain: scripts and python module to validate files according to the `openPMD standard`
  - [repository](https://github.com/openPMD/openPMD-validator) (ISC)
  - maintainers: A Huebl @ax3l, R Lehe @RemiLehe
  - status: implemented (base standard + ED-PIC)

- openPMD-updater (HZDR, LBNL)
  - domain: scripts and python module to update openPMD files to newer versions of the `openPMD standard`
  - [repository](https://github.com/openPMD/openPMD-updater) (ISC)
  - maintainers: A Huebl @ax3l, R Lehe @RemiLehe
  - status: currently implementing update routines for openPMD 1.0/1.1 to (upcoming) openPMD 2.0

- openPMD-converter
  - domain: copy converters from and to openPMD, e.g. for tools/frameworks/applications without native openPMD support
  - [repository](https://github.com/openPMD/openPMD-converter)
  - maintainers: various

- [HDF Compass](https://github.com/HDFGroup/hdf-compass) (HDF Group; `third party`)
  - domain: viewer for HDF5 and related formats
  - [repository](https://github.com/HDFGroup/hdf-compass) (BSD-3-Clause-HDF)
  - [development repository](https://github.com/ComputationalRadiationPhysics/hdf-compass)
    (our fork for ADIOS support)
  - maintainer: HDF Group (HZDR: ADIOS reader contribution by @michaelsippel)
  - status: HZDR implemented an
            [ADIOS reader](https://github.com/ComputationalRadiationPhysics/hdf-compass)

- [HDFView](https://www.hdfgroup.org/products/java/hdfview/) (HDF Group; `third party`)
  - domain: viewer for HDF5
  - maintainer: HDF Group
  - [download](https://www.hdfgroup.org/products/java/hdfview/) (BSD-3-Clause-HDF)

- HDF5 command line tools (HDF Group; `third party`)
  - domain: HDF5 file handling
  - maintainer: HDF Group
  - examples: `h5ls`, `h5dump`, `h5diff`, `h5repack`, `gif2h5`, ...

- ADIOS command line tools (ORNL, United States; `third party`)
  - domain: ADIOS file handling
  - maintainers: N Podhorszki @pnorbert, S Klasky @sklasky et al.
  - examples: `bpls`, `bpdump`, `bpdiff`, `bp2bp`, `bp2h5`, ...

- [png2gas](https://github.com/ComputationalRadiationPhysics/picongpu/tree/master/src/tools/png2gas) (HZDR, Germany)
  - domain: convert a 2D png image into a 3D density profile,
            useful for particle-in-cell simulations
  - [repository](https://github.com/ComputationalRadiationPhysics/picongpu/tree/master/src/tools/png2gas) (GPLv3+)
  - maintainer: originally by PIConGPU team
  - status: [needs adjustments for openPMD 1.0.0](https://github.com/ComputationalRadiationPhysics/picongpu/issues/1446)

