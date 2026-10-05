Step 1 — Get the starter repository (individual)
1. Open the starter repository link from the LMS and click Use this template → Create a new repository (or Fork). Name it lab01-<github-username>. 2. Clone your copy: $ mkdir -p ~/projects/csc10014 && cd ~/projects/csc10014
$ git clone git@github.com:<you>/lab01-<you>.git
$ cd lab01-<you>
Step 2 — Create the environment $ python -m venv .venv
$ source .venv/bin/activate # Windows: .venv\Scripts\Activate.ps1
Step 3 — Install dependencies
(.venv) $ pip install -r requirements.txt
(.venv) $ pip install -e .
Step 4 — Run the starter app and the tests
(.venv) $ python -m assistant "where is the IT helpdesk?"
(.venv) $ pytest -q
Write down every command that worked — you need them in Step 5.
Step 5 — Add .gitignore and write the README
1. Create .gitignore (Part E.2). Run git status — .venv/ must not appear. 2. Replace every TODO in README.md with real instructions (Part F). 3. Run python scripts/check_env.py until every line is [ OK ].
Step 6 — Make your first meaningful commits
At least three commits, each with a Conventional Commit message: .gitignore, README, and one small improvement of your choice (for example, a new office in data/offices.csv with a test). Push and tag v0.1.
