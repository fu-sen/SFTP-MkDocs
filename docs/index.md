## FTP-MkDocs

<https://github.com/fu-sen/FTP-MkDocs>

**MkDocs with FTP (minimal configuration)**

- [MkDocs](https://www.mkdocs.org/)

## How to use

1. Edit `mkdocs.yml` and `docs/index.md`, add more files if needed.
2. Add the pip package to `requirements.txt` . (Themes and plugins)
3. Select `Settings` for your GitHub project.
4. Select `Secrets and variables ` in `Secrets`.
5. Select `Actions`
6. Select `New repository secrets`.
7. Add the following name and value:
    - FTP_SERVER: FTP server name
    - FTP_USERNAME: FTP user name
    - FTP_PASSWORD: FTP password
    - FTP_PROTOCOL: `ftp` or `ftps` (`ftps` is recommended)
    - FTP_SERVERDIR: Destination FTP server directory ()
8. Commit to a GitHub project: `git push`

Please check with your FTP client before configuring.  
