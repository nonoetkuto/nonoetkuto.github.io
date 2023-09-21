# Nono et Kuto - L'actualité e-sport (draft)

## Installation procedure & content management

### Install Hugo using winget
```shell
winget install Hugo.hugo.Extended
hugo --version # Check if hugo is correctly installed
```

Once hugo is installed, checkout the git repository on your machine.

### Run locally
```shell
cd <project_dir>
hugo server
# or
hugo server -D # Run locally with content marked as draft
```

### Create a blog post
```shell
cd <project_dir>
hugo new content posts/<blogpost_dir>/index.md
```

`blogpost_dir` must be named as following: `YYYYMMDD-your-project-title`

For example:
- `20160107-lancement-nk`
- `20170922-test-nentendo-switch`
- `20230921-lideal-cest-de-niro`

`index.md` will be the content of your blog post.