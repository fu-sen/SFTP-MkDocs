<!-- 2025/06/22 MkDocs 1.6.1 -->

## FTP-MkDocs

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

## Note

If you have created `.htaccess` ,  
please include the file in the `docs/` folder.

## Build error

Many of the build error are that you mistyped `mkdocs.yml`
or you forgot to add the package to` requirements.txt`.
Check the file change immediately before the error occurred.

This is often not a problem with this project.
You should not open an issue for that.
