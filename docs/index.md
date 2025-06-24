## SFTP-MkDocs

<https://github.com/fu-sen/SFTP-MkDocs>

**MkDocs with SFTP (minimal configuration)**

- [MkDocs](https://www.mkdocs.org/)

## How to use

1. Edit `mkdocs.yml` and `docs/index.md`, add more files if needed.
2. Add the pip package to `requirements.txt` . (Themes and plugins)
3. Select `Settings` for your GitHub project.
4. Select `Secrets and variables ` in `Secrets`.
5. Select `Actions`
6. Select `New repository secrets`.
7. Add the following name and value:
    - SFTP_HOST: SFTP server name
    - SFTP_PORT: SFTP port number
    - FTP_SUSERNAME: SFTP user name
    - FTP_SPASSWORD: SFTP password
    - SFTP_PRIVATEKEY: SSH private key
    - SFTP_PASSPHASE: Passphase of SSH private key
    - SFTP_REMOTEDIR: Destination SFTP server directory
8. Commit to a GitHub project: `git push`

Please check with your FTP client before configuring.  
