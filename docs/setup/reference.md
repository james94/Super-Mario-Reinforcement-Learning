# Environment Setup Reference

## Anaconda

Create a **super-mario-rl** conda environment provisioned with all libraries to run this program:

~~~bash
conda env create -f environment-gpu.yml
~~~

> **Note**: if you don't have access to a gpu, then run `environment.yml`

Verify **super-mario-rl** environment exists in your environments:

~~~bash
conda info --envs
~~~

Cleanup downloaded libraries (remove tarballs, zip files, etc):

~~~bash
conda clean -tp
~~~

Activate the **super-mario-rl** environment:

~~~bash
conda activate super-mario-r1
~~~

If you install new packages into your anaconda environment, export your environment:

~~~
(super-mario-rl) % conda env export --file environment.yml
~~~

This will make your work reproducible for others.

Deactivate the **super-mario-rl** environment:

~~~bash
conda deactivate
~~~

Remove **super-mario-rl** environment:

~~~bash
conda remove --name super-mario-rl --all
~~~

### Anaconda Further Reading

- [Managing Environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
