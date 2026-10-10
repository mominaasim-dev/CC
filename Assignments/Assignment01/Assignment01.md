# Assignment 01

**Student Name:** Momina Asim
**Registration Number:** fa24b1-se-069
**GitHub Username:** mominaasim-dev

## Task 1 — Install Gitea and Push a Repository from the Ubuntu Server

- Installed Docker Engine and Docker Compose on the Ubuntu server.
- Cloned instructor's Gitea repository and started Gitea + PostgreSQL via `docker compose up -d`.
- Verified: `docker compose ps` showed both `gitea` and `gitea_db` running; `curl http://127.0.0.1:3000/` returned HTTP status **200**.
- Completed Gitea installation wizard with PostgreSQL settings (`db:5432`, user `gitea`, db `gitea`), Server domain `192.168.182.129`, Gitea base URL `http://192.168.182.129:3000/`.
- Created the public Gitea repository `Assignment01` (empty, no README).
- Created a separate local repo `~/Asignment01` with `README.md` containing full name and registration number.
- Added the gitea remote (no token in URL) and pushed `main`.
- Screenshots: `task1_gitea_running.png`, `task1_gitea_push.png`, `task1_gitea_repository.png`.

## Task 2 — Push the Same Repository to GitHub

- Created the public GitHub repository `Assignment01`.
- Added the github remote: `https://github.com/mominaasim-dev/Assignment01.git`.
- Verified both remotes with `git remote -v` (no tokens visible).
- Pushed `main` to GitHub successfully using a Personal Access Token.
- Screenshots: `task2_remotes.png`, `task2_github_push.png`, `task2_github_repository.png`.

## Task 3 — Track Three Large Files with Git LFS

- `git lfs install`, `git lfs version`, `git lfs track "*.bin"` — `.gitattributes` shows `*.bin filter=lfs diff=lfs merge=lfs -text`.
- Created three files >100 MiB: `large-file-1.bin` (101 MB), `large-file-2.bin` (102 MB), `large-file-3.bin` (103 MB).
- Verified with `git lfs ls-files --size`.
- Committed and pushed to GitHub — LFS upload completed at 100% (3/3).
- Screenshots: `task3_lfs_setup.png`, `task3_lfs_files.png`, `task3_lfs_push.png`.

## Task 4 — Create a Portfolio with GitHub Pages

- Created public repo `mominaasim-dev.github.io`.
- Added `index.html` and `styles.css` with sections: About Me, Education, Skills, Projects.
- Pushed to `main`.
- Enabled GitHub Pages: Deploy from a branch → main / (root).
- Site live at: **https://mominaasim-dev.github.io/**
- Screenshots: `task4_pages_repository.png`, `task4_pages_deployment.png`, `task4_portfolio_live.png`.

## Submission Links

- CC: https://github.com/mominaasim-dev/CC
- Assignment01: https://github.com/mominaasim-dev/Assignment01
- Portfolio: https://mominaasim-dev.github.io/
