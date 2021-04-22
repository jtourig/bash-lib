# bash-lib utils/

executable convenince scripts, mostly for working on the cluster

## jbatch / jrun

**Tired of copy-pasta-ing Slurm directives to all of your job scripts?  Can't be bothered to remember all the command line options?**

`jbatch` wraps `sbatch` and will set some sane defaults, prepending the directives to your job script before submitting them to half a node in the general queue (allocations can be overridden with `sbatch` options - see `jbatch --help` for more info)

`jrun` does much the same with `srun` for running interacting jobs on [Carbonate](https://kb.iu.edu/d/aolp), with options for low / med / high / whole node requests - run `jrun -h` for details.