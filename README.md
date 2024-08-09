# Handbuch Proto4DigEd: Prototypische Workflows für digitale wissenschaftliche Editionen (DSE)

Zum [Handbuch zur Erstellung einer digitalen Edition](https://digital-editions.pages.uzh.ch/proto4diged/handbook)

## Run mkdocs on your local machine

If you have Python (with PIP) and Git available on your machine, you can easily set up mkdocs to run on localhost.
This guide focuses on UNIX systems but it is also possible to install on Windows machines.

### 1. Clone the repository

To copy the repository, paste the following command into your terminal in the directory where you want the code for this repository:

```bash
git clone git@gitlab.uzh.ch:digital-editions/proto4diged/handbook.git
```

You may need to import an SSH key into your user account, as described in the [Gitlab documentation](https://docs.gitlab.com/ee/user/ssh.html).

### 2. Set up an environment for your installation

To avoid conflicts with other Python projects, we recommend using a local environment. Theoretically this step can be skipped.

Create an environment with:

```bash
python3 -m venv venv
```

Activate the invironment with:

```bash
source venv/bin/activate
```

### 3. Install the dependencies

The needed Python packages are defined in `requirements.txt`. You can install them with:

```bash
pip3 install -r requirements.txt
```

### 4. Check out the branch you want to see

GitLab Pages at UZH will only run the `master` branch. To view other branches, you will have to check them out with:

```bash
git checkout developer
```

### 5. Start the local server

Start `mkdocs` with:

```bash
mkdocs serve
```

Open a browser on [http://localhost:8000](http://localhost:8000).

### Update your local code

When others have contributed to the repository, update your code with with your preferred branch already checked out:

```bash
git pull
```

## Contribute to the repository

New content to the handbook has to be added to a feature resp. development branch. Its content can be
added to the `master` branch via merge request, where it will be reviewed.
