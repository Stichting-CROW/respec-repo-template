# GitHub Workflows

| file                                     | triggers                                       | desc                                                                       |
| ---------------------------------------- | ---------------------------------------------- | -------------------------------------------------------------------------- |
| [`setup.yaml`](setup.yaml)               | push                                           | on first clone, perform initialization; set repo / GH Pages configuration. |
| [`add-doc.yaml`](add-doc.yaml)           | workflow_dispatch                              | on request, add `im` to `main:docs/`                                       |
| [`auto-publish.yaml`](auto-publish.yaml) | push (`main`), workflow_dispatch, workflow_run | on push to `main`                                                          |
| [`lifecycle.yaml`](lifecycle.yaml)       | workflow_dispatch                              | on request, add `v/...` to `gh-pages:/`                                    |
| [`deploy.yaml`](deploy.yaml)             | workflow_run \*                                | trigger redeploy, report on what documents are served from `gh-pages:` .   |
