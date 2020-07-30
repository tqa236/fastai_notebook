# fastai_notebook

My notebooks for the FastAI course

<https://github.com/fastai/course-v3> is added as a submodule to keep the notebooks up-to-date.

To compare 2 notebook folders:

```console
git diff --no-index nbs course-v3/nbs
nbdiff nbs/dl1/00_notebook_tutorial.ipynb course-v3/nbs/dl1/00_notebook_tutorial.ipynb
```

## Build Docker image

```bash
docker build --tag train .
docker run -it -p 8888:8888 -v "$PWD":/workspace/fastai --rm train bash
```
