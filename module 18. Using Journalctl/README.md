## Prerequizites

 1. Log in to VM as devops user and run Terminal (Applications - System Tools - Terminal)

## Tasks

1. Check status of httpd service. Is it running?

2. Comment out line `Listen 80` in `httpd.conf` file, then restart httpd service. What happend?

3. Open journal by running `journalctl -xe`. Find error message in the end. What caused the problem with httpd?

4. Uncomment line `Listen 80` from `httpd.conf`, then restart httpd service.

5. Check status of httpd service. Is it running now?

6. Display only messages about httpd by running `journalctl -u httpd.service`. Did service start normally?

7. Check boot logs with `journalctl -b`. Can you find info about previous boots?

8. Check last 15 strings of the journal by running `journalctl -n 15`.


## Helpful Materials
- https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/system_administrators_guide/ch-viewing_and_managing_log_files
- https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/system_administrators_guide/s1-using_the_journal
